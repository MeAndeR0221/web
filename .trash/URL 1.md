# __`统一资源定位系统（uniform resource locator : URL）`__
是因特网的万维网服务程序上用于指定信息位置的表示方法。因特网上的可用资源可以用简单字符串来表示，该文档就是描述了这种字符串的语法和语义。

URL通常被写成如下形式：<方案>:<方案描述部分>。
一个URL包含了它使用的方案名称（<方案>）, 其后紧跟一个冒号，然后是一个字符串（<方案描述部分>），这部分的解释由所使用的方案来决定。方案名称由一串字符组成。小写字母“a”——“z”，数字，字符加号（“+”），句点（“.”）和连字号（“-”）都可以。为了方便起见，程序在解释URL的时候应该视方案名称中的大写字母和小写字母一样。（例如：视“HTTP”和“http”一样）。

一些已经存在的标准协议和正处于试验中的协议之间的映射关系的轮廓用BNF语法定义进行描述。下面对一些协议进行了注释：
- ftp : File Transfer protocol（文件传输协议）
- http : Hypertext Transfer Protocol（超文本传输协议）
- news : USENET news（USENET新闻）
- file : Host-specific file names（特殊主机文件名）
----
# __`统一资源标识符（Uniform Resource Identifier : URI）`__
是一个用于标识某一互联网资源名称的字符串。 该种标识允许用户对任何（包括本地和互联网）的资源通过特定的协议进行交互操作。URI由包括确定语法和相关协议的方案所定义。
Web上可用的每种资源 -HTML文档、图像、视频片段、程序等，由一个通用资源标识符进行定位。