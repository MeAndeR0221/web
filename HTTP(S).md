# __`HTTP`__
**超文本传输协议**（**H**yper**T**ext **T**ransfer **P**rotocol）是一种用于分布式、协作式和[超媒体](https://zh.wikipedia.org/wiki/%E8%B6%85%E5%AA%92%E9%AB%94 "超媒体")信息系统的应用层协议。HTTP是[万维网](https://zh.wikipedia.org/wiki/%E5%85%A8%E7%90%83%E8%B3%87%E8%A8%8A%E7%B6%B2 "万维网")的数据通信的基础。
设计HTTP最初的目的是为了提供一种发布和接收[HTML](https://zh.wikipedia.org/wiki/HTML "HTML")页面的方法。通过HTTP或者[HTTPS](https://zh.wikipedia.org/wiki/HTTPS "HTTPS")协议请求的资源由[统一资源标识符](https://zh.wikipedia.org/wiki/%E7%BB%9F%E4%B8%80%E8%B5%84%E6%BA%90%E6%A0%87%E5%BF%97%E7%AC%A6 "统一资源标志符")（Uniform Resource Identifiers，URI）来标识。

HTTP是一个客户端（用户）和服务端（网站）之间请求和应答的标准，通常使用[TCP协议](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E6%8E%A7%E5%88%B6%E5%8D%8F%E8%AE%AE "传输控制协议")。通过使用[网页浏览器](https://zh.wikipedia.org/wiki/%E7%B6%B2%E9%A0%81%E7%80%8F%E8%A6%BD%E5%99%A8 "网页浏览器")、[网络爬虫](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E7%88%AC%E8%99%AB "网络爬虫")或者其它的工具，客户端发起一个HTTP请求到服务器上指定端口（默认[端口](https://zh.wikipedia.org/wiki/%E9%80%9A%E8%A8%8A%E5%9F%A0 "端口")为80）。我们称这个客户端为用户代理程序（user agent）。应答的服务器上存储着一些资源，比如HTML文件和图像。我们称这个应答服务器为源服务器（origin server）。在用户代理和源服务器中间可能存在多个“中间层”，比如[代理服务器](https://zh.wikipedia.org/wiki/%E4%BB%A3%E7%90%86%E4%BC%BA%E6%9C%8D%E5%99%A8 "代理服务器")、[网关](https://zh.wikipedia.org/wiki/%E7%BD%91%E5%85%B3 "网关")或者[隧道](https://zh.wikipedia.org/wiki/%E9%9A%A7%E9%81%93 "隧道")（tunnel）。

尽管[TCP/IP](https://zh.wikipedia.org/wiki/TCP/IP "TCP/IP")协议是互联网上最流行的应用，但是在HTTP协议中并没有规定它必须使用或它支持的层。事实上HTTP可以在任何互联网协议或其他网络上实现。HTTP假定其下层协议提供可靠的传输。因此，任何能够提供这种保证的协议都可以被其使用，所以其在TCP/IP协议族使用TCP作为其传输层。

通常，由HTTP客户端发起一个请求，创建一个到服务器指定端口（默认是80端口）的TCP连接。HTTP服务器则在那个端口监听客户端的请求。一旦收到请求，服务器会向客户端返回一个状态，比如"HTTP/1.1 200 OK"，以及返回的内容，如请求的文件、错误消息、或者其它信息。

HTTP/1.1协议中共定义了八种方法（也叫“动作”）来以不同方式操作指定的资源：
1. GET
向指定的资源发出“显示”请求。使用GET方法应该只用在读取资料，而不应当被用于产生“[副作用](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE#%E5%89%AF%E4%BD%9C%E7%94%A8)”的操作中，例如在[网络应用程序](https://zh.wikipedia.org/wiki/%E7%BD%91%E7%BB%9C%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F "网络应用程序")中。其中一个原因是GET可能会被[网络爬虫](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E7%88%AC%E8%9F%B2 "网络爬虫")等随意访问。参见[安全方法](https://zh.wikipedia.org/wiki/%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE#%E5%AE%89%E5%85%A8%E6%96%B9%E6%B3%95)。浏览器直接发出的GET只能由一个url触发。GET上要在url之外带一些参数就只能依靠url上附带querystring。
2. HEAD
与GET方法一样，都是向服务器发出指定资源的请求。只不过服务器将不传回资源的本文部分。它的好处在于，使用这个方法可以在不必传输全部内容的情况下，就可以获取其中“关于该资源的信息”（元信息或称元数据）。
3. POST
向指定资源提交数据，请求服务器进行处理（例如提交表单或者上传文件）。数据被包含在请求本文中。这个请求可能会创建新的资源或修改现有资源，或二者皆有。每次提交，表单的数据被浏览器用编码到HTTP请求的body里。浏览器发出的POST请求的body主要有两种格式，一种是application/x-www-form-urlencoded用来传输简单的数据，大概就是"key1=value1&key2=value2"这样的格式。另外一种是传文件，会采用multipart/form-data格式。采用后者是因为application/x-www-form-urlencoded的编码方式对于文件这种二进制的数据非常低效。
4. PUT
向指定资源位置上传其最新内容。
5. DELETE
请求服务器删除Request-URI所标识的资源。
6. TRACE
回显服务器收到的请求，主要用于测试或诊断。
7. OPTIONS
这个方法可使服务器传回该资源所支持的所有HTTP请求方法。用"\*"来代替资源名称，向Web服务器发送OPTIONS请求，可以测试服务器功能是否正常运作。
8. CONNECT
HTTP/1.1协议中预留给能够将连接改为隧道方式的代理服务器。通常用于SSL加密服务器的链接（经由非加密的HTTP代理服务器）。

方法名称是区分大小写的。当某个请求所针对的资源不支持对应的请求方法的时候，服务器应当返回[状态码405](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#405 "HTTP状态码")（Method Not Allowed），当服务器不认识或者不支持对应的请求方法的时候，应当返回[状态码501](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#501 "HTTP状态码")（Not Implemented）。

**HTTP服务器至少应该实现GET和HEAD方法**，其他方法都是可选的。当然，所有的方法支持的实现都应当符合下述的方法各自的语义定义。此外，除了上述方法，特定的HTTP服务器还能够扩展自定义的方法。例如PATCH（由 [RFC 5789](https://tools.ietf.org/html/rfc5789) 指定的方法），用于将局部修改应用到资源。

所有HTTP响应的第一行都是**状态行**，依次是当前HTTP版本号，3位数字组成的 **[状态代码](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81 "HTTP状态码")**，以及描述状态的短语，彼此由空格分隔。

状态代码的第一个数字代表当前响应的类型：
-   [1xx消息](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#1xx%E6%B6%88%E6%81%AF "HTTP状态码")——请求已被服务器接收，继续处理
-   [2xx成功](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#2xx%E6%88%90%E5%8A%9F "HTTP状态码")——请求已成功被服务器接收、理解、并接受
-   [3xx重定向](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#3xx%E9%87%8D%E5%AE%9A%E5%90%91 "HTTP状态码")——需要后续操作才能完成这一请求
-   [4xx请求错误](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#4xx%E8%AF%B7%E6%B1%82%E9%94%99%E8%AF%AF "HTTP状态码")——请求含有词法错误或者无法被执行
-   [5xx服务器错误](https://zh.wikipedia.org/wiki/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#5xx%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%94%99%E8%AF%AF "HTTP状态码")——服务器在处理某个正确请求时发生错误

# __`HTTPS`__
**超文本传输安全协议**（**H**yper**T**ext **T**ransfer **P**rotocol **S**ecure），常称为HTTP over TLS、HTTP over SSL或HTTP Secure，是一种通过[计算机网络](https://zh.wikipedia.org/wiki/%E8%A8%88%E7%AE%97%E6%A9%9F%E7%B6%B2%E7%B5%A1 "计算机网络")进行安全通信的[传输协议](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E5%82%B3%E8%BC%B8%E5%8D%94%E5%AE%9A "网络传输协议")。HTTPS经由[[#__ HTTP __|HTTP]]进行通信，但利用[SSL/TLS](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E5%B1%82%E5%AE%89%E5%85%A8 "传输层安全")来[加密](https://zh.wikipedia.org/wiki/%E5%8A%A0%E5%AF%86 "加密")数据包。HTTPS开发的主要目的，是提供对[网站](https://zh.wikipedia.org/wiki/%E7%B6%B2%E7%AB%99 "网站")服务器的[身份认证](https://zh.wikipedia.org/wiki/%E8%BA%AB%E4%BB%BD%E9%AA%8C%E8%AF%81 "身份验证")，保护交换资料的隐私与[完整性](https://zh.wikipedia.org/wiki/%E5%AE%8C%E6%95%B4%E6%80%A7 "完整性")。这个协议由[网景](https://zh.wikipedia.org/wiki/%E7%B6%B2%E6%99%AF "网景")公司（Netscape）在1994年首次提出，随后扩展到[互联网](https://zh.wikipedia.org/wiki/%E7%B6%B2%E9%9A%9B%E7%B6%B2%E8%B7%AF "互联网")上。

历史上，HTTPS连接经常用于[万维网](https://zh.wikipedia.org/wiki/%E4%B8%87%E7%BB%B4%E7%BD%91 "万维网")上的交易支付和企业信息系统中敏感信息的传输。在2000年代末至2010年代初，HTTPS开始广泛使用，以确保各类型的网页真实，保护账户和保持用户通信，身份和网络浏览的私密性。

另外，还有一种[安全超文本传输协议](https://zh.wikipedia.org/wiki/%E5%AE%89%E5%85%A8%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "安全超文本传输协议")（S-HTTP）的HTTP安全传输实现，但是HTTPS的广泛应用而成为事实上的HTTP安全传输实现，S-HTTP并没有得到广泛支持。

HTTPS的主要作用是在不安全的网络上创建一个安全信道，并可在使用适当的加密包和服务器证书可被验证且可被信任时，对[窃听](https://zh.wikipedia.org/wiki/%E7%AB%8A%E8%81%BD "窃听")和[中间人攻击](https://zh.wikipedia.org/wiki/%E4%B8%AD%E9%97%B4%E4%BA%BA%E6%94%BB%E5%87%BB "中间人攻击")提供合理的防护。

HTTPS的信任基于预先安装在[操作系统](https://zh.wikipedia.org/wiki/%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F "操作系统")中的[证书颁发机构](https://zh.wikipedia.org/wiki/%E8%AF%81%E4%B9%A6%E9%A2%81%E5%8F%91%E6%9C%BA%E6%9E%84 "证书颁发机构")（CA）。因此，与一个网站之间的HTTPS连线仅在这些情况下可被信任：

-   浏览器正确地实现了HTTPS且操作系统中安装了正确且受信任的证书颁发机构；
-   证书颁发机构仅信任合法的网站；
-   被访问的网站提供了一个有效的证书，也就是说它是一个由操作系统信任的证书颁发机构签发的（大部分浏览器会对无效的证书发出警告）；
-   该证书正确地验证了被访问的网站（例如，访问`https://example.com`时收到了签发给`example.com`而不是其它[域名](https://zh.wikipedia.org/wiki/%E5%9F%9F%E5%90%8D "域名")的证书）；
-   此协议的加密层（[SSL/TLS](https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E5%B1%82%E5%AE%89%E5%85%A8 "传输层安全")）能够有效地提供认证和高强度的加密。

不应将HTTPS和在[RFC 2660](https://tools.ietf.org/html/rfc2660)中定义的[安全超文本传输协议](https://zh.wikipedia.org/wiki/%E5%AE%89%E5%85%A8%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE "安全超文本传输协议")（S-HTTP）相混淆。