### 一 漏洞描述
NFS（Network File System）即网络文件系统，它允许网络中的计算机之间通过TCP/IP网络共享资源。在NFS的应用中，本地NFS的客户端应用可以透明地读写位于远端NFS服务器上的文件，就像访问本地文件一样。若运维人员未对文件访问进行控制，将导致本地文件可被任意读取。

### 二 漏洞利用
利用 mount -t nfs ip:/home/username 挂载。

### 三 漏洞修复
1 限制文件夹权限  
2 iptables限制  
3 Kerberos V5
