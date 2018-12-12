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
1、上官网下载Windows客户端：[https://openvpn.net/index.php/open-source/downloads.html](https://openvpn.net/index.php/open-source/downloads.html)<br>或者链接：[https://pan.baidu.com/s/1_o3nZ2zL5y94WQ7-w7zLQw](https://pan.baidu.com/s/1_o3nZ2zL5y94WQ7-w7zLQw)
提取码：k0ck 

2、默认安装，选择easy-rsa，安装路径默认为C:\Program Files\OpenVPN<br> 

   <b>注意：当系统提示有关TAP网络适配器时，请务必同时安装它。</b><br>

![提示这个的时候](https://github.com/bindaolh/openvpn-install/blob/master/pic/1.png)

3、将客户端证书文件移动到C:\Program Files\OpenVPN\config

4、必须以管理员身份运行OpenVPN才能正常运行。有两种方法可以做到这一点：<br>
选项1：右键单击OpenVPN桌面快捷方式，然后选择以管理员身份运行。每次连接到VPN时都必须执行此操作。

选项2：配置快捷方式以使用管理员权限自动运行。这将适用于系统上的所有用户。右键单击OpenVPN GUI快捷方式，选择“ 属性”。转至兼容性选项卡，选择对所有用户更改设置。选择以管理员身份运行此程序，然后单击确定。<br>

5、当您启动OpenVPN应用程序时，其图标将显示在任务栏中。右键单击它并选择“ 连接”。OpenVPN任务栏图标将变为黄色，将出现一个对话框，显示连接过程的详细输出。成功连接后，图标将变为绿色并显示一个确认气泡,表示连接成功。<br>

  ![图标变为绿色](https://github.com/bindaolh/openvpn-install/blob/master/pic/2.png)


## windows xp 安装使用openVPN 客户端

1、下载客户端安装包
下载地址（根据自己的系统选择对应的安装包）
32位 [http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-i686.exe](http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-i686.exe)
64位 [http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-x86_64.exe](http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-x86_64.exe)

2、找到安装的程序
右击---属性-兼容性，两个地方钩上，选择自己的系统<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/3.png)

3、点击安装包，下一步下一步进行安装<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/4.png)

4、安装完毕，在右下角出现一个红色电脑图标<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/5.png)

5、将客户端证书文件移动到C:\Program Files\OpenVPN\config

6、启动客户端程序，在任务栏的右下方有个红色小图标，双机就可以启动了，连接成功后出现下面界面,窗口自动关闭，右下标的颜色变成绿色<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/6.png)<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/7.png)



## macOS版

由于openvpn官方没有开发适用于mac os 的客户端，所以只能用第三方开发的。Tunnelblick是一个免费的开源应用程序，可让您将OS X和macOS连接到OpenVPN服务器.<br>

1、Tunnelblick 第三方软件，完全免费，并且适用于openvpn的配置。
下载地址：[http://code.google.com/p/tunnelblick/wiki/DownloadsEntry?tm=2](http://code.google.com/p/tunnelblick/wiki/DownloadsEntry?tm=2)

2、安装Tunnelblick
下载完成之后是一个dmg格式的文件，打开文件安装（如下图）

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/7.1.png)

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/8.png)

3、双击给你的文件中解压出来的 .ovpn 文件。（可根据你自己需要选择）

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/9.png)

4、安装完成后，在屏幕右上角有一个‘n’型图标。点开->连接，连接成功如下图显示

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/10.png)<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/11.png)


## Android版
Android OpenVPN客户端有两个主选项。第一个是在 Google Play上的OpenVPN Connect，它是OpenVPN技术公司的官方客户，也是OpenVPN背后的母公司。第二个选项则是Google Play和F-droid上的OpenVPN for Android。这两个客户端是类似的，但OpenVPN for Android是开源的，功能更丰富，并且经常更新，所以我们将它。<br>
```注意 如果您有Windows计算机或是Linux计算机安装了gvfs-backends的软件包，则可以通过USB连接该设备，它将作为外部USB设备显示在系统的文件管理器中。如果您有macOS设备，则需要先安装Android文件传输。```

