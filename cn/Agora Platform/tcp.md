
---
title: TCP
description: Definition of TCP
platform: All Platforms
updatedAt: Wed Sep 30 2020 08:53:08 GMT+0800 (CST)
---
# TCP
TCP（Transmission Control Protocol），即传输控制协议，是一种面向连接的、可靠的传输层通信协议。

面向连接是指在传输数据之前必须先在发送端和接收端之间建立连接。TCP 通过三次握手的方式建立连接：

- 第一次握手：发送端向接收端发送连接请求。
- 第二次握手：接收端同意连接，向发送端发送应答。
- 第三次握手：发送端收到应答，向接收端发送确认信息。

如果发出连接请求后，发送端没有收到接收端的回复，那么发送端就会持续发送请求，而不会直接传输数据。

为了保证传输的可靠性，TCP 会给每个数据包一个序号，接收端成功收到数据包后会发回一个相应的确认（ACK），如果在一定的往返时延后发送端没有收到确认，数据包会被重传。

TCP 只支持一对一的传输，不支持一对多或者多对多的数据传输。

TCP 可以用于对传输数据的完整性要求较高、对实时性要求不高的场景，比如文件传输。Agora 实时消息服务使用的主要是 TCP 协议。

<div class="alert info">相关链接：
	<li><a href="../../cn/Agora%20Platform/udp.md">UDP</a></li>
	<li><a href="https://www.bilibili.com/video/BV1ET4y1u7Pq">你知道吗？每次上网，都是一场大型协议互签会</a></li>
</div>

<a href="../../cn/Agora%20Platform/terms.md"><button>返回术语库</button></a>