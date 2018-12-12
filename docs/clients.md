
Configuring the openVPN client
=================
<i>Other language versions:</i> [English](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients.md), [中文](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md） <br>

After successfully building your own VPN server, follow the steps below to configure your device. openVPN is supported on Android, iOS, OS X and Windows without the need to install additional software. The setup process usually takes only a few minutes. If you are unable to connect, first check if you have the correct VPN login credentials.

-------------------------------------------------- --------
* Platform name<br>
    * [Windows](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md#windows)
    * [OS X (macOS)](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md#os-x)
    * [Android](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md#Android)
    * [iOS (iPhone/iPad)](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md#ios-iphoneipad)
    * [Linux](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients-zh.md#Linux)
* Troubleshooting <br>
    * [Connection failed](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients.md#connection-failed)
    * [Unable to access the network if the connection is successful](https://github.com/bindaolh/openvpn-install/blob/master/docs/clients.md#the-connection-succeeded-and-the-network-could-not-be-accessed)






Windows
==============

## Windows 10 and 8.x adn 7.x
1. Download the Windows client on Shangguan.com: [https://openvpn.net/index.php/open-source/downloads.html] (https://openvpn.net/index.php/open-source/downloads.html ) <br> or link: [https://pan.baidu.com/s/1_o3nZ2zL5y94WQ7-w7zLQw](https://pan.baidu.com/s/1_o3nZ2zL5y94WQ7-w7zLQw)
Extraction code: k0ck

2, the default installation, select easy-rsa, the installation path defaults to C:\Program Files\OpenVPN<br>

   <b>Note: When prompted with the TAP network adapter, be sure to install it at the same time. </b><br>

![When prompted this] (https://github.com/bindaolh/openvpn-install/blob/master/pic/1.png)

3. Move the client certificate file to C:\Program Files\OpenVPN\config

4. You must run OpenVPN as an administrator to run properly. There are two ways to do this:<br>
Option 1: Right-click on the OpenVPN desktop shortcut and select Run as administrator. This must be done each time you connect to a VPN.

Option 2: Configure shortcuts to run automatically with administrator privileges. This will apply to all users on the system. Right click on the OpenVPN GUI shortcut and select Properties. Go to the Compatibility tab and choose to change the settings for all users. Select Run this program as an administrator and click OK. <br>

5. When you launch the OpenVPN application, its icon will appear in the taskbar. Right click on it and select Connect. The OpenVPN taskbar icon will turn yellow and a dialog will appear showing the detailed output of the connection process. Upon successful connection, the icon will turn green and a confirmation bubble will appear indicating that the connection was successful. <br>

  ![icon turns green](https://github.com/bindaolh/openvpn-install/blob/master/pic/2.png)


## windows xp installation using openVPN client

1, download the client installation package
Download address (select the corresponding installation package according to your own system)
32-bit [http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-i686.exe] (http://swupdate.openvpn.org/community/releases/openvpn-install- 2.3.0-I005-i686.exe)
64-bit [http://swupdate.openvpn.org/community/releases/openvpn-install-2.3.0-I005-x86_64.exe] (http://swupdate.openvpn.org/community/releases/openvpn-install- 2.3.0-I005-x86_64.exe)

2, find the installed program
Right click --- attribute - compatibility, hook on two places, choose your own system<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/3.png)

3. Click on the installation package and proceed to the next step to install <br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/4.png)

4. After installation, a red computer icon appears in the lower right corner<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/5.png)

5. Move the client certificate file to C:\Program Files\OpenVPN\config

6, start the client program, there is a small red icon in the lower right of the taskbar, the dual machine can be started, the following interface appears after the connection is successful, the window automatically closes, the color of the right subscript becomes green <br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/6.png)<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/7.png)



## OS X

Since openvpn officially does not develop a client for mac os, it can only be developed by a third party. Tunnelblick is a free open source application that allows you to connect OS X and macOS to an OpenVPN server.<br>

1. Tunnelblick third-party software, completely free, and suitable for openvpn configuration.
Download address: [http://code.google.com/p/tunnelblick/wiki/DownloadsEntry?tm=2](http://code.google.com/p/tunnelblick/wiki/DownloadsEntry?tm=2)

2, install Tunnelblick
After the download is completed, it is a file in dmg format, open the file installation (as shown below)

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/7.1.png)

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/8.png)

3. Double-click the .ovpn file that was extracted from your file. (can choose according to your own needs)

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/9.png)

4. After the installation is complete, there is an ‘n’ icon in the upper right corner of the screen. Click on -> Connect, the connection is successful as shown below

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/10.png)<br>
![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/11.png)


## Android
The Android OpenVPN client has two main options. The first is OpenVPN Connect on Google Play, the official client of OpenVPN Technologies and the parent company behind OpenVPN. The second option is OpenVPN for Android on Google Play and F-droid. These two clients are similar, but OpenVPN for Android is open source, more feature-rich, and updated frequently, so let's take it. <br>
```Note If you have a gvfs-backends package installed on a Windows or Linux computer, you can connect to the device via USB and it will be displayed as an external USB device in the system's file manager. If you have a macOS device, you will need to install Android file transfer first. ```

1. Download and install the client software OpenVPN for Android<br>
[https://f-droid.org/packages/de.blinkt.openvpn](https://f-droid.org/packages/de.blinkt.openvpn/)

2. Copy the VPN client certificate from the local computer to the Android device. You can put them in the ../Internal storage/ folder in the directory.

3. Disconnect the device from the USB and start OpenVPN for Android. To import a VPN profile, click the Import icon in the top right corner.

![1](https://ask.qcloudimg.com/http-save/1206624/bihkd6xlnm.png?imageView2/2/w/1620)<br>
You will then see the file browser. Navigate to the folder you copied to the device in the previous step and click on the client.ovpn file to import it as a VPN profile.

![1](https://ask.qcloudimg.com/http-save/1206624/aljgxrgvta.png?imageView2/2/w/1620)<br>

4. On the Convert Profile screen, verify that the certificate and key file names are correct. Then click the checkmark symbol in the upper right corner of the screen to complete the import process.

![1](https://ask.qcloudimg.com/http-save/1206624/8sppyfpfeg.png?imageView2/2/w/1620)<br>

5. To connect to the VPN server, click on the configuration file you just created and confirm the connection request. The log screen will show the connection status, and soon after, Android will be connected. You can further customize the configuration file in the application's Settings tab. <br>

![1](https://ask.qcloudimg.com/http-save/1206624/679jtvy62n.png?imageView2/2/w/1620)<br>
![1](https://ask.qcloudimg.com/http-save/1206624/xu45twaemo.png?imageView2/2/w/1620)<br>
![1](https://ask.qcloudimg.com/http-save/1206624/3qzr226n8s.png?imageView2/2/w/1620)<br>
<b>Note: After importing the configuration file and confirming that everything is ok, back up the client certificate file to external storage and remove the key and certificate files from the device. Once imported, they will reside in the client's VPN profile and no longer need to be kept in their internal storage, which is readable by other applications. </b>


## iOS (iPhone/iPad)

OpenVPN Connect is used to manage Apple iOS OpenVPN connections for iPhone and iPad. We will use iTunes to transfer files from a computer running macOS or Windows to an iOS device. A Linux computer with the component gvfs-backends can install an iOS device as external storage.

```Note The following example uses iTunes 12 and OpenVPN Connect 1.0.5 to run on iOS 9.0.2 and macOS 10.10. ```

1. Make sure your iOS device is updated and install OpenVPN Connect from the iTunes App Store. <br>

![1](https://ask.qcloudimg.com/http-save/1206624/bu17f0m841.png?imageView2/2/w/1620)<br>

2. Connect your iOS device to a computer running macOS or Windows and open iTunes. <br>
3. Select the iPad or iPhone icon near the top left corner of the menu bar. <br>
Note If this is your first time connecting an iOS device to iTunes, you will need to click the overflow menu (three horizontal dots) and select “Apps”, then click “Start”.

![1](https://ask.qcloudimg.com/http-save/1206624/nuvq0mtqx5.png?imageView2/2/w/1620)<br>
4. In the left sidebar, select "Applications" and scroll down to the "File Sharing" category in the main window. You will see the OpenVPN Connect icon. Click it and then click Add in the OpenVPN Document box. Navigate to the ta.key file in the Finder and the .opvn file configured by the client, then drag them to the iTunes window. If you want to add them separately, add a key before the client profile or OpenVPN Connect can't find the key. <br>

![1](https://ask.qcloudimg.com/http-save/1206624/exxl4cmnkf.png?imageView2/2/w/1620)<br>
5. Open the OpenVPN Connect app on your iOS device. You will see an area indicating that you can import a new OpenVPN profile. Click on it to highlight the profile and click the green button to add it. <br>

![1](https://ask.qcloudimg.com/http-save/1206624/cc1v623ml7.png?imageView2/2/w/1620)<br>
6. On the next screen, click the “Connect” slider to connect to the VPN server.

![1](https://ask.qcloudimg.com/http-save/1206624/ip1rciq8h4.png?imageView2/2/w/1620)<br>
7. You will see a notification prompt asking you to allow OpenVPN to enable the connection. Choose yes. iOS will connect soon.

![1](https://ask.qcloudimg.com/http-save/1206624/4rjd1ex2sq.png?imageView2/2/w/1620)<br>
8. The OpenVPN Connect application settings can be used to further tweak the connection. For example, you can specify whether the VPN is connected via WiFi or cellular network or both. For a description of each option, see the OpenVPN Connect iOS FAQ (https://docs.openvpn.net/docs/openvpn-connect/openvpn-connect-ios-faq.html).

![1](https://ask.qcloudimg.com/http-save/1206624/kjtq2you47.png?imageView2/2/w/1620)<br>
Note: After importing the configuration file and verifying that it is working properly, back up the client credential file to external storage and remove the key and certificate files from the device. Once imported, they will reside in the client's VPN profile and no longer need to be kept in their internal storage, which is readable by other applications.


## Linux

### ubuntu

1. Install openvpn<br>
Sudo apt-get install openvpn

2. Configure openvpn<br>
First copy the configuration file client.ovpn provided by the OpenVPN server to /etc/openvpn/

3. Connect openvpn, the connection is successful as shown below <br>
Sudo openvpn /etc/openvpn/client.ovpn

![1](https://github.com/bindaolh/openvpn-install/blob/master/pic/12.png)<br>
4. Use aliases to optimize the command to open openvpn<br>
Edit the .bashrc file and add a line to the file as shown below.<br>
Sudo vim .bashrc<br>

Alias ​​vpn='sudo openvpn /etc/openvpn/client.ovpn' <br>

After saving, you can connect to openvpn directly by executing vpn. <br>

5. Force disconnection of the vpn connection with ctrl+c. <br>

The above command is not convenient in practice because it takes up a separate terminal. After the test is successful, you can connect to OpenVPN in the background using the following command:<br>
Vpn > /dev/null &

It is commendable that openvpn is very intelligent, and it will automatically reconnect if the connection is abnormally interrupted, the server cannot be connected, or the network is disconnected. Therefore, if you want to automatically connect to OpenVPN when you boot, or if VPN is online all the year round, you can add the above command line to <br>

/etc/rc.local

in. Note that the ampersand at the end of the command cannot be omitted, otherwise the normal startup of the system may be blocked.

### other Linux

Other versions of the Linux system are similar to Ubuntu, except that the installation commands are slightly different. Let's try it ourselves!


## Connection failed

1. Check that you are using administrator identity permissions? If not, please use admin rights!

2. Check if the imported configuration file is correct?

3. Check if the command you are running is correct?

## The connection succeeded and the network could not be accessed.

1, check the local firewall configuration

2, check the server-side firewall configuration


