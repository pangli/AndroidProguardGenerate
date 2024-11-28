# Android混淆字典生成工具

### 使用**ProguardGenerateClass**生成你认为比较乱的一些规则。

- `comm_dict.txt`文件是由`ProguardGenerateClassOne.java`生成，`output_dict.txt`是在`comm_dict.txt`
  基础上由`ProguardGenerateClassTwo.java`生成，添加了一些其他的字符，使得更加的乱。

- `comm_dict.txt`和`output_dict.txt`是生成输出的文件，可以直接使用。

#### 使用

在我们的混淆文件中，添加以下规则即可：

```
-obfuscationdictionary output_dict.txt
-classobfuscationdictionary output_dict.txt
-packageobfuscationdictionary output_dict.txt
```