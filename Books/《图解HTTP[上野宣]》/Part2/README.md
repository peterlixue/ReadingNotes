## 第2章 简单的HTTP协议



 1.请求报文是由请求方法、请求URI、协议版本、可选的请求首部字段和内容实体构成的。
 
 ---
 
 2.响应报文基本上由协议版本、状态码(表示请求成功或失败的数字代码)、用以解释状态码的原因短语、可选的响应首部字段以及实体主体构成。
 
 ---
  
 3.HTTP是一种不保存状态，即无状态协议。
 
 ---
  
 4.告知服务器意图的HTTP方法
 - GET:获取资源
 - POST:传输实体主体
 - PUT:传输文件
 - HEAD:获得报文首部
 - DELETE:删除文件
 - OPTIONS:询问支持的方法
 - TRACE:追踪路径
 - CONNECT:要求用隧道协议连接代理
  
 ---
 
 5.在HTTP/1.1中，所有的连接默认都是持久连接。
  
 ---
 
 6.持久连接使得多数请求以管线化(pipelining)方式发送成为可能。
