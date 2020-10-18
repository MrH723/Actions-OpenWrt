![GitHub Repo stars](https://img.shields.io/github/stars/MrH723/Actions-OpenWrt)
![GitHub forks](https://img.shields.io/github/forks/MrH723/Actions-OpenWrt?label=Fork)
![GitHub](https://img.shields.io/github/license/MrH723/Actions-OpenWrt)

第一部分
======================

openwrt-packages — OpenWrt第三方全家桶软件源
======================

--编译脚本使用的第三方全家桶软件源
-------------

```bash
https://github.com/MrH723/openwrt-packages
```

--第三方全家桶软件源更新状态
-------------

- ![Update packages](https://github.com/MrH723/openwrt-packages_action/workflows/Update%20packages/badge.svg)

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

Actions-OpenWrt — 多设备固件自动云编译
======================

-- 支持的设备平台以及固件下载地址
-------------

|    序号   |     平台-设备名称     |   编译状态+下载链接 |  
| :-----------------: | :-------------: |:-----------------: | 
| 1 |   [![](https://img.shields.io/badge/OpenWrt-x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80%E7%89%88-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80.yml)    | [![x86多拨极简.yml](https://github.com/MrH723/Actions-OpenWrt/workflows/x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80.yml/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80.yml) |
| 2 |   [![](https://img.shields.io/badge/OpenWrt-x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80%E7%89%88-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80.yml)    | [![x86旁路由极简.yml](https://github.com/MrH723/Actions-OpenWrt/workflows/x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80.yml/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3Ax86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80.yml) |
| 3 |   [![](https://img.shields.io/badge/OpenWrt-%E5%B0%8F%E5%A8%B1%20C5-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+XiaoYu+XY-C5+OpenWrt%22)    | [![Build XiaoYu XY-C5 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20XiaoYu%20XY-C5%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+XiaoYu+XY-C5+OpenWrt%22) |
| 4 |   [![](https://img.shields.io/badge/OpenWrt-%E6%A0%91%E8%8E%93%E6%B4%BE%203B%2F3B%2B-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+RaspBerryPi3+OpenWrt%22)    | [![Build RaspBerryPi3 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20RaspBerryPi3%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+RaspBerryPi3+OpenWrt%22) |
| 5 |   [![](https://img.shields.io/badge/OpenWrt-%E7%BA%A2%E7%B1%B3%20AC2100-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Redmi+AC2100+OpenWrt%22)    | [![Build Redmi AC2100 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Redmi%20AC2100%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Redmi+AC2100+OpenWrt%22) |
| 6 |   [![](https://img.shields.io/badge/OpenWrt-%E6%A0%91%E8%8E%93%E6%B4%BE%204B-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22)    | [![Build RaspBerryPi4 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20RaspBerryPi4%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22) |
| 7 |   [![](https://img.shields.io/badge/OpenWrt-%E7%BD%91%E4%BB%B6%20R7800-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22)    | [![Build Netgear R7800 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Netgear%20R7800%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22) |
| 8 |   [![](https://img.shields.io/badge/OpenWrt-%E5%B0%8F%E7%B1%B3%20R3G-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+R3G+OpenWrt%22)    | [![Build Mi R3G OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Mi%20R3G%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+R3G+OpenWrt%22) |
| 9 |   [![](https://img.shields.io/badge/OpenWrt-NanoPi%20R2S-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+NanoPi+R2S+OpenWrt%22)    | [![Build NanoPi R2S OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20NanoPi%20R2S%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+NanoPi+R2S+OpenWrt%22) |
| 10 |   [![](https://img.shields.io/badge/OpenWrt-Newwifi3%20D2-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Newifi+D2+OpenWrt%22)    | [![Build Newifi D2 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Newifi%20D2%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Newifi+D2+OpenWrt%22) |
| 11 |   [![](https://img.shields.io/badge/OpenWrt-NanoPi%20NEO2-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+NanoPi+NEO2+OpenWrt%22)    | [![Build NanoPi NEO2 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20NanoPi%20NEO2%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+NanoPi+NEO2+OpenWrt%22) |
| 12 |   [![](https://img.shields.io/badge/OpenWrt-%E5%B0%8F%E7%B1%B3%20R3P-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+R3P+OpenWrt%22)    | [![Build Mi R3P OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Mi%20R3P%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+R3P+OpenWrt%22) |
| 13 |   [![](https://img.shields.io/badge/OpenWrt-K3-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K3+OpenWrt%22)    | [![Build K3 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20K3%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K3+OpenWrt%22) |
| 14 |   [![](https://img.shields.io/badge/OpenWrt-K2T-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K2T+OpenWrt%22)    | [![Build K2T OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20K2T%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K2T+OpenWrt%22) |
| 15 |   [![](https://img.shields.io/badge/OpenWrt-K2P-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K2P+OpenWrt%22)    | [![Build K2P OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20K2P%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+K2P+OpenWrt%22) |
| 16 |   [![](https://img.shields.io/badge/OpenWrt-%E7%AB%9F%E6%96%97%E4%BA%91-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+G-Dock+OpenWrt%22)    | [![Build G-Dock OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20G-Dock%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+G-Dock+OpenWrt%22) |
| 17 |   [![](https://img.shields.io/badge/OpenWrt-N1%20%E7%9B%92%E5%AD%90-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+N1+OpenWrt%22)    | [![Build N1 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20N1%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+N1+OpenWrt%22) |
| 18 |   [![](https://img.shields.io/badge/OpenWrt-%E5%B0%8F%E7%B1%B3%20Mini-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+Mini+OpenWrt%22)    | [![Build Mi Mini OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Mi%20Mini%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Mi+Mini+OpenWrt%22) |
| 19 |   [![](https://img.shields.io/badge/OpenWrt-%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92%20CM520-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92+CM520+OpenWrt%22)    | [![Build 星际宝盒 CM520 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92%20CM520%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92+CM520+OpenWrt%22) |
| 20 |   [![](https://img.shields.io/badge/OpenWrt-%E6%9E%81%E8%B7%AF%E7%94%B1%20B70-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+HiWiFi+B70+OpenWrt%22)    | [![Build HiWiFi B70 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20HiWiFi%20B70%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+HiWiFi+B70+OpenWrt%22) |

-- 关于自动编译固件的说明
-------------

- 不建议Fork，按需下载即可。
- 自动编译，自动拉取最新版本插件。
- x86多拨极简版为自用固件仅包含 （pw,S,上网时间控制，upnp,ddns,去广告，多拨，负载均衡，流量监控，主题只加入了默认主题以及自己比较喜欢的edge主题）
- x86旁路由极简版为自用，建议配合爱快使用，仅包含（pw，S，去广告，主题只加入了默认主题以及自己比较喜欢的edge主题）
- x86全家桶固件正在处理中，由于部分插件冲突需要些时间排雷。

## 鸣谢
 
[P3TERX 的 Action 源码] [![](https://img.shields.io/badge/P3TERX-源码-orange.svg)](https://github.com/P3TERX/Actions-OpenWrt)

[Lean 的 OpenWrt 源码] [![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)

## 特别鸣谢
[Lienol] [![](https://img.shields.io/badge/Lienol-%E6%BA%90%E7%A0%81-orange.svg)](https://github.com/Lienol)

[Kenzok8] [![](https://img.shields.io/badge/Kenzok8-%E6%BA%90%E7%A0%81-orange.svg)](https://github.com/kenzok8)

***由于本人小白，有可能使用到了大神的代码，没有放进鸣谢名单里的，请联系添加，再次感谢各位大神的贡献***



##### Table of Contents  
[Headers](#headers)  
[Emphasis](#emphasis)  
...snip...    
<a name="headers"/>
## Headers
