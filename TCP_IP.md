# __`TCP/IP`__

^7b5a65

**[互联网](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91)协议套件**（英语：Internet Protocol Suite，缩写IPS）是网络通信模型，以及整个[网络传输协议(Communications Protocol)](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "网络传输协议")家族，为[网际网络](https://zh.wikipedia.org/wiki/%E7%BD%91%E9%99%85%E7%BD%91%E7%BB%9C "网际网络")的基础通信架构。它常通称为**TCP/IP协议族**（英语：TCP/IP Protocol Suite，或TCP/IP Protocols），简称TCP/IP。因为该协议家族的两个核心协议：TCP（[传输控制协议](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "传输控制协议")）和IP（[网际协议](https://zh.wikipedia.org/wiki/%E7%BD%91%E9%99%85%E5%8D%8F%E8%AE%AE "网际协议")），为该家族中最早通过的标准。由于在网络通讯协议普遍采用分层的结构，当多个层次的协议共同工作时，类似计算机科学中的[堆栈](https://zh.wikipedia.org/wiki/%E5%A0%86%E6%A0%88 "堆栈")，因此又称为**TCP/IP协议栈（英语：TCP/IP Protocol Stack）**。
-   一个简单的路由器上可能会实现[ARP](https://zh.wikipedia.org/wiki/%E5%9C%B0%E5%9D%80%E8%A7%A3%E6%9E%90%E5%8D%8F%E8%AE%AE "地址解析协议")，[IP](https://zh.wikipedia.org/wiki/%E7%BD%91%E9%99%85%E5%8D%8F%E8%AE%AE "网际协议")，[ICMP](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E6%8E%A7%E5%88%B6%E6%B6%88%E6%81%AF%E5%8D%8F%E8%AE%AE "互联网控制消息协议")，[UDP](https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE "用户数据报协议")，[SNMP](https://zh.wikipedia.org/wiki/%E7%AE%80%E5%8D%95%E7%BD%91%E7%BB%9C%E7%AE%A1%E7%90%86%E5%8D%8F%E8%AE%AE "简单网络管理协议")，[RIP](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E4%BF%A1%E6%81%AF%E5%8D%8F%E8%AE%AE "路由信息协议")。
-   [WWW](https://zh.wikipedia.org/wiki/%E4%B8%87%E7%BB%B4%E7%BD%91 "万维网")[^1]用户端使用[ARP](https://zh.wikipedia.org/wiki/%E5%9C%B0%E5%9D%80%E8%A7%A3%E6%9E%90%E5%8D%8F%E8%AE%AE "地址解析协议")，[IP](https://zh.wikipedia.org/wiki/%E7%BD%91%E9%99%85%E5%8D%8F%E8%AE%AE "网际协议")，[ICMP](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E6%8E%A7%E5%88%B6%E6%B6%88%E6%81%AF%E5%8D%8F%E8%AE%AE "互联网控制消息协议")，[UDP](https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE "用户数据报协议")，[TCP](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "传输控制协议")，[DNS](https://zh.wikipedia.org/wiki/DNS "DNS")，[HTTP](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "超文本传输协议")，[FTP](https://zh.wikipedia.org/wiki/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "文件传输协议")。
-   一台用户电脑上还会运行如[TELNET](https://zh.wikipedia.org/wiki/TELNET "TELNET")，[SMTP](https://zh.wikipedia.org/wiki/%E7%AE%80%E5%8D%95%E9%82%AE%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "简单邮件传输协议")

TCP/IP提供了点对点链接的机制，将资料应该如何封装、寻址、传输、路由以及在目的地如何接收，都加以标准化。它将软件通信过程[抽象化](https://zh.wikipedia.org/wiki/%E6%8A%BD%E8%B1%A1%E5%8C%96_(%E8%A8%88%E7%AE%97%E6%A9%9F%E7%A7%91%E5%AD%B8) "抽象化 (计算机科学)")为四个[抽象层](https://zh.wikipedia.org/wiki/%E6%8A%BD%E8%B1%A1%E5%B1%A4 "抽象层")，采取[协议堆栈](https://zh.wikipedia.org/w/index.php?title=%E5%8D%94%E5%AE%9A%E5%A0%86%E7%96%8A&action=edit&redlink=1 "协议堆栈（页面不存在）")的方式，分别实现出不同通信协议。TCP/IP协议栈起始于第三层协议IP（[网际协议](https://zh.wikipedia.org/wiki/%E7%B6%B2%E9%9A%9B%E5%8D%94%E8%AD%B0 "网际协议")）。协议族下的各种协议，依其功能不同，分别归属到这四个层次结构之中，常视为是简化的七层[OSI模型](https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B "OSI模型")。 ^c6f43a

所有的TCP/IP应用都必须实现**IP和[ICMP](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E6%8E%A7%E5%88%B6%E6%B6%88%E6%81%AF%E5%8D%8F%E8%AE%AE "互联网控制消息协议")**。对于一个[路由器](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8 "路由器")（router）而言，有这两个协议就可以运作，实际的路由器一般还需要运行许多“推荐”使用的协议，以及一些其他的协议。 

几乎所有连接到互联网上的电脑上都存在的IPv4协议出生在1981年，今天的版本和最早的版本并没有多少改变。升级版IPv6的工作始于1995年，目的在于取代IPv4。ICMP协议主要用于收集有关网络的信息查找错误等工作。

下面试图显示不同的TCP/IP和其他的协议在最初[OSI模型](https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B "OSI模型")中的位置：

7. **应用层**(application layer)
例如[HTTP](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "超文本传输协议")、[SMTP](https://zh.wikipedia.org/wiki/%E7%AE%80%E5%8D%95%E9%82%AE%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "简单邮件传输协议")、[SNMP](https://zh.wikipedia.org/wiki/%E7%AE%80%E5%8D%95%E7%BD%91%E7%BB%9C%E7%AE%A1%E7%90%86%E5%8D%8F%E8%AE%AE "简单网络管理协议")、[FTP](https://zh.wikipedia.org/wiki/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "文件传输协议")、[Telnet](https://zh.wikipedia.org/wiki/Telnet "Telnet")、[SIP](https://zh.wikipedia.org/wiki/%E4%BC%9A%E8%AF%9D%E5%8F%91%E8%B5%B7%E5%8D%8F%E8%AE%AE "会话发起协议")、[SSH](https://zh.wikipedia.org/wiki/Secure_Shell "Secure Shell")、[NFS](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E6%96%87%E4%BB%B6%E7%B3%BB%E7%BB%9F "网络文件系统")、[RTSP](https://zh.wikipedia.org/wiki/RTSP "RTSP")、[XMPP](https://zh.wikipedia.org/wiki/XMPP "XMPP")、[Whois](https://zh.wikipedia.org/wiki/WHOIS "WHOIS")、[ENRP](https://zh.wikipedia.org/w/index.php?title=ENRP&action=edit&redlink=1)、[TLS](https://zh.wikipedia.org/wiki/%E5%82%B3%E8%BC%B8%E5%B1%A4%E5%AE%89%E5%85%A8%E6%80%A7%E5%8D%94%E5%AE%9A "传输层安全性协议")
6. **表示层** (presentation layer)
例如[XDR](https://zh.wikipedia.org/wiki/%E5%A4%96%E9%83%A8%E6%95%B0%E6%8D%AE%E8%A1%A8%E7%A4%BA%E6%B3%95 "外部数据表示法")、[ASN.1](https://zh.wikipedia.org/wiki/ASN.1 "ASN.1")、[NCP](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "网络控制协议")、[TLS](https://zh.wikipedia.org/wiki/TLS "TLS")、[ASCII](https://zh.wikipedia.org/wiki/ASCII "ASCII")
5. **会话层** (session layer)
例如[ASAP](https://zh.wikipedia.org/w/index.php?title=ASAP&action=edit&redlink=1)、ISO 8327 / CCITT X.225、[RPC](https://zh.wikipedia.org/wiki/%E9%81%A0%E7%A8%8B%E9%81%8E%E7%A8%8B%E8%AA%BF%E7%94%A8 "远程过程调用")、[NetBIOS](https://zh.wikipedia.org/wiki/NetBIOS "NetBIOS")、[Winsock](https://zh.wikipedia.org/wiki/Winsock "Winsock")、[BSD sockets](https://zh.wikipedia.org/wiki/Berkeley%E5%A5%97%E6%8E%A5%E5%AD%97 "Berkeley套接字")、[SOCKS](https://zh.wikipedia.org/wiki/SOCKS "SOCKS")、[PAP](https://zh.wikipedia.org/w/index.php?title=%E5%AF%86%E7%A2%BC%E9%A9%97%E8%AD%89%E5%8D%94%E8%AD%B0&action=edit&redlink=1 "密码验证协议（页面不存在）")
4. **传输层**(transport layer)
例如[TCP](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "传输控制协议")、[UDP](https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE "用户数据报协议")、[RTP](https://zh.wikipedia.org/wiki/%E5%AE%9E%E6%97%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "实时传输协议")、[SCTP](https://zh.wikipedia.org/wiki/%E6%B5%81%E6%8E%A7%E5%88%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "流控制传输协议")、[SPX](https://zh.wikipedia.org/wiki/%E5%BA%8F%E5%88%97%E5%88%86%E7%B5%84%E4%BA%A4%E6%8F%9B "串行分组交换")、[ATP](https://zh.wikipedia.org/wiki/AppleTalk "AppleTalk")
3. **网络层**(network layer)
例如[IP](https://zh.wikipedia.org/wiki/%E7%BD%91%E9%99%85%E5%8D%8F%E8%AE%AE "网际协议")、[ICMP](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E6%8E%A7%E5%88%B6%E6%B6%88%E6%81%AF%E5%8D%8F%E8%AE%AE "互联网控制消息协议")、[IPX](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E5%88%86%E7%BB%84%E4%BA%A4%E6%8D%A2%E5%8D%8F%E8%AE%AE "互联网分组交换协议")、[BGP](https://zh.wikipedia.org/wiki/%E8%BE%B9%E7%95%8C%E7%BD%91%E5%85%B3%E5%8D%8F%E8%AE%AE "边界网关协议")、[OSPF](https://zh.wikipedia.org/wiki/OSPF "OSPF")、[RIP](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E4%BF%A1%E6%81%AF%E5%8D%8F%E8%AE%AE "路由信息协议")、[IGRP](https://zh.wikipedia.org/wiki/IGRP "IGRP")、[EIGRP](https://zh.wikipedia.org/wiki/EIGRP "EIGRP")、[ARP](https://zh.wikipedia.org/wiki/%E5%9C%B0%E5%9D%80%E8%A7%A3%E6%9E%90%E5%8D%8F%E8%AE%AE "地址解析协议")、[RARP](https://zh.wikipedia.org/wiki/RARP "RARP")、[X.25](https://zh.wikipedia.org/wiki/X.25 "X.25")
2. **数据链路层**(data link layer)
例如[以太网](https://zh.wikipedia.org/wiki/%E4%BB%A5%E5%A4%AA%E7%BD%91 "以太网")、[令牌环](https://zh.wikipedia.org/wiki/%E4%BB%A4%E7%89%8C%E7%8E%AF "令牌环")、[HDLC](https://zh.wikipedia.org/wiki/HDLC "HDLC")、[帧中继](https://zh.wikipedia.org/wiki/%E5%B8%A7%E4%B8%AD%E7%BB%A7 "帧中继")、[ISDN](https://zh.wikipedia.org/wiki/ISDN "ISDN")、[ATM](https://zh.wikipedia.org/wiki/%E5%BC%82%E6%AD%A5%E4%BC%A0%E8%BE%93%E6%A8%A1%E5%BC%8F "异步传输模式")、[IEEE 802.11](https://zh.wikipedia.org/wiki/IEEE_802.11 "IEEE 802.11")、[FDDI](https://zh.wikipedia.org/wiki/FDDI "FDDI")、[PPP](https://zh.wikipedia.org/wiki/%E7%82%B9%E5%AF%B9%E7%82%B9%E5%8D%8F%E8%AE%AE "点对点协议")
1. **物理层**(physical layer)
例如[调制解调器](https://zh.wikipedia.org/wiki/%E6%95%B8%E6%93%9A%E6%A9%9F "调制解调器")、[无线电](https://zh.wikipedia.org/wiki/%E6%97%A0%E7%BA%BF%E7%94%B5 "无线电")、[光纤](https://zh.wikipedia.org/wiki/%E5%85%89%E7%BA%A4 "光纤")

通常人们认为OSI模型的最上面三层（应用层、表示层和会话层）在TCP/IP组中是一个应用层。由于TCP/IP有一个相对较弱的会话层，由TCP和RTP下的打开和关闭连接组成，并且在TCP和UDP下的各种应用提供不同的端口号，这些功能能够由单个的应用程序（或者那些应用程序所使用的库）增加。与此相似的是，IP是按照将它下面的网络当作一个黑盒子的思想设计的，这样在讨论TCP/IP的时候就可以把它当作一个独立的层。

4. **应用层**(application layer)
例如[HTTP](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "超文本传输协议")、[FTP](https://zh.wikipedia.org/wiki/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "文件传输协议")、[DNS](https://zh.wikipedia.org/wiki/DNS "DNS")  
_（如[BGP](https://zh.wikipedia.org/wiki/%E8%BE%B9%E7%95%8C%E7%BD%91%E5%85%B3%E5%8D%8F%E8%AE%AE "边界网关协议")和[RIP](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E4%BF%A1%E6%81%AF%E5%8D%8F%E8%AE%AE "路由信息协议")这样的路由协议，尽管由于各种各样的原因它们分别运行在TCP和UDP上，仍然可以将它们看作网络层的一部分）_
3. **传输层**(transport layer)
例如[TCP](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "传输控制协议")、[UDP](https://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E6%95%B0%E6%8D%AE%E6%8A%A5%E5%8D%8F%E8%AE%AE "用户数据报协议")、[RTP](https://zh.wikipedia.org/wiki/RTP "RTP")、[SCTP](https://zh.wikipedia.org/wiki/SCTP "SCTP")  
_（如[OSPF](https://zh.wikipedia.org/wiki/OSPF "OSPF")这样的路由协议，尽管运行在IP上也可以看作是网络层的一部分）_
2. **网络互连层**(internet layer)
对于TCP/IP来说这是[因特网协议](https://zh.wikipedia.org/wiki/%E5%9B%A0%E7%89%B9%E7%BD%91%E5%8D%8F%E8%AE%AE "因特网协议")（IP）  
_（如[ICMP](https://zh.wikipedia.org/wiki/%E4%BA%92%E8%81%94%E7%BD%91%E6%8E%A7%E5%88%B6%E6%B6%88%E6%81%AF%E5%8D%8F%E8%AE%AE "互联网控制消息协议")和[IGMP](https://zh.wikipedia.org/wiki/%E5%9B%A0%E7%89%B9%E7%BD%91%E7%BB%84%E7%AE%A1%E7%90%86%E5%8D%8F%E8%AE%AE "因特网组管理协议")这样的必须协议尽管运行在IP上，也仍然可以看作是网络互连层的一部分；[ARP](https://zh.wikipedia.org/wiki/%E5%9C%B0%E5%9D%80%E8%A7%A3%E6%9E%90%E5%8D%8F%E8%AE%AE "地址解析协议")不运行在IP上）_
1.**网络访问（链接）层**  (Network Access (link) layer)
例如[以太网](https://zh.wikipedia.org/wiki/%E4%BB%A5%E5%A4%AA%E7%BD%91 "以太网")、[Wi-Fi](https://zh.wikipedia.org/wiki/Wi-Fi "Wi-Fi")、[MPLS](https://zh.wikipedia.org/wiki/%E5%A4%9A%E5%8D%8F%E8%AE%AE%E6%A0%87%E7%AD%BE%E4%BA%A4%E6%8D%A2 "多协议标签交换")等。

[^1]:万维网并不等同互联网，万维网只是互联网所能提供的服务其中之一，是靠着互联网运行的一项服务。
***
# __`TCP（Transmission Control Protocol）`__
传输控制协议（TCP，Transmission Control Protocol）是一种面向连接的、可靠的、基于字节流的端到端传输层通信协议，由IETF的RFC 793定义。

TCP旨在适应支持多网络应用的分层协议层次结构。互联网络与单个网络有很大的不同，因为互联网络的不同部分可能有截然不同的拓扑结构、带宽、延迟、数据包大小和其他参数。TCP的设计目标是能够动态地适应互联网络的这些特性，而且具备面对各种故障时的健壮性。
开放系统互联（Open System Interconnection）：
![[Pasted image 20220827225111.png]]
TCP工作在网络[[#^c6f43a|OSI]]的七层模型中的第四层——传输层，IP在第三层——网络层，ARP 在第二层——数据链路层；同时，我们需要简单的知道，数据从应用层发下来，会在每一层都会加上头部信息，进行封装，然后再发送到数据接收端。这个基本的流程你需要知道，就是每个数据都会经过数据的封装和解封装的过程。
![[Pasted image 20220827230424.png]]
tcp协议比较复杂，因为它要实现可靠传输，为了确保它的可靠传输，于是协议就相当复杂了。它的主要特点是：
-   面向连接，就像打电话一样，必须一对一的接通电话，两个人才能讲电话，而udp有点像发微信，不需要对方做准备，我想发就发
-   点对点，每一条tcp连接只能是点对点，一对一
-   提供可靠交付，通过tcp传送的数据，无差错，不丢失，不重复，并且按序到达
-   全双工通信，即tcp双方都有缓存，发送方将数据传送给tcp缓存之后就可以做自己的事了，接收方在适当的时候读取缓存
-   面向字节流

可靠传输原理：
ip层只提供尽最大努力服务，也就是说，tcp层之下的网络所提供的是不可靠的传输，那么，tcp要采用什么措施才能实现可靠传输呢？
理想的传输条件有两个特点：
-   传输信道不产生差错；
-   不管发送方以多快的速率发送数据，接收方也来得及处理。
但实际上不可能的，网络总是变化的，有好有快，而且根据木桶理论，只要有一环较差，网络就好不起来。另外，接收主机的性能也有好有坏，数据处理自然也会有快有慢了。
如果网络不好，我没有收到传输的数据，可以让发送方重新发送数据。如果我处理数据的速度有限，可以告诉发送方速度不要过快，在某个速度之下。这就是tcp可靠传输的基本思想。

停止等待协议：
停止等待，就是每发送完一个分组就停止发送，等待对方确认，收到确认后再发送下一个分组。如果按照这个策略，那么传输肯定是可靠的，因为每个数据对方都会确认是否收到。
在无差错的情况下，情况如图所示：
![](https://pic3.zhimg.com/80/v2-0d3c6390ff115840f641c7949e2022f2_720w.jpg)
发送方发送一帧后，就会启用超时计数器，在计数时间范围内，如果还没有收到接收方发送过来的确认，那么就认为数据已丢失，就需要重新发送一次
![](https://pic1.zhimg.com/80/v2-c07b77f9af4fe9f5042198432a996a8c_720w.jpg)
这样做，肯定是可靠传输的，但有个问题，信道复用率太低，发送方发送完之后就处于等待之中了，整个网络会处于巨大浪费之中。
![](https://pic3.zhimg.com/80/v2-9b6bfe2a307372452155134042833792_720w.jpg)
为了解决信道利用率低的问题，就需要使用连续ARQ协议和滑动窗口协议了。
![](https://pic4.zhimg.com/80/v2-718fbe1af085fe5dba147be654e3876b_720w.jpg)
如上图所示，发送方维持着一个发送窗口，它的意义是，发送窗口内的5个分组都可以连续地发送出去，而不需要等待对方的确认，这样信道利用率就高了。发送完一个分组后，窗口向前滑动，新的发送窗口就包含2到6这五个分组了，这就是滑动窗口。发送方每收到一个确认，就会把发送窗口向前滑动一个分组的位置。如上图，如果收到分组1的确认，发送窗口就滑动到6的位置了。
但接收方一般采用累积确认的方式，也就是说，接收方不必对收到的分组作逐个确认，而是在收到几个分组后，对按序到达的最后一个分组做确认就行，这就表示，到这个分组为止的所有分组都已确认。比如说，发送方发送完2到6之后，接收方发送6的确认，发送方就认为2到6都已经收到了，于是向前滑动5个分组，新的发送窗口变成7到11。
但这里有一个条件，接收方只对按序到达的最后一个分组作确认，如果接收方只收到2、3、6三个分组，4和5没有收到，那么接收方应该只发送3的确认。如果超时后还没有收到4和5的确认，会重新发送4、5、6，6也会被重发。

超时时间选择：
A向B发送了一个报文，但因为网络不好，B发送的确认报文A迟迟没有收到，A很着急，于是重发报文，但网络堵塞在那，A依然无法收到B的确认报文，反而因为A发了多次，导致网络更加堵塞了。
所以，有个关键问题，超时时间该如何确定呢？太短会引起很多不必要的重传，太长也不行，会让网络的空闲时间增大，影响效率。
TCP采用一种自适应算法。它记录一个报文段发出的时间，以及收到相应确认的时间，这两个时间之差不是报文段的往返时间RTT。
![](https://pic3.zhimg.com/80/v2-230752717c3ae3bb0066aa183b6eeba6_720w.jpg)
**新的加权平均往返时间RTTs = （1 - a）x 旧的RTTs + a x** **_新的RTT样本。_(其中0 < a < 1)**  
如果 a很小，趋近于0，说明新的RTT样本作用不大。  
如果 a 很大，趋近于1，则说明旧的RTTs对新的RTTs的影响很小。
当第一次取到RTT样本时，RTTs = RTT

现在通用的a的取值为1/8，即0.125。  
显然，新的RT0的值应该要略大于RTTs的值。  
**RTO = RTTs + 4 x RTTd（RTTd为RTT偏差的加权平均）**

第一次测量时，RTTd1 = RTT1 / 2
  
**新的RTTd = (1-B) x 旧的RTTd+B x |RTTs-_新的RTT样本_|** **。 (其中0< B<1)**  
B的建议取值为1/4，即0.25

当报文段重传时，就把超时重传时间RTO增大一些，典型的做法就是把新的重传时间设置为旧的重传时间的2倍。

流量控制：
网络的带宽有限，端处理数据速度有限，发送数据的速度应该要有限制，TCP使用滑动窗口来控制流量。
tcp的首部中，有个窗口字段，窗口字段告诉发送方，接收方此时还能最多接收多少数据。
另外，为了增加网络使用效率，tcp的数据字段也不宜过短，比如每次只发送一个字节的数据，这明显是不合适，因为tcp的首部至少有20字节，ip协议的首部也要20字节，整个tcp报文段不可能发这么多首部，而数据只有可怜的一点点。但如果报文长度太长了，也有问题，过长则需要分片，而分片了，效率就会降低。所以目前默认规定的最大报文长度MSS，为536字节。

拥塞控制：
假设端上处理能力非常强，有多少处理多少。那么发送端能无限制任意发送吗？明显是不行的，接收端处理能力强，不代表网络的带宽情况。如果网络拥堵的情况下，发送端发得过多，接收端依然收不到，还会导致大量的重发，效率相当低下。所以需要拥塞控制。
![](https://pic4.zhimg.com/80/v2-2036c3386d49ffcfa420cb024adce0b7_720w.jpg)
如何防止拥塞，其实用的是一种探测的思想，因为没有任何直接的可量化的参数能表明当前的网络拥塞程序，所以只好不停的探测，让网络处于一个较为高效的状态。
通常使用的方法叫慢开始。它的思路是这样的，当主机开始发送数据的时候，由小到大逐渐增大发送窗口，通常是在刚开始发送的时候，先把拥塞窗口设置为一个最大报文段MSS的数值，而在每收到一个对新的报文段的确认后，把拥塞窗口增加到多一个MSS的数据。用这样的方法逐步增大，可以让分组注入网络的速率更加合理。
拥塞窗口是发送端维持的一个状态变量，发送方让自己的发送窗口等于拥塞窗口。

## __`三次握手（Three-way handshake）`__
通信双方的三次TCP(Transmission Control Protocol)报文段[^2]的交换过程，也就是通常所说的TCP连接建立实现的三次握手(Three-Way Handshake)过程。所谓的“三次握手”，是为了对每次发送的数据量进行跟踪与协商，确保数据段的发送和接收同步，根据所接收到的数据量而确认数据发送、接收完毕后何时撤消联系，并建立虚连接。
![[Pasted image 20220824224939.png]]
为了建立连接TCP连接，通信双方必须从对方了解如下信息：对方报文发送的开始序号、对方发送数据的缓冲区大小、能被接收的最大报文段长度MSS（Maximum Segment Size）、被支持的TCP选项。
当连接建立完成之后，则：
1. TCP连接的通信双方均可知道连接上对方将被发送的第一个字节的序列号（发给对方的确认号，A发给B的确认号就是B将发送的序列号，同样B也是）；
2. 双方均可知道连接上能发送的MSS，从而即可选取握手阶段双方交换的SYN报文和SYN+ACK报文中MSS选项中较小的值作为实际值；
3. 双方均可知道对方的接收缓冲区大小；
4. 双方均可知道对方能否使用SACK、窗口缩放等选项。
基于这些信息，双方即可建立一个TCP连接(x，y)并基于该连接开始报文段的传输。

1. 第一次握手：建立连接时，[客户端](https://baike.baidu.com/item/%E5%AE%A2%E6%88%B7%E7%AB%AF)发送[syn](https://baike.baidu.com/item/syn)包（seq=j）到[服务器](https://baike.baidu.com/item/%E6%9C%8D%E5%8A%A1%E5%99%A8)，并进入[SYN_SENT](https://baike.baidu.com/item/SYN_SENT)状态，等待服务器确认；SYN：同步序列编号（Synchronize Sequence Numbers）。
2. 第二次握手：服务器收到syn包，必须确认客户端的SYN（[ack](https://baike.baidu.com/item/ack)=j+1），同时自己也发送一个SYN包（seq=k），即SYN+ACK)包，此时服务器进入[SYN_RECV](https://baike.baidu.com/item/SYN_RECV)状态。
3. 第三次握手：客户端收到服务器的SYN+ACK包，向服务器发送确认包ACK(ack=k+1)，此包发送完毕，客户端和服务器进入[ESTABLISHED](https://baike.baidu.com/item/ESTABLISHED)（TCP连接成功）状态，完成三次握手。

## __`四次挥手`__
对于一个已经建立的连接，TCP使用改进的四次挥手来释放连接（使用一个带有FIN附加标记的报文段）。TCP关闭连接的步骤如下：
1. 第一步，当主机A的应用程序通知TCP数据已经发送完毕时，TCP向主机B发送一个带有FIN附加标记的报文段（FIN表示英文finish）；
2. 第二步，主机B收到这个FIN报文段之后，并不立即用FIN报文段回复主机A，而是先向主机A发送一个确认序号ACK，同时通知自己相应的应用程序：对方要求关闭连接（先发送ACK的目的是为了防止在这段时间内，对方重传FIN报文段）；
3. 第三步，主机B的应用程序告诉TCP：我要彻底的关闭连接，TCP向主机A送一个FIN报文段；
4. 第四步，主机A收到这个FIN报文段后，向主机B发送一个ACK表示连接彻底释放。

[^2]:TCP提供的是一种面向连接的，可靠的字节流服务，TCP提供可靠性的一种重要的方式就是MSS。通过MSS，应用数据被分割成TCP认为最适合发送的数据块，由TCP传递给IP的信息单位称为报文段或段(segment)。代表一个TCP socket的结构体struct tcp_sock中有多个成员用于确定应用数据被分割成最大为多大的数据块较为合适(最大报文段长度MSS)。

# __`用户数据报协议（UDP，User Datagram Protocol）`__
Internet 协议集[^3]支持一个**无连接**的[传输协议](https://baike.baidu.com/item/%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/8048821)，提供面向事务的简单不可靠信息传送服务，该协议称为用户数据报协议。UDP为应用程序提供了一种无需建立连接就可以发送封装的IP数据包的方法。RFC 768描述了UDP。

Internet 的传输层有两个主要协议，互为补充。无连接的是 UDP，它除了给应用程序发送数据包功能并允许它们在所需的层次上架构自己的协议之外，几乎没有做什么特别的事情。面向连接的是[[#^7b5a65|TCP]]，该协议几乎做了所有的事情。

UDP协议与[[#^7b5a65|TCP]]协议一样用于处理数据包，在[OSI](https://baike.baidu.com/item/OSI)模型中，两者都位于[传输层](https://baike.baidu.com/item/%E4%BC%A0%E8%BE%93%E5%B1%82/4329536)，处于IP协议的上一层。
- UDP有不提供数据包分组、组装和不能对数据包进行排序的缺点，也就是说，当报文发送之后，是无法得知其是否安全完整到达的；
- 其传输数据之前源端和终端不建立连接， 当它想传送时就简单地去抓取来自应用程序的数据，并尽可能快地把它扔到网络上；在接收端，UDP把每个消息段放在队列中，应用程序每次从队列中读一个消息段；
- 由于传输数据不建立连接，因此也就不需要维护连接状态，包括收发状态等， 因此一台服务机可同时向多个客户机传输相同的消息；
- UDP信息包的标题很短，只有8个字节，相对于TCP的20个字节信息包的额外开销很小；
- 吞吐量不受拥挤控制算法的调节，只受应用软件生成数据的速率、传输带宽、 源端和终端主机性能的限制；
- UDP使用尽最大努力交付，即不保证可靠交付， 因此主机不需要维持复杂的链接状态表。
- UDP是面向报文的。发送方的UDP对应用程序交下来的报文， 在添加首部后就向下交付给IP层。既不拆分，也不合并，而是保留这些报文的边界， 因此，应用程序需要选择合适的报文大小。
- 我们经常使用ping命令来测试两台主机之间TCP/IP通信是否正常， 其实ping命令的原理就是向对方主机发送UDP数据包，然后对方主机确认收到数据包， 如果数据包是否到达的消息及时反馈回来，那么网络就是通的。

UDP用来支持那些需要在计算机之间传输数据的网络应用。包括[网络视频会议](https://baike.baidu.com/item/%E7%BD%91%E7%BB%9C%E8%A7%86%E9%A2%91%E4%BC%9A%E8%AE%AE)系统在内的众多的客户/服务器模式的网络应用都需要使用UDP协议。

[^3]:Internet协议（Internet Protocol）是一个协议簇的总称，其本身并不是任何协议。一般有[文件传输协议](https://baike.baidu.com/item/%E6%96%87%E4%BB%B6%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/1874113)、[电子邮件协议](https://baike.baidu.com/item/%E7%94%B5%E5%AD%90%E9%82%AE%E4%BB%B6%E5%8D%8F%E8%AE%AE/4105152)、[超文本传输协议](https://baike.baidu.com/item/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE/8535513)、通信协议、远程登录（Telnet）、网络管理（SNMP简单网络管理协议）、域名系统（DNS）等。