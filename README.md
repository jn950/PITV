# 📺 ΠTV (PITV) · 智能电视极速播放器

<p align="center">
  <img src="https://img.shields.io/badge/Release-v1.3.4.4-brightgreen.svg" alt="Latest Release" />
  <img src="https://img.shields.io/badge/Platform-Android%20TV%20%7C%20Box-blue.svg" alt="Platform" />
  <img src="https://img.shields.io/badge/Arch-armeabi--v7a%20%7C%20arm64--v8a-orange.svg" alt="Architecture" />
  <img src="https://img.shields.io/badge/Android-4.4%2B-blueviolet.svg" alt="Android Compatibility" />
  <img src="https://img.shields.io/badge/License-Apache--2.0-lightgrey.svg" alt="License" />
</p>

---

## 🌟 项目简介

**ΠTV (PITV)** 是一款专为智能电视（Android TV）、机顶盒及大屏安卓设备量身打造的高性能 IPTV 直播播放器。

本项目基于定制优化的高性能播放内核与底层 Native C 安全加速模块构建，具有**毫秒级起播、极速平滑换台、全格式多线路自动容错、手机局域网扫码遥控与自建直播源管理**等核心特性。

- 📦 **GitHub 仓库**：[https://github.com/jn950/PITV](https://github.com/jn950/PITV)
- 🚀 **最新版本下载**：[GitHub Releases 发布页面](https://github.com/jn950/PITV/releases)
- ⚡ **国内高速直链下载**：[PITV-v1.3.4.4.apk (高速代理镜像)](https://gh-proxy.org/https://github.com/jn950/PITV/releases/download/pitv/PITV-v1.3.4.4.apk)

---
![截图](/img/img1.jpg)
![截图](/img/img5.png)
![截图](/img/img2.png)
![截图](/img/img3.png)
![截图](/img/img4.png)
![截图](/img/img6.png)
![截图](/img/img7.png)

## ✨ 核心特性

### 1. 🚀 毫秒级起播与硬解加速
- 集成定制优化版 `ijkplayer` 媒体内核，底层深度优化缓冲区机制与网络探测策略。
- 自动适配 MediaCodec 硬件解码，4K / 1080P 超高清低延迟稳定解码，告别卡顿与音画不同步。
- 支持 HLS (`.m3u8`)、FLV、TS、MP4、MPEG-DASH 等主流协议流的动态识别与无缝分流。

### 2. 📡 全域电视频道与独家解析
- **央视 / 卫视 / 地方高清频道**：覆盖全国主流频道，支持央视频 (YSP) 原生鉴权解析起播。
- **⚽ 咪咕体育赛事专区**：独家支持咪咕体育赛事直播，内置**昨日、今日、明日**独立赛程三级分类导航，赛事实时追踪。
- **🌐 互联网主流直播生态**：支持 Bilibili、抖音、虎牙、斗鱼、YY、看看新闻、触电新闻 (GDTV) 等网络直播流一键直连。
- **地方专线专区**：内置江苏 (JSTV)、河南 (HNTV)、海南 (HNNTV)、芒果TV (MGTV) 等多地省市专线。

### 3. 📱 手机扫码局域网可视化遥控
- 内置轻量级本地 HTTP 控制服务，无需安装任何额外 App，同局域网下**手机扫码即用**。
- **可视化触控换台**：大屏当前播放状态实时同步，支持点击频道换台、音量调节、偏好设置。
- **自定义直播源管理**：支持自定义 M3U / M3U8 / TXT 格式直播源批量导入、编辑与云端同步。
- **会员账号系统**：支持卡密与账号登录激活，专享云端订阅源与高速加速专区。

### 4. 🛡️ Native 安全体系与完整性防护
- 核心算法与签名校验全部沉降至底层 Native C (`libtv_security.so`) 模块编译。
- 主线程快速自检防二次打包，保证客户端环境纯净可靠。
- 结合远端版本时效策略与备用节点自动容错，保障服务的可持续性与稳定性。

### 5. 🎮 遥控器与大屏专属交互
- 专为大屏距离优化的现代化暗色微光 UI 与悬浮台标。
- 完整的实时 EPG 电子节目单展示，预加载下一节目信息。
- 支持**数字键快速选台**（屏幕浮动数字水印）、**方向上下键极速换台**、**方向左右键平滑切换多线路**。

---

## 🕹️ 遥控器操作指南

| 按键 | 功能说明 |
| :--- | :--- |
| **【上 / 下键】** | 切换上一个 / 下一个电视频道 |
| **【左 / 右键】** | 切换当前频道的备用线路 / 多码率线路 |
| **【OK / 确定键】** | 打开频道列表与 EPG 节目单面板 |
| **【菜单键 (Menu)】** | 打开电视端局域网管理后台（查看 IP、管理地址与二维码） |
| **【返回键 (Back)】** | 退出列表或连续按返回键确认退出应用 |
| **【数字键 0-9】** | 直接输入频道号极速直达选台 |

---

## 📝 最近更新日志 (v1.3.4.4)

- 🔒 **强化安全防御**：新增底层 Native C 签名完整性自检与自毁机制，全面防范二次打包与非法篡改。
- ⚽ **咪咕体育重构**：全新重构咪咕体育赛程，实现**昨日 / 今日 / 明日**独立分类三级赛事看板。
- 📺 **版本展示与遥控关于**：在频道列表品牌标及 Web 遥控端“关于”中常驻显示官方客户端版本号。
- 🌐 **双通道时效策略**：版本时效策略接入 `my9.ltd` 官方主节点，并配置离线与备用容灾热备。
- ⚡ **播放体验提升**：优化起播预缓冲分配策略，极大提升老旧电视盒子及弱网环境下的秒开率。

---

## 📥 下载与安装

### 方式一：国内镜像加速下载（推荐）
点击下方直链，即可通过加速节点直接下载最新版 APK 安装包：
👉 **[下载最新 PITV-v1.3.4.4.apk (高速代理镜像)](https://gh-proxy.org/https://github.com/jn950/PITV/releases/download/pitv/PITV-v1.3.4.4.apk)**

### 方式二：GitHub Releases 官方下载
前往官方 Releases 发布仓库下载：
👉 **[GitHub Releases - jn950/PITV](https://github.com/jn950/PITV/releases)**

### 安装说明：
1. 下载 `.apk` 文件并拷贝至 U 盘；
2. 将 U 盘插入智能电视或电视盒子的 USB 接口；
3. 打开电视自带的文件管理器，找到安装包并根据系统提示授权安装即可。

---

## 🛠️ 本地编译构建

本项目基于 Android SDK 与 Android NDK 构建：

```bash
# 1. 克隆代码仓库
git clone https://github.com/jn950/PITV.git
cd PITV

# 2. 编译底层 Native 动态链接库 (需要配置 NDK r21e 及以上)
cd app/src/main/jni
ndk-build NDK_PROJECT_PATH=. APP_BUILD_SCRIPT=Android.mk NDK_APPLICATION_MK=Application.mk

# 3. 返回工程根目录执行正式签名打包
cd ../../../..
./gradlew assembleRelease
```
编译产物位于：`app/build/outputs/apk/release/app-release.apk`。

---

## ⚖️ 免责声明 (Disclaimer)

1. 本项目仅供个人学习、流媒体编解码技术研究及智能大屏交互体验交流使用。
2. 本项目自身不分发、不托管、不存储任何音视频节目内容，所有直播流地址均源自公开互联网或用户自建导入。
3. 请在遵守相关法律法规的前提下合法合规使用。

---

## 💖 致谢与开源项目

- 原项目致谢：[NativeWasmTv](https://github.com/buhanzhe/NativeWasmTv)
- 播放内核：[bilibili / ijkplayer](https://github.com/bilibili/ijkplayer)
- Google AndroidX & ExoPlayer
