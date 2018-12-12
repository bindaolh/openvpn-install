openVPN 服务器一键安装脚本
=================
使用 Linux 脚本一键快速搭建自己的 openVPN 服务器。OpenSSL加密库中的SSLv3/TLSv1协议函数库，可用于 Ubuntu/Debian/CentOS 系统。你只需提供自己的 VPN 登录证书凭证，然后运行脚本自动完成安装。<br>

openVPN 可以加密你的网络流量，以防止在通过因特网传送时，你和 VPN 服务器之间的任何人对你的数据的未经授权的访问。在使用不安全的网络时，这是特别有用的，例如在咖啡厅，机场或旅馆房间。<br>

» 另见： Docker 上的 openVPN 服务器   即将完成<br>

<i>其他语言版本:</i> [English](https://github.com/bindaolh/openvpn-install/edit/master/README.md), [简体中文](https://github.com/bindaolh/openvpn-install/edit/master/README-zh.md). <br>

## 目录
  * 快速开始
  * 功能特性
  * 系统要求
  * 安装说明
  * 下一步
  * 重要提示
  * 问题和反馈
  * 卸载说明
  * 另见

## 快速开始

首先，在你的 Linux 服务器* 上全新安装一个 Ubuntu LTS, Debian 或者 CentOS 系统。

使用以下命令快速搭建 openVPN 服务器：<br>
```curl -O https://raw.githubusercontent.com/bindaolh/openvpn-install/setup.sh
chmod +x setup.sh.sh```
