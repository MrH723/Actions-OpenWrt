![GitHub Repo stars](https://img.shields.io/github/stars/MrH723/Actions-OpenWrt)
![GitHub forks](https://img.shields.io/github/forks/MrH723/Actions-OpenWrt?label=Fork)
![GitHub](https://img.shields.io/github/license/MrH723/Actions-OpenWrt)

第一部分
======================

openwrt-packages — OpenWrt第三方全家桶软件源
======================

编译脚本使用的第三方全家桶软件源
-------------

```bash
https://github.com/MrH723/openwrt-packages
```

第三方全家桶软件源更新状态
-------------

![Update packages](https://github.com/MrH723/openwrt-packages_action/workflows/Update%20packages/badge.svg)

-- 关于更新状态的说明
-------------

- ![](https://img.shields.io/badge/Update%20packages-failing-red.svg) 所有上游源码无更新,本软件仓库所有软件均为最新版。
- ![](https://img.shields.io/badge/Update%20packages-passing-green.svg) 上游源码有更新，且已经全部更新到本软件源当中，本软件仓库所有软件均为最新版。
- 总之无论什么时候都是最新的。




-- 关于本软件源的使用方法
-------------

- 建议使用lean源码 [![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)

- 不建议 Fork (因为你Fork 过去不会自动更新）

- 国内常用OpenWrt软件包源码合集，每天两次自动更新

- packages 分支 供18.06 使用

- packages-19.07 分支 供19.07 使用

- 我只是个小白搬运工，不保证所有插件都能使用，各位可以自行尝试。



1. 先cd进package目录，然后执行
```bash
 git clone https://github.com/MrH723/openwrt-packages
```
2. 或者添加下面代码到feeds.conf.default文件
```bash
 src-git MrH723_packages https://github.com/MrH723/openwrt-packages
```
3. 先cd进package目录，然后执行
```bash
 svn co https://github.com/MrH723/openwrt-packages/branches/packages
```

第二部分
======================

Actions-OpenWrt — 多设备固件云编译
======================

|    序号   |     设备平台     |   编译状态及下载链接 |  
| :-----------------: | :-------------: |:-----------------: | 
| 1 |   [![](https://img.shields.io/badge/OpenWrt-x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80.yml)    | [![](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80.yml) |


## 鸣谢
 
[P3TERX 的 Action 源码] [![](https://img.shields.io/badge/P3TERX-源码-orange.svg)](https://github.com/P3TERX/Actions-OpenWrt)

[Lean 的 OpenWrt 源码] [![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)

