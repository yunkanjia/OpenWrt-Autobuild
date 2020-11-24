[![如页面部分图片无法显示，请直接点这里到末尾看修复教程](https://visitor-badge.glitch.me/badge?page_id=OpenWrt-DIY-visitor-badge)](#解决-github-网页上图片显示失败的问题) [![](https://img.shields.io/github/issues/dreamskr/OpenWrt-DIY?color=FFFFFF)](https://github.com/dreamskr/OpenWrt-DIY/issues) [![](https://img.shields.io/github/stars/dreamskr/OpenWrt-DIY?color=FFFFFF)](https://github.com/dreamskr/OpenWrt-DIY/stargazers) [![](https://img.shields.io/github/forks/dreamskr/OpenWrt-DIY?color=FFFFFF)](https://github.com/dreamskr/OpenWrt-DIY/network/members)
<a href="#readme">
    <img src="https://img.vim-cn.com/48/6e4b91fdeefa201f93befdf858a13eefeaff5c.jpg" alt="图裂了😂" title="OpenWrt-DIY" align="right" height="180" />
</a>

OpenWrt DIY — 多设备固件云编译
======================

[![](https://img.shields.io/badge/-目录:-696969.svg)](#readme) [![](https://img.shields.io/badge/-基本介绍-F5F5F5.svg)](#基本介绍-) [![](https://img.shields.io/badge/-鸣谢-F5F5F5.svg)](#鸣谢-)

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

#### 1.单次编译用法 [参考Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)
- 根据 [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) 的步骤(第1~4步)，生成 `.config` . 
- 上传 `.config` 文件到GitHub 目录.
- 在Actions页选择 `Build OpenWrt`.
- 点击 `Run workflow` 按钮.
- 当编译完成后，在Actions页的右上角，点击 `Artifacts` 按钮下载固件.

#### 2.自动编译用法 [参考IvanSolis1989](https://github.com/IvanSolis1989/OpenWrt-DIY)
- 除了build-openwrt.yml，其它每周五 12:00 拉取 Lean 最新源码和第三方软件包项目自动编译（根据设备不同编译时间在1~5个小时，这样晚上回家就可以愉快的开刷啦），默认情况下固件每周编译一次 (config 文件更新时除外)，固件包含必要驱动及常用插件（各设备的 config 借鉴大雕设置及根据网友需求调整），未逐一经过实机测试，故 不保证 100% 可靠性. 
- 在固件编译完成后，会上传一份副本到 WeTransfer 和 奶牛快传，对于国内网络用户，为提高下载体验，可下载存放于这两个网站中的固件副本，副本下载地址位于固件下载页面中固件文件列表下的 Annotations 提示框内，几天之后网盘内的文件会失效，所以推荐周五~周日上去下载；
- 在极少数情况下，因网络原因这两份副本可能会上传失败，如果遇到这种情况，就只能下载存放在 Github Action 里的固件了，由于 Github Action 限制，需要登录 Github 账号才可下载存放于 Github Action 中的固件 (未登录时固件链接不可被点击)，但 WeTransfer 和 奶牛快传 的固件下载链接在未登录状态下可正常查看，不受影响；
- 如果需要下载存放于 Github Action 上的固件，由于众所周知的原因，请尽量使用科学上网方式下载固件，固件下载完成后，请下载 sha256sums 文件或使用压缩软件的 "测试压缩文件" 功能来验证固件的完整性。
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
