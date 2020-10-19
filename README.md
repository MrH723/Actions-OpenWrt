![GitHub Repo stars](https://img.shields.io/github/stars/MrH723/Actions-OpenWrt?color=Blue&label=Stars&style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/MrH723/Actions-OpenWrt?color=Blue&label=Fork&style=for-the-badge)
![GitHub](https://img.shields.io/github/license/MrH723/Actions-OpenWrt?color=Blue&style=for-the-badge)

+ [![](https://img.shields.io/badge/-目录-blue.svg)](#目录-)

   + [![](https://img.shields.io/badge/-全家桶软件库-green.svg)](#全家桶软件库-)

      + [![](https://img.shields.io/badge/-软件库地址-lightgrey.svg)](#软件库地址-)
      + [![](https://img.shields.io/badge/-软件库更新说明-lightgrey.svg)](#软件库更新说明-)
      + [![](https://img.shields.io/badge/-软件库使用方法-lightgrey.svg)](#软件库使用方法-)
   + [![](https://img.shields.io/badge/-云编译固件-green.svg)](#云编译固件-)
      + [![](https://img.shields.io/badge/-设备及固件列表下载-lightgrey.svg)](#设备及固件列表下载-)
      + [![](https://img.shields.io/badge/-自动编译说明-lightgrey.svg)](#自动编译说明-)
   + [![](https://img.shields.io/badge/-赞助项目-green.svg)](#赞助项目-)
   + [![](https://img.shields.io/badge/-机场推荐-green.svg)](#机场推荐-)
   + [![](https://img.shields.io/badge/-鸣谢-green.svg)](#鸣谢-)
   + [![](https://img.shields.io/badge/-免责声明-green.svg)](#免责声明-)

第一部分
======================

openwrt-packages — OpenWrt第三方全家桶软件库 [![](https://img.shields.io/badge/-全家桶软件库-green.svg)](#全家桶软件库-)
======================

--编译脚本使用的第三方全家桶软件仓库[![](https://img.shields.io/badge/-软件库地址-lightgrey.svg)](#软件库地址-)
-------------

```bash
https://github.com/MrH723/openwrt-packages
```

-- 关于第三方全家桶软件仓库更新的说明[![](https://img.shields.io/badge/-软件库更新说明-lightgrey.svg)](#软件库更新说明-)
-------------

- 每日两次自动拉取更新所有上游源码至上方软件仓库，所以此软件仓库永远都是最新的。
- 云编译脚本会调用此仓库软件编译OpenWrt固件，每日一次编译。




-- 关于本软件仓库的使用方法[![](https://img.shields.io/badge/-软件库使用方法-lightgrey.svg)](#软件库使用方法-)
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

Actions-OpenWrt — 多设备固件自动云编译[![](https://img.shields.io/badge/-云编译固件-green.svg)](#云编译固件-)
======================

-- 支持的设备平台以及固件下载地址[![](https://img.shields.io/badge/-设备及固件列表下载-lightgrey.svg)](#设备及固件列表下载-)
-------------

|    序号   |     平台-设备名称     |   编译状态+下载链接 |  
| :-----------------: | :-------------: |:-----------------: | 
| 1 |   [![](https://img.shields.io/badge/OpenWrt-x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80%E7%89%88-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80+OpenWrt%22)    | [![x86多拨极简 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22x86%E5%A4%9A%E6%8B%A8%E6%9E%81%E7%AE%80+OpenWrt%22) |
| 2 |   [![](https://img.shields.io/badge/OpenWrt-x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80%E7%89%88-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80+OpenWrt%22)    | [![x86旁路由极简 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22x86%E6%97%81%E8%B7%AF%E7%94%B1%E6%9E%81%E7%AE%80+OpenWrt%22) |
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
| 21 |   [![](https://img.shields.io/badge/OpenWrt-Amlogic%20S905X3-lightgrey.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Amlogic+S905X3+OpenWrt%22)    | [![Build Amlogic S905X3 OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20Amlogic%20S905X3%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+Amlogic+S905X3+OpenWrt%22) |
| 22 |   [![](https://img.shields.io/badge/OpenWrt-%E9%A6%99%E6%A9%99%E6%B4%BE%20Zero%20Plus-yellowgreen.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+%E9%A6%99%E6%A9%99%E6%B4%BE+Zero+Plus+OpenWrt%22)    | [![Build 香橙派 Zero Plus OpenWrt](https://github.com/MrH723/Actions-OpenWrt/workflows/Build%20%E9%A6%99%E6%A9%99%E6%B4%BE%20Zero%20Plus%20OpenWrt/badge.svg)](https://github.com/MrH723/Actions-OpenWrt/actions?query=workflow%3A%22Build+%E9%A6%99%E6%A9%99%E6%B4%BE+Zero+Plus+OpenWrt%22) |

-- 关于自动编译固件的说明[![](https://img.shields.io/badge/-自动编译说明-lightgrey.svg)](#自动编译说明-)
-------------

- 不建议Fork，按需下载即可。
- 自动编译，自动拉取最新版本插件。
- x86多拨极简版为自用固件仅包含 （pw,S,上网时间控制，upnp,ddns,去广告，多拨，负载均衡，流量监控，主题只加入了默认主题以及自己比较喜欢的edge主题）
- x86旁路由极简版为自用，建议配合爱快使用，仅包含（pw，S，去广告，主题只加入了默认主题以及自己比较喜欢的edge主题）
- x86全家桶固件正在处理中，由于部分插件冲突需要些时间排雷。

赞助[![](https://img.shields.io/badge/-赞助项目-green.svg)](#赞助项目-)
======================
- 您要是觉得好用不错的话，不妨考虑赞助一下本项目。

<img src="https://github.com/MrH723/Actions-OpenWrt/blob/main/img/alipay.jpg?raw=true" width="160" height="180" />

我用过的机场[![](https://img.shields.io/badge/-机场推荐-green.svg)](#机场推荐-)
======================

[我用过的机场]  [![](https://img.shields.io/badge/%E5%85%A8IPLC%E6%9C%BA%E5%9C%BA-iplc.vip-brightgreen.svg)](https://portal.iplc-j.pw/aff.php?aff=1228)

鸣谢[![](https://img.shields.io/badge/-鸣谢-green.svg)](#鸣谢-)
======================
 
[P3TERX 的 Action 源码] [![](https://img.shields.io/badge/P3TERX-源码-orange.svg)](https://github.com/P3TERX/Actions-OpenWrt)

[Lean 的 OpenWrt 源码] [![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)

特别鸣谢
======================
[Lienol] [![](https://img.shields.io/badge/Lienol-%E6%BA%90%E7%A0%81-orange.svg)](https://github.com/Lienol)

[Kenzok8] [![](https://img.shields.io/badge/Kenzok8-%E6%BA%90%E7%A0%81-orange.svg)](https://github.com/kenzok8)


免责声明[![](https://img.shields.io/badge/-免责声明-green.svg)](#免责声明-)
======================
***- 由于本人小白，有可能使用到了大神的代码，没有放进鸣谢名单里的，请联系添加，再次感谢各位大神的贡献***

***- 请务必遵从‘不涉及政治，不涉及宗教，不涉及黄赌毒’的三不原则***


