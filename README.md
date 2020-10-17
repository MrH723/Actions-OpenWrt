![GitHub Repo stars](https://img.shields.io/github/stars/MrH723/Actions-OpenWrt)
![GitHub forks](https://img.shields.io/github/forks/MrH723/Actions-OpenWrt?label=Fork)
![GitHub](https://img.shields.io/github/license/MrH723/Actions-OpenWrt)

openwrt-packages — OpenWrt第三方全家桶软件源
======================

脚本使用的第三方全家桶软件源
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

***---建议使用lean源码 [![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)***

***---不建议 Fork (因为你Fork 过去不会自动更新）***

***---国内常用OpenWrt软件包源码合集，每天两次自动更新***

***---packages 分支 供18.06 使用***

***---packages-19.07 分支 供19.07 使用***

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

|    序号   |     设备平台     |   编译状态及下载链接 |   源码   | 备注说明   |
| :-----------------: | :-------------: |:-----------------: | :-----------------: |  :-----------------: | 
| 1 |   [![](https://img.shields.io/badge/OpenWrt-x86_64_(64位)-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2864bit%29+OpenWrt%22)    | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20X86(64bit)%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2864bit%29+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |  |  
| 2 |    [![](https://img.shields.io/badge/OpenWrt-x86_(32位)-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2832bit%29+OpenWrt%22)     |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20X86(32bit)%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2832bit%29+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | | 
| 3 |        [![](https://img.shields.io/badge/OpenWrt-竞斗云-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+G-Dock+OpenWrt%22)         |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20G-Dock%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+G-Dock+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | | 
| 4 |        [![](https://img.shields.io/badge/OpenWrt-极路由_B70-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+HiWiFi+B70+OpenWrt%22)        |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20HiWiFi%20B70%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+HiWiFi+B70+OpenWrt%22)|[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | |
| 5 |        [![](https://img.shields.io/badge/OpenWrt-K2T-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K2T+OpenWrt%22)           | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20K2T%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K2T+OpenWrt%22)|[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | | 
| 6 |        [![](https://img.shields.io/badge/OpenWrt-K2P-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K2P+OpenWrt%22)           |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20K2P%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K2P+OpenWrt%22)|[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | | 
| 7 |       [![](https://img.shields.io/badge/OpenWrt-K3-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K3+OpenWrt%22)           |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20K3%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+K3+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  |  | 
| 8 |       [![](https://img.shields.io/badge/OpenWrt-N1_盒子-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+N1+OpenWrt%22)         |[![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20N1%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+N1+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  |Docker N1 | 
| 9 |    [![](https://img.shields.io/badge/OpenWrt-红米_AC2100-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Redmi+AC2100+OpenWrt%22)     | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Redmi%20AC2100%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Redmi+AC2100+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | | 
| 10 |    [![](https://img.shields.io/badge/OpenWrt-Newifi3_D2-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Newifi+D2+OpenWrt%22)      |  [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Newifi%20D2%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Newifi+D2+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | | 
| 11 |    [![](https://img.shields.io/badge/OpenWrt-树莓派_3B/3B+-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi3+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20RaspBerryPi3%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi3+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | 含 USB 网卡驱动 |
| 12 |    [![](https://img.shields.io/badge/OpenWrt-树莓派_4B-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22)    | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20RaspBerryPi4%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22)  |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | 含 USB 网卡驱动，自用 |
| 13 |     [![](https://img.shields.io/badge/OpenWrt-小娱_C5-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+XiaoYu+XY-C5+OpenWrt%22)        | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20XiaoYu%20XY-C5%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+XiaoYu+XY-C5+OpenWrt%22)   |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  |  |
| 14|      [![](https://img.shields.io/badge/OpenWrt-NanoPi_NEO2-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+NanoPi+NEO2+OpenWrt%22)     |  [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20NanoPi%20NEO2%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+NanoPi+NEO2+OpenWrt%22)  |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | ZIP 解压后刷写 |
| 15|      [![](https://img.shields.io/badge/OpenWrt-NanoPi_R2S-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+NanoPi+R2S+OpenWrt%22)     |  [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20NanoPi%20R2S%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+NanoPi+R2S+OpenWrt%22)  |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | ZIP 解压后刷写 |
| 16|     [![](https://img.shields.io/badge/OpenWrt-小米_R3G-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+R3G+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Mi%20R3G%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+R3G+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |
| 17|     [![](https://img.shields.io/badge/OpenWrt-小米_R3P-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+R3P+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Mi%20R3P%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+R3P+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |
| 18|     [![](https://img.shields.io/badge/OpenWrt-小米_Mini-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+Mini+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Mi%20Mini%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Mi+Mini+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |
| 19|     [![](https://img.shields.io/badge/OpenWrt-网件_R7800-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20Netgear%20R7800%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |
| 20|     [![](https://img.shields.io/badge/OpenWrt-星际宝盒_CM520-FFFFFF.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92+CM520+OpenWrt%22)   | [![](https://github.com/IvanSolis1989/OpenWrt-DIY/workflows/Build%20星际宝盒%20CM520%20OpenWrt/badge.svg)](https://github.com/IvanSolis1989/OpenWrt-DIY/actions?query=workflow%3A%22Build+%E6%98%9F%E9%99%85%E5%AE%9D%E7%9B%92+CM520+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |

## 鸣谢
 
[P3TERX 的 Action 源码](https://github.com/P3TERX/Actions-OpenWrt)

[Lean 的 OpenWrt 源码](https://github.com/coolsnowwolf/lede)

