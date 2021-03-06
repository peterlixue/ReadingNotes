第7章 确保Web安全的HTTPS

---

1.http的缺点

- 通信使用明文(不加密)，内容可能会被窃听

- 不验证通信方身份，因此有可能遭遇伪装

- 无法证明报文的完整性，所以有可能已遭篡改

---

2.通信使用明文可能会被窃听

由于HTTP本身不具备加密的功能，所以无法做到对通信整体进行加密。

---

3.TCP/IP是可能被窃听的网络

按TCP/IP协议族的工作机制，通信内容在所有的通信线路上都有可能遭到窥视。

---

4.加密处理防止被窃听

- 通信的加密

HTTP协议中没有加密机制，但可以通过和SSL(Secure Socket Layer,安全套接层)或TLS(Transport Layer Security,安全层传输协议)的组合使用，加密HTTP的通信内容。



- 内容的加密

把HTTP报文里所含的内容进行加密处理。

由于不同于SSL或TLS将整个通信线路加密处理，所以内容仍有被篡改的风险。

---

5.不验证通信方的身份就可能遭遇伪装

HTTP协议中的请求和响应不会对通信方进行确认

---

6.任何人都可能发起请求

隐患：

- 无法确定是否是伪装的Web服务器

- 无法确定是否是伪装的客户端

- 无法确定正在通信的对方是否具备访问权限

- 无法判定请求是来自何方、出自谁手

- 即使是无意义的请求也会照单全收。无法阻止海量请求下的DoS攻击(Denial of Service,拒绝服务攻击)

---

7.查明对手的证书

只要能够确认通信方(服务器或客户端)持有的证书，即可判断通信方的真实意图。

---

8.无法证明报文完整性，可能已遭篡改

若无法证明信息完整性，也就意味着无法判断信息是否准确

---

9.接收到的内容可能有误

请求或响应在传输途中，遭攻击者拦截并篡改内容的攻击称为中间人攻击(Man-in-the-Middle attack,MITM)

---

10.如何防止篡改

常用的是MD5和SHA-1等散列值校验的方法

---

11.HTTP+加密+认证+完整性保护 = HTTPS

---

12.HTTPS是身披SSL外壳的HTTP

HTTPS并非是应用层的一种新协议。只是HTTP通信接口部分用SSL和TLS协议代替而已

---

13.SSL采用一种公开密钥加密的加密处理方式

---

14.HTTPS采用共享密钥加密和公开密钥加密两者并用的混合加密机制。

---

15.公开密钥加密方式存在一些问题，就是无法证明公开密钥本身就是货真价实的公开密钥。

为了解决这个问题，可以使用由数字证书认证机构(CA,Certificate Authority)和其相关相关颁发的公开密钥证书。

---

16.可证明组织真实性的EV SSL证书

EV SSL证书是基于国际标准的认证指导方针颁发的证书。

---

17.由自认证机构颁发的证书称为自签名证书

在互联网上不可作为证书使用。

---

18.HTTPS也存在一些问题，当使用SSL时，处理速度会变慢。

-通信慢

-处理慢(大量消耗CPU及内存等资源)

---

2017.9.16 8:26:45~2017.9.16 9:25:15