1、下载安装客户端软件OpenVPN for Android<br>
[https://f-droid.org/packages/de.blinkt.openvpn](https://f-droid.org/packages/de.blinkt.openvpn/)

2、将VPN客户端证书从本地计算机复制到Android设备。您可以将它们放入目录中的../Internal storage/的文件夹中。

3、断开设备与USB的连接并启动OpenVPN for Android。要导入VPN配置文件，请点击右上角的“导入”图标。

![1](https://ask.qcloudimg.com/http-save/1206624/bihkd6xlnm.png?imageView2/2/w/1620)<br>
然后，您将看到文件浏览器。导航到您在上一步中复制到设备的文件夹，然后点击该client.ovpn文件将其作为VPN配置文件导入。

![1](https://ask.qcloudimg.com/http-save/1206624/aljgxrgvta.png?imageView2/2/w/1620)<br>

4、在“ 转换配置文件”屏幕上，验证证书和密钥文件名是否正确。然后点击屏幕右上角的对勾符号以完成导入过程。

![1](https://ask.qcloudimg.com/http-save/1206624/8sppyfpfeg.png?imageView2/2/w/1620)<br>

5、要连接到VPN服务器，请点击刚刚创建的配置文件并确认连接请求。日志屏幕将显示连接状态，不久之后，Android将被连接。您可以在应用程序的“设置”选项卡中进一步自定义配置文件。<br>

![1](https://ask.qcloudimg.com/http-save/1206624/679jtvy62n.png?imageView2/2/w/1620)<br>
![1](https://ask.qcloudimg.com/http-save/1206624/xu45twaemo.png?imageView2/2/w/1620)<br>
![1](https://ask.qcloudimg.com/http-save/1206624/3qzr226n8s.png?imageView2/2/w/1620)<br>
<b>注：导入配置文件并确认一切正常后，将客户端证书文件备份到外部存储，并从设备中删除密钥和证书文件。导入后，它们将驻留在客户端的VPN配置文件中，不再需要保留在其内部存储中，这是其他应用程序可读取的。</b>


## iOS版

OpenVPN Connect 用于管理Apple iOS用于iPhone和iPad的OpenVPN连接。我们将使用iTunes将文件从运行macOS或Windows的计算机中传输到iOS设备。带有组件gvfs-backends的Linux计算机可以将iOS设备安装为外部存储。

```注意 以下示例使用 iTunes 12 和OpenVPN Connect 1.0.5在 iOS 9.0.2和macOS 10.10上运行。```

1、确保您的iOS设备已更新完成，然后从iTunes App Store 安装OpenVPN Connect。<br>

![1](https://ask.qcloudimg.com/http-save/1206624/bu17f0m841.png?imageView2/2/w/1620)<br>

2、将iOS设备连接到运行macOS或Windows系统的计算机，打开iTunes。<br>
3、选择菜单栏左上角附近的iPad或iPhone图标。<br>
注意 如果这是您第一次将iOS设备连接到iTunes，则需要单击溢出菜单（三个水平点）并选择“ 应用程序”，然后单击“开始”。

![1](https://ask.qcloudimg.com/http-save/1206624/nuvq0mtqx5.png?imageView2/2/w/1620)<br>
4、在左侧边栏中，选择“ 应用程序”并向下滚动到主窗口中的“ 文件共享”类别。您将看到OpenVPN Connect的图标。单击它，然后单击“ OpenVPN文档”框中的“ 添加 ”。导航到Finder中的ta.key文件和客户端配置的.opvn文件，然后将它们拖到iTunes窗口中。如果您要单独添加它们，请在客户端配置文件或OpenVPN Connect无法找到密钥之前添加密钥。<br>

![1](https://ask.qcloudimg.com/http-save/1206624/exxl4cmnkf.png?imageView2/2/w/1620)<br>
5、在iOS设备上打开OpenVPN Connect应用程序。您将看到一个区域表示可以导入新的OpenVPN配置文件。点击它以突出显示配置文件，然后点击绿色按钮添加它。<br>

![1](https://ask.qcloudimg.com/http-save/1206624/cc1v623ml7.png?imageView2/2/w/1620)<br>
6、在下一个屏幕画面中，点击“ 连接”滑块以连接到VPN服务器。

![1](https://ask.qcloudimg.com/http-save/1206624/ip1rciq8h4.png?imageView2/2/w/1620)<br>
7、您将看到一个通知提示，要求允许OpenVPN启用连接。选择是。iOS将在不久之后连接。

![1](https://ask.qcloudimg.com/http-save/1206624/4rjd1ex2sq.png?imageView2/2/w/1620)<br>
8、OpenVPN Connect的应用程序设置可用于进一步调整连接。例如，您可以指定VPN是通过WiFi或是蜂窝网络连接还是两者使用。有关每个选项的说明，[请参阅OpenVPN Connect iOS常见问题解答](https://docs.openvpn.net/docs/openvpn-connect/openvpn-connect-ios-faq.html)。

![1](https://ask.qcloudimg.com/http-save/1206624/kjtq2you47.png?imageView2/2/w/1620)<br>
注：导入配置文件并确认其工作正常后，将客户端凭据文件备份到外部存储，并从设备中删除密钥和证书文件。导入后，它们将驻留在客户端的VPN配置文件中，不再需要保留在其内部存储中，这是其他应用程序可以读取的。


## Linux

### ubuntu

1.安装openvpn<br>
sudo apt-get install openvpn
2.配置openvpn<br>
首先将OpenVPN服务器提供的配置文件client.ovpn复制到 /etc/openvpn/中

3.连接openvpn<br>
sudo openvpn /etc/openvpn/client.ovpn
4.用别名来优化开启openvpn的命令<br>
编辑.bashrc文件，在文件中如下图后边加入一行

 
sudo vim .bashrc

alias vpn='sudo openvpn /etc/openvpn/client.ovpn' (插入之文件）
保存后，执行 vpn  就可以直接连接openvpn。
5.用ctrl+c强制断开vpn连接。
上面的命令在实际中并不方便，因为它要占用一个独立的终端。在测试成功后，使用以下命令即可在后台连接OpenVPN：
openvpn /etc/openvpn/client.ovpn > /dev/null &
值得称赞的是，openvpn非常智能，在连接异常中断、无法连接服务器、断网的情况下，它会自动重连。因此，如果希望开机即自动连接OpenVPN，或者是VPN常年在线，则可将上述命令行加入
/etc/rc.local
中。注意，命令末尾的&符号不能省略，否则将可能阻塞系统的正常启动。
