# Action Openwrt Cloud Automatic Compilation
⏰ **Automatically pull the latest source code and compile it every week**

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<br />

<p align="center">
  <a href="https://github.com/bigbugcc/OpenWrts">
    <img src="./assets/images/action1.jpg" alt="Logo" width="500" />
  </a>
  <h3 align="center">Openwrt/LEDE cloud compilation (with app store)</h3>
  <p align="center">
    👉 Automatically pull the latest Openwrt source code and compile it every week, and automatically publish it to [<a herf="https://github.com/bigbugcc/OpenWrts/releases"> Releases </a>]👈
    <br />
    <a href="https://github.com/bigbugcc/OpenWrts"><strong>Explore the project's documentation»</strong></a>
    <br />
    <br />
    <a href="https://github.com/bigbugcc/OpenWrts/releases">download link</a>
    ·
    <a href="https://github.com/bigbugcc/OpenWrts/actions">Action</a>
    ·
    <a href="https://github.com/bigbugcc/OpenWrts/issues">Propose new features</a>
  </p>

</p>

## Table of contents

- [Action Openwrt Cloud automatic compilation](#action-openwrt-Cloud-automatic-compilation)
- [Directory](#Directory)
- [Supported Devices](#SupportedDevices)
- [🎯Firmware Default Settings](#Firmware-Default-Settings)
- [Firmware Features](#Firmware-Features)
- [Built-in Plugins](#Built-inPlugins)
- [File Directory Description](#FileDirectoryDescription)
- [Custom Firmware](#CustomFirmware)
- [Notes](#Notes)
- [Firmware Preview](#FirmwarePreview)
- [Copyright Notice](#CopyrightNotice)
- [Project Support](#ProjectSupport)
- [Stargazers over time](#stargazers-over-time)
<br>


## Supported devices
🎯 Firmware with app store: `x86Lite`
|           Supported devices        |         Category         |        Action         |            state          |              Download page          |
| :------------------------: | :---------------------: | :-------------------: | :-------------------: | :--------------------------: |
|             x86_64                    |  [LEDE](https://github.com/coolsnowwolf/lede) |[🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/x86_64.yml) | ![x86_64](https://github.com/bigbugcc/openwrts/actions/workflows/x86_64.yml/badge.svg) |  [✔](https://github.com/bigbugcc/OpenWrts/releases) |
| x86_64Lite | [LEDE](https://github.com/coolsnowwolf/lede) |[🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/x86_64Lite.yml) | ![x86_64Lite](https://github.com/bigbugcc/openwrts/actions/workflows/x86_64Lite.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             Raspberry Pi 3B/3B+             | [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/RaspberryPi3.yml) | ![RaspberryPi3](https://github.com/bigbugcc/openwrts/actions/workflows/RaspberryPi3.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             Raspberry Pi 4B             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/RaspberryPi4.yml) | ![RaspberryPi4](https://github.com/bigbugcc/openwrts/actions/workflows/RaspberryPi4.yml/badge.svg) |  [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             Raspberry Pi 5             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/RaspberryPi5.yml) | ![RaspberryPi5](https://github.com/bigbugcc/openwrts/actions/workflows/RaspberryPi5.yml/badge.svg) |  [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             NanoPi R2S             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![R2S](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             NanoPi R4S             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![R4S](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             NanoPi R5C             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![R5C](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             NanoPi R5S             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![R5S](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             FastRhino R68S             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![R68S](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |
|             Orange Pi R1 Plus             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/bigbugcc/OpenWrts/actions/workflows/Rockchip_armv8.yml) | ![OrangePiR1](https://github.com/bigbugcc/openwrts/actions/workflows/Rockchip_armv8.yml/badge.svg) | [✔](https://github.com/bigbugcc/OpenWrts/releases) |

<br>

### 🎯 Firmware-Default-Settings
- Router address: `192.168.10.1`
- Default username: `root`
- Default password: `password`

<br>

## Firmware-Features
⏰ Firmware compilation changed to `weekly update` (mainly stability, reduce resource waste)

✨ iStore application store [AppStore](./assets/images/appstore.png)

✨ Built-in commonly used plug-ins

✨ Arm integrates all openwrt USB drivers

✨ ~~Integrated Python3.x (with pip) environment~~

✨ Integrated Docker-CE

✨ ~~Integrated Node.js (14.xLTS with npm, yarn)~~

✨ Brand new [Them](https://github.com/jerrykuku/luci-theme-argon)

✨ x86_64 vmdk firmware integrated with vm-tools

✨ x86_64 iso format image

✨ x86_64 Lite version (necessary plug-ins & application store)

<br>

## 自带插件
🍕 默认插件
- PassWall2 / SSR Plus
- AdGuard Home
- Mentohust
- ~~luci-app-vssr~~
- luci-adbyby-plus
- luci-app-unblockmusic
- luci-app-ddns
- luci-app-pushbot (全能推送)
- luci-app-onliner
- luci-app-ttyd
- luci-app-turboacc
- luci-app-upnp
- luci-app-netdata
- luci-usb-printer
- luci-app-nps
- luci-app-frpc
- luci-app-n2n
- luci-app-syncdial (多播插件)
- luci-app-turboacc
- luci-app-kms
- luci-app-docker
- luci-app-serverchan
- luci-app-control-timewol (定时wol唤醒)
- luci-app-aliyundrive-webdav (阿里云盘)
- luci-app-filebrowser
- luci-app-nfs   
......

<br>

## File directory description
eg:
```
filetree
├── .github/workflows
│  ├── Rockchip_armv8.yml
│  ├── RaspberryPi3.yml
│  ├── RaspberryPi4.yml
│  ├── RaspberryPi5.yml
│  ├── x86_64.yml
│  ├── x86_64Lite.yml
│  ├── update-checker.yml
├── /configs/ (配置文件目录)
│  ├── LuciApp.config (插件配置文件)
│  ├── LuciApp_Lite.config (简洁配置文件)
│  ├── RPi3.config
│  ├── RPi4.config
│  ├── RPi5.config
│  ├── x86_64.config
│  ├── Rockchip.config
├── configure.sh (固件参数修改)
├── package.sh (luci-app)

Tips:
x86.conf | RPi4.config - 该类型配置文件主要为机型配置文件
LuciApp.conf / LuciApp_Lite.conf - 主要用于配置固件插件应用 
```
<br>

## 定制固件
1. Fork 此项目
2. 按需修改 ```configure.sh``` 和 ```package.sh``` 文件
3. 上传你自己的 ```xx.config``` 配置文件到configs目录
4. 添加或修改自己的``````xx.yml``````文件
5. 最后根据个人喜好修改 ```update-checker.yml``` 需自行添加 ```Actions secrets``` (触发自动编译)

### 注意事项：
📌 修改默认系统参数 👉 ```configure.sh```   
📌 添加其它Luci插件 👉 ```package.sh```   
📌 插件 / 应用配置文件 👉 ```configs/LuciApp.config```   
<br>

## 固件预览
**主界面(主题一)：**
![主界面](./assets/images/openwrt.png)

**应用商店/插件**
![应用商店/插件](./assets/images/appstore.png)

**服务/插件：**
![服务/插件](./assets/images/service.png)

**网络：**
![网络](./assets/images/network.png)

**经典主题二：**
![登录页](./assets/images/infinityfreedom-theme.png)

**主界面：**
![主界面](./assets/images/infinityfreedom-theme-main.png)


## 版权说明

该项目签署了MIT 授权许可，详情请参阅 [LICENSE](https://github.com/bigbugcc/OpenWrts/blob/main/LICENSE)


## 项目支持
- [P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [luci-theme-argon](https://github.com/jerrykuku/luci-theme-argon)
- [istore](https://github.com/linkease/istore)

## Stargazers over time
[![Stargazers over time](https://starchart.cc/bigbugcc/OpenWrts.svg)](https://starchart.cc/bigbugcc/OpenWrts)

<!-- links -->
[your-project-path]:https://github.com/bigbugcc/OpenWrts/
[contributors-shield]: https://img.shields.io/github/contributors/bigbugcc/OpenWrts?style=flat-square
[contributors-url]: https://github.com/bigbugcc/OpenWrts/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/bigbugcc/OpenWrts?style=flat-square
[forks-url]: https://github.com/bigbugcc/OpenWrts/network/members
[stars-shield]: https://img.shields.io/github/stars/bigbugcc/OpenWrts?style=flat-square
[stars-url]: https://github.com/bigbugcc/OpenWrts/stargazers
[issues-shield]: https://img.shields.io/github/issues/bigbugcc/OpenWrts?style=flat-square
[issues-url]: https://img.shields.io/github/issues/bigbugcc/OpenWrts
[license-shield]: https://img.shields.io/github/license/bigbugcc/OpenWrts?style=flat-square
[license-url]: https://github.com/bigbugcc/OpenWrts/blob/master/LICENSE
