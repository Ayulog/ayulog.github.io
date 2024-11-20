---
title: Windows NAS istoreos
date: 2024-11-20 09:00:00 +/+0800
#自定义文章描述，不显示文章自动生成的描述
description: Windows Nas 安装istoreos
categories:
  - winnas
tags:
  - winnas
  - hyper-v
---
使用`Hyper-V`安装`iStoreOS`作为旁路由，并进行相关设置

## 准备工作：
- 确保你的 Windows 系统支持`Hyper-V`，并且已经启用`Hyper-V`。
## 下载 OpenWrt 镜像：
- 从[iStoreOS官网地址](https://www.istoreos.com/)下载适用于`x86_64`的`img`镜像文件。
## 转换镜像：
- 使用工具（如[StarWind V2V Image Converter](https://www.starwindsoftware.com/starwind-v2v-converter)）将`img`文件转换为`VHDX`格式。
 - 选择从`local file`到`local file`，点击转换
## 创建虚拟机：
- 打开`Hyper-V 管理器`，选择`虚拟交换机管理器`，新建`外部虚拟交换机`，勾选`允许管理操作系统共享此网络配置`
- 选择“新建” -> “虚拟机”。
 - 输入虚拟机名称（如`iStoreOS`），选择`第一代虚拟机`。
 - 分配内存（`如1024MB`），选择使用现有虚拟硬盘（选择转换后的`VHDX`文件）。
 - 添加网络适配器，连接到你的主网络（选择新建的外部虚拟交换机），勾选`启用MAC地址欺骗`
## 启动并配置 iStoreOS：
- 启动虚拟机，连接到控制台。
- 进行基本网络配置，输入`vim /etc/config/network`进入网络编辑界面，英文输入法下按`i`进行编辑
 - 设置 LAN 口 IP 地址（如 192.168.10.1），避免与其他设备冲突。
 - 更改完成后按`Esc`退出编辑，输入`:wq`保存
## 配置旁路由：
- 浏览器输入更改好的`lan ip`，用户名`root`，密码`password`
- 在 iStoreOS 的 Web 管理界面中，配置防火墙和 NAT 设置，使其作为旁路由工作。
- 确保主路由器将流量转发到 iStoreOS 旁路由。

## 参考
- [Hyper-V安装OpenWrt虚拟机(以iStoreOS为例)](https://www.bilibili.com/video/BV1Bh4y1i7th/?spm_id_from=333.337.search-card.all.click)
