__`用户数据报协议（UDP，User Datagram Protocol）`__
Internet 协议集[^1]支持一个无连接的[传输协议](https://baike.baidu.com/item/%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/8048821)，提供面向事务的简单不可靠信息传送服务，该协议称为用户数据报协议。UDP为应用程序提供了一种无需建立连接就可以发送封装的IP数据包的方法。RFC 768描述了UDP。
Internet 的传输层有两个主要协议，互为补充。无连接的是 UDP，它除了给应用程序发送数据包功能并允许它们在所需的层次上架构自己的协议之外，几乎没有做什么特别的事情。面向连接的是[[TCP]]，该协议几乎做了所有的事情。
UDP协议与[[TCP]]协议一样用于处理数据包，在[OSI](https://baike.baidu.com/item/OSI)模型中，两者都位于[传输层](https://baike.baidu.com/item/%E4%BC%A0%E8%BE%93%E5%B1%82/4329536)，处于IP协议的上一层。UDP有不提供数据包分组、组装和不能对数据包进行排序的缺点，也就是说，当报文发送之后，是无法得知其是否安全完整到达的。UDP用来支持那些需要在计算机之间传输数据的网络应用。包括[网络视频会议](https://baike.baidu.com/item/%E7%BD%91%E7%BB%9C%E8%A7%86%E9%A2%91%E4%BC%9A%E8%AE%AE)系统在内的众多的客户/服务器模式的网络应用都需要使用UDP协议。


[^1]:Internet协议（Internet Protocol）是一个协议簇的总称，其本身并不是任何协议。一般有[文件传输协议](https://baike.baidu.com/item/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/1874113)、[电子邮件协议](https://baike.baidu.com/item/%E7%94%B5%E5%AD%90%E9%82%AE%E4%BB%B6%E5%8D%8F%E8%AE%AE/4105152)、[超文本传输协议](https://baike.baidu.com/item/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/8535513)、通信协议等。