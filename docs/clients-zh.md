配置 openVPN 客户端
=================
<i>其他语言版本:</i> [English](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients.md), [简体中文](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md). <br>

在成功搭建自己的 VPN 服务器之后，按照下面的步骤来配置你的设备。openVPN 在 Android, iOS, OS X 和 Windows 上均受支持，无需安装额外的软件。设置过程通常只需要几分钟。如果无法连接,请首先检查是否倒入了正确的 VPN 登录凭证。

----------------------------------------------------------
* 平台名称<br>
  * Windows
  * OS X (macOS)
  * Android
  * iOS (iPhone/iPad)
  * Linux
* 故障排除<br>








Windows
==============

## Windows 10 and 8.x adn 7.x
1、上官网下载Windows客户端：[https://openvpn.net/index.php/open-source/downloads.html](https://openvpn.net/index.php/open-source/downloads.html)<br>

2、默认安装，选择easy-rsa，安装路径默认为C:\Program Files\OpenVPN<br> 

   <b>注意：当系统提示有关TAP网络适配器时，请务必同时安装它。</b><br>

![提示这个的时候](https://github.com/bindaolh/openvpn-install/blob/master/pic/1.png)

3、将客户端证书文件移动到C:\Program Files\OpenVPN\config

4、必须以管理员身份运行OpenVPN才能正常运行。有两种方法可以做到这一点：<br>
选项1：右键单击OpenVPN桌面快捷方式，然后选择以管理员身份运行。每次连接到VPN时都必须执行此操作。

选项2：配置快捷方式以使用管理员权限自动运行。这将适用于系统上的所有用户。右键单击OpenVPN GUI快捷方式，选择“ 属性”。转至兼容性选项卡，选择对所有用户更改设置。选择以管理员身份运行此程序，然后单击确定。<br>

5、当您启动OpenVPN应用程序时，其图标将显示在任务栏中。右键单击它并选择“ 连接”。OpenVPN任务栏图标将变为黄色，将出现一个对话框，显示连接过程的详细输出。成功连接后，图标将变为绿色并显示一个确认气泡<br>

  [图标变为绿色](https://github.com/bindaolh/openvpn-install/blob/master/pic/2.png)


