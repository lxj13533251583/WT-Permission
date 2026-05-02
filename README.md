# <img src="https://ldy2330785100.github.io/WT-Permission/avatar.jpg" width="25" align="center"> WT权限站

一个完全运行在浏览器端的**隐私权限检测工具**，帮助用户了解网站在不经授权或主动授权的情况下，能够获取到哪些设备与网络信息。

<div>
  <a href="https://github.com/ldy2330785100/WT-Permission">
    <img src="https://img.shields.io/badge/website-live-brightgreen" alt="Website">
  </a>
  <br>
  <a href="https://github.com/ldy2330785100/WT-Permission/stargazers">
    <img src="https://img.shields.io/github/stars/ldy2330785100/WT-Permission" alt="GitHub stars">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission/commits/main">
    <img src="https://img.shields.io/github/last-commit/ldy2330785100/WT-Permission" alt="GitHub last commit">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission/releases">
    <img src="https://img.shields.io/github/v/release/ldy2330785100/WT-Permission" alt="GitHub release">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission/releases">
    <img src="https://img.shields.io/github/release-date/ldy2330785100/WT-Permission" alt="Release date">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission">
    <img src="https://img.shields.io/github/repo-size/ldy2330785100/WT-Permission" alt="Repo size">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission/commits/main">
    <img src="https://img.shields.io/github/commit-activity/m/ldy2330785100/WT-Permission" alt="Commit activity">
  </a>
  <a href="https://github.com/ldy2330785100/WT-Permission">
    <img src="https://img.shields.io/badge/Maintenance-Active-brightgreen" alt="Maintenance">
  </a>
</div>

🌐 **在线体验**：[点击跳转](https://ldy2330785100.github.io/WT-Permission/)

## 📌 功能总览

本站将可检测的权限与信息按敏感度分为五个等级，每个等级下展示大量无需授权即可获取的信息：

| 等级 | 颜色 | 主要检测信息 |
|------|------|----------------|
| 极高敏感 | 🔴 | 公网IP、运营商、IP归属地、WebGL渲染器、Canvas/音频指纹、电池状态、CPU核心数、已安装字体、浏览器插件、综合设备指纹 |
| 高敏感 | 🟠 | Cookie、LocalStorage、SessionStorage、IndexedDB、Referrer、历史记录长度、页面可见性、闲置时长 |
| 中等敏感 | 🟡 | 精确系统时间、设备内存、RTT延迟、下行带宽、网络连接类型、DNS/TCP/TLS耗时、页面加载时间 |
| 低敏感 | 🔵 | 网络类型（WiFi/数据流量/以太网）、省流量模式、完整UA、操作系统、浏览器版本、语言偏好、上行测速 |
| 极低敏感 | 🟢 | 屏幕物理分辨率、像素比、屏幕方向、时区（中文）、地区码、系统语言、渲染引擎、API支持列表、DOM加载时间、缓存状态、MIME类型、默认字号、色彩深度 |

 **手动授权权限**：支持以下需要用户主动授权的权限请求按钮：
- 定位、摄像头、麦克风、通知、剪贴板读写、屏幕录制/共享、蓝牙、USB、串口、外设键鼠/手柄（HID）、本地文件访问、永久存储、后台同步、运动传感器、设备振动、多屏幕管理等。

**实时行为追踪**：可记录并展示点击、滚轮滚动等行为，支持卡片内滚动。

## ✨ 主要特性

- ✅ **纯前端运行**：所有检测均在浏览器本地完成，不会将隐私数据上传至任何服务器。唯一的外部请求是用于获取公网IP归属地的公开API（可配置）。
- ✅ **智能交互**：
  - 点击权限名可查看详细解释。
  - 点击任意已获取的信息文字可直接复制到剪贴板，并在文字旁弹出“已复制”提示。
  - 授权成功/失败分别用绿色圆形勾和红色圆形叉图标表示，直观且不突兀。
- ✅ **优雅的动效**：
  - 页面切换、卡片入场使用弹簧缓动曲线，呈现淡入滑入效果。
  - 加载状态统一使用沙漏⏳旋转动画。
- ✅ **汉化支持**：
  - 时区、网络类型、系统语言等信息自动映射为中文（如 `Asia/Shanghai` → `亚洲/上海`，`cellular` → `数据流量`）。
  - 时间单位统一为`秒`
- ✅ **响应式与主题**：跟随系统亮色/暗色模式，适配手机与电脑屏幕。
- ✅ **隐私提醒**：简介提醒用户谨慎截图或公开访问，保护个人隐私。

## 🛠 技术栈

- HTML5 + CSS3（Grid 布局、自定义属性、媒体查询、动画）
- 原生 JavaScript（ES6+，IntersectionObserver、Clipboard API、各种浏览器原生API）
- 浏览器 API 覆盖：
  - `fetch`、`WebGL`、`Canvas 2D`、`AudioContext`、`Battery Status`、`Performance`、`Navigator`、`Screen`、`Intl`、`Clipboard`、`MediaDevices`、`Bluetooth`、`USB`、`Serial`、`HID` 等

## 🔗源码
- [前往下载](https://github.com/ldy2330785100/WT-Permisson/releases/)

## 📝 更新日志

- [ChangeLog](https://ldy2330785100.github.io/WT-Permission/changelog.html)

## ⚠️ 声明

1. **项目性质**：本项目为个人技术练习与作品展示，非商业用途，不代表任何官方立场。
2. **版权与许可**：
   - **代码**：本项目代码采用 **[MIT License](https://opensource.org/licenses/MIT)** 开源。
   - **图标**：图标为原创，未经允许禁止商用；如需个人使用请告知作者。
3. **责任限制**：作者不对因使用本项目代码或访问网站内容导致的任何损失承担责任。
4. **隐私说明**：
   - 本网站为纯静态页面，不收集任何用户隐私数据，所有设置仅保存在浏览器本地。
   - 所有检测均在本机浏览器完成，除公网IP查询需调用公开API外，不会将任何数据发送到外部服务器。不建议在本站内**截图**或公开访问，以免泄露隐私。

## 🙏 特别鸣谢

- [GitHub](https://github.com) 提供仓库与 Pages 托管服务
- https://chat.deepseek.com 提供技术建议与代码优化
- [Font Awesome](https://fontawesome.com) 提供高质量图标库

---

<div align="center">
  &copy; 2026 旅冬亦 版权所有
</div>