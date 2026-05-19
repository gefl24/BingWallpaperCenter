# 🏔️ BingWallpaperCenter (必应壁纸控制台)

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Windows-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

BingWallpaperCenter 是一个优雅、轻量且纯粹的跨平台桌面壁纸引擎。它能够在后台默默为你抓取每日必应 4K 壁纸并自动更换，同时提供了一个媲美 macOS 原生系统美学的控制面板。

告别臃肿的流氓软件，把桌面的控制权交还给自己。

## ✨ 核心特性

- 🍏 **Mac 原生级体验**：完美融入 macOS 生态。纯状态栏 (Menu Bar) 驻留，**彻底隐藏 Dock 栏图标**。UI 界面 1:1 复刻 macOS 系统设置，支持深色/浅色模式无缝切换。
- 🛡️ **底层 API 驱动 (零弹窗)**：针对 macOS 重写底层逻辑，放弃繁琐的 AppleScript，直接调用 `AppKit/NSWorkspace` 原生 API 更换壁纸，**不会弹出烦人的权限请求窗口**。
- 🕰️ **历史时光机**：突破微软官方 API 仅支持近 8 天数据的限制！内置全量穷举引擎，可从 GitHub 归档库定向拉取过去数月甚至数年的必应 4K 历史壁纸。
- 🚀 **双进程守护架构**：前后台彻底分离。UI 界面关闭即刻释放内存，仅留占用极低的 Daemon 守护进程在后台默默调度定时任务。
- ⚡ **极致性能优化**：告别原图加载卡顿。内置轻量级图像处理引擎（Pillow），在后台动态生成并缓存极小体积的缩略图，千张图库也能秒开。

