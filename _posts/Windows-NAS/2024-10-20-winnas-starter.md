---
title: Windows Nas Starter
date: 2024-10-21 09:00:00 +/+0800
#自定义文章描述，不显示文章自动生成的描述
description: Windows Nas 从入门到养老
categories:
  - winnas
tags:
  - winnas
  - 目录
---

# 系统选择
底层系统选择Windows Server 2022
## 系统安装
下载：
初始安装参考B站UP:HUGO驼驼视频。
[用windows server 2022安装自己的WINDOWS NAS_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1mr4y1k7cE/?spm_id_from=333.999.0.0)
## 系统激活
系统激活使用KMS方式，教程参看肥猫大佬网站。
[大客户VL版本Windows客户端加域自动激活详细教程](https://www.mr-mao.cn/archives/vl_windows_join_dc_auto_activation.html)
## 更改远程连接端口
Windows默认远程连接为3389，建议更改为高位端口。
# 下载器
## qbittorrent
[qbittorrent 官网](https://www.qbittorrent.org/)
配置
Windows多开qbittorrent方法
将qbittorrent.setup.exe安装程序解压，在解压后的文件夹内创建profile文件夹
将原qbittorrent配置文件夹下面全部文件复制到profile文件夹内，删除种子即可
![[Pasted image 20240415200847.png]]
![[Pasted image 20240415200826.png]]
## transmission
[Transmission 官网](https://transmissionbt.com/)
### 传统WEBUI[ronggang/transmission-web-control](https://github.com/ronggang/transmission-web-control)
### Remote GUI，暂无中文[openscopeproject/TrguiNG](https://github.com/openscopeproject/TrguiNG)
### jayzcoder/TrguiNG: Transmission WebUI [基于 openscopeproject/TrguiNG 汉化和改进 ](https://github.com/jayzcoder/TrguiNG)
# 媒体库
## Emby
[Emby 官网](https://emby.media/)
## Plex
[Plex 官网](https://www.plex.tv/)
## Jellyfin
[Jellyfin 官网](https://jellyfin.org/)
# 虚拟机VMWare Workstation
[虚拟机开机自启动、随宿主机开机自启](https://blog.csdn.net/Dontla/article/details/132762521)
[B站VMWare Workstation安装各类系统-大大鹅体验个人主页](https://space.bilibili.com/517246386)
## 黑群晖
[VMware安装群晖7.2NAS系统](https://www.bilibili.com/video/BV1SN4y1m7F4/?spm_id_from=333.999.0.0)
## Unraid
[Unraid 官网](https://unraid.net/)
[ VMware安装Unraid NAS系统](https://www.bilibili.com/video/BV1QQ4y1M7oG/?spm_id_from=333.999.0.0)
## iStoreOS
[iStoreOS 官网](https://www.istoreos.com/)
[VMware虚拟机安装软路由系统iStoreOS](https://www.cpolar.com/blog/vmware-virtual-machines-install-the-soft-routing-system-istoreos)
## 小雅Alist
[小雅Windows VMware系统成](https://p.kdocs.cn/s/7VXZW6IZABADA)
# PT工具
## IYUU
[IYUUPlus官网](https://www.iyuu.cn)
[IYUUDev](https://doc.iyuu.cn)
## Reseed Puppy
[Reseed Puppy Wiki](https://zxfsadly.gitee.io/reseed-puppy-wiki/)
## Cookie Cloud
[Cookie Cloud GitHub](https://github.com/easychen/CookieCloud)
## Movie Pilot
[Movie Pilot GitHub](https://github.com/jxxghp/MoviePilot)
## Vertex
[Vertex Wiki](https://wiki.vertex.icu/)
## QD签到
[QD签到 官网](https://qd-today.github.io/qd/zh_CN/)
# 远程连接方案
## DDNS-GO
[DDNS-GO GitHub](https://github.com/jeessy2/ddns-go)
## ZeroTier
[ZeroTier 官网](https://my.zerotier.com/)
## Tailscale
[Tailscale 官网](https://tailscale.com/)
## Lucky
[Lucky 官网](https://lucky666.cn/)

# Windows文件共享
## Alist搭建
1.桌面端安装
2.本地存储挂载
3.防火墙放行
4.使用lucky反代
## 笔记软件Obsidian
插件remotely save
## 同步方案
