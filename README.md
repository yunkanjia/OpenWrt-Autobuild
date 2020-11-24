OpenWrt DIY — 多设备固件云编译
======================

[![](https://img.shields.io/badge/-目录:-696969.svg)](#readme) [![](https://img.shields.io/badge/-基本介绍-F5F5F5.svg)](#基本介绍-) [![](https://img.shields.io/badge/-近期更新-F5F5F5.svg)](#近期更新-) [![](https://img.shields.io/badge/-注意事项-F5F5F5.svg)](#注意事项-) [![](https://img.shields.io/badge/-USB网卡推荐-F5F5F5.svg)](#usb-网卡推荐-) [![](https://img.shields.io/badge/-OpenWrt小贴士-F5F5F5.svg)](#openwrt-小贴士-)

<p align="center"></p>

**点击下表中 [![](https://img.shields.io/badge/设备-passing-32CD32.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions) 即可跳转到该设备固件下载页面** 

|    序号   |     设备平台     |   编译状态及下载链接 |   源码   | 备注说明   |
| :-----------------: | :-------------: |:-----------------: | :-----------------: |  :-----------------: | 
| 1 |   [![](https://img.shields.io/badge/OpenWrt-x86_64_(64位)-FFFFFF.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2864bit%29+OpenWrt%22)    | [![](https://github.com/dreamskr/OpenWrt-DIY/workflows/Build%20X86(64bit)%20OpenWrt/badge.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2864bit%29+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |  |  
| 2 |    [![](https://img.shields.io/badge/OpenWrt-x86_(32位)-FFFFFF.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2832bit%29+OpenWrt%22)     |[![](https://github.com/dreamskr/OpenWrt-DIY/workflows/Build%20X86(32bit)%20OpenWrt/badge.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+X86%2832bit%29+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) | | 
| 3 |    [![](https://img.shields.io/badge/OpenWrt-树莓派_4B-FFFFFF.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22)    | [![](https://github.com/dreamskr/OpenWrt-DIY/workflows/Build%20RaspBerryPi4%20OpenWrt/badge.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+RaspBerryPi4+OpenWrt%22)  |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede)  | 含 USB 网卡驱动，自用 |
| 4|     [![](https://img.shields.io/badge/OpenWrt-网件_R7800-FFFFFF.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22)   | [![](https://github.com/dreamskr/OpenWrt-DIY/workflows/Build%20Netgear%20R7800%20OpenWrt/badge.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+R7800+OpenWrt%22) |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |
| 5|     [![](https://img.shields.io/badge/OpenWrt-网件_wndr3800-FFFFFF.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+wndr3800+OpenWrt%22)   | [![](https://github.com/dreamskr/OpenWrt-DIY/workflows/Build%20Netgear%20wndr3800%20OpenWrt/badge.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions?query=workflow%3A%22Build+Netgear+Wndr3800+OpenWrt%22)  |[![](https://img.shields.io/badge/Lean-源码-orange.svg)](https://github.com/coolsnowwolf/lede) |   |

**提示：**[![](https://img.shields.io/badge/设备-passing-32CD32.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions) 标志为正常，[![](https://img.shields.io/badge/设备-failing-DC143C.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions) 或 [![](https://img.shields.io/badge/设备-no_status-A9A9A9.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions) 不代表所有编译均失败。请点击 [![](https://img.shields.io/badge/设备-状态-32CD32.svg)](https://github.com/dreamskr/OpenWrt-DIY/actions) 到 **Actions** 进一步查看。

<a href="#readme">
    <img src="https://img.shields.io/badge/-返回顶部-orange.svg" alt="图裂了??" title="返回顶部" align="right"/>
</a>

## 基本介绍

- 根据 [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) 的步骤(第1~4步)，生成 `.config` . 
- 上传 `.config` 文件到GitHub 目录.
- 在Actions页选择 `Build OpenWrt`.
- 点击 `Run workflow` 按钮.
- 当编译完成后，在Actions页的右上角，点击 `Artifacts` 按钮下载固件.

## 鸣谢 
 
- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [c-hive/gha-remove-artifacts](https://github.com/c-hive/gha-remove-artifacts)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)

###### [解决 Github 网页上图片显示失败的问题](https://blog.csdn.net/qq_38232598/article/details/91346392)

<a href="#readme">
    <img src="https://img.shields.io/badge/-返回顶部-orange.svg" alt="图裂了??" title="返回顶部" align="right"/>
</a>
