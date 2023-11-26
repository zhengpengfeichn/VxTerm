# VxTerm
github无法正常更新，最新版本请访问：
[[http://](https://blog.forbs.cn/post/111.html)](https://blog.forbs.cn/post/111.html)

#### 介绍
VxTerm，Telnet、SSH、MUD远程终端仿真工具

VxTerm现在集以下特点于一身：

-   1、内置触发器，可以根据屏幕和收到的信息内容触发指定的脚本
-   2、内置VxMatScript脚本，可以不需要在您的工作环境中再安装配置各种第三方的运行环境！
-   3、无依赖、单文件、纯绿色，无需安装，就一个文件就可以运行
-   4、多线程、多窗口、多会话
-   5、国产的！免费的！无任何功能限制！不需要注册！不需要破解！
-   6、Telnet、SSH、SFTP、Serial、以后可能会增加更多的协议
-   支持中文命令！ 

VxTerm是目前唯一一个可以以一个文件的方式助您完成全自动化运维的超级工具！

内置几个用于自动登录的触发器脚本：

```
（1）提示行为Login:或UserName:时自动发送已保存的用户名
    触发字符串 = "\\S*[Ll][Oo][Gg][Ii][Nn]:\\s*$|\\S*[Uu][Ss][Ee][Rr][Nn][Aa][Mm][Ee]:\\s*$"; // L"username[:]{0,1}[ ]*$"
    发送字符串 = "Sendln [$username]";

（2）提示行为Password:时自动发送已保存的密码，同时关闭登录触发器
    触发字符串 = "\\S*[Pp][Aa][Ss][Ss][Ww][Oo][Rr][Dd]:\\s*$";
    发送字符串 = "Sendln [$password]\nTrig- 登录";

（3）在连接端口成功后开始计时，如果超过3秒钟就关闭登录触发器
    触发字符串 = "^Connected$";
    发送字符串 = "Trig+ 登录\nwait 3000\nTrig- 登录";
```


#### 安装教程
不需要安装，就一个运行文件，直接点击运行即可。
