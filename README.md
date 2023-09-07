## 实现功能

项目分为两个端，WeChatRobot和WeChatHelper。WeChatRobot作为客户端负责和服务端进行通信，将服务端传回的数据显示到界面。WeChatHelper作为服务端，注入到微信进程，进行取数据和HOOK的相关操作，并且将取回的数据发回给客户端。

客户端和服务端之间采用WM_COPYDATA的方式进行进程通讯，互相传输数据

## 技术细节

PCXX逆向：使用CE+OD查找个人数据：https://blog.csdn.net/qq_38474570/article/details/92571302

PCXX逆向：使用HOOK拦截二维码：https://blog.csdn.net/qq_38474570/article/details/92798577

PCXX逆向：发送与接收消息的分析与代码实现：https://blog.csdn.net/qq_38474570/article/details/93339861

PCXX逆向：使用HOOK获取好友列表和群列表：https://blog.csdn.net/qq_38474570/article/details/95889507

PC微信逆向：两种姿势教你解密数据库文件：https://blog.csdn.net/qq_38474570/article/details/96606530
