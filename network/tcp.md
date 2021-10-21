### TCP 



三次握手
<img src="1.jpg" />


TCP服务器进程先创建传输控制块TCB，时刻准备接受客户进程的连接请求 LISTEN状态


TCP客户进程先创建传输控制块TCB，向服务器发送连接请求报文，同步位SYN=1，同时选择一个初始序列号seq=x TCP客户端进入SYN-SENT 同步已发送状态



TCP服务器接收到连接请求报文，如果同意连接，则发出确认报文 ACK=1 SYN=1 ，确认号为 ack=x+1,初始化一个seq=y，服务器进入SYN-RECV 同步收到状态

TCP客户端收到连接确认报文，确认报文的ACK=1，ack=y+1 seq=x+1,客户端连接建立，进入ESTABLISHED连接已建立状态

TCP服务端收到确认报文 进入ESTABLISHED 连接已建立状态



四次挥手

<img src="2.jpg" />
