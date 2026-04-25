# <img src="https://lxj13533251583.github.io/WT-Permission/avatar.jpg" width="25" align="center"> WT权限站

一个完全运行在浏览器端的**隐私权限检测工具**，帮助用户了解网站在不经授权或主动授权的情况下，能够获取到哪些设备与网络信息。

<div>
  <a href="https://github.com/lxj13533251583/WT-Permission/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="License">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission">
    <img src="https://img.shields.io/badge/website-live-brightgreen" alt="Website">
  </a>
  <br>
  <a href="https://github.com/lxj13533251583/WT-Permission/stargazers">
    <img src="https://img.shields.io/github/stars/lxj13533251583/ldy" alt="GitHub stars">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission/commits/main">
    <img src="https://img.shields.io/github/last-commit/lxj13533251583/ldy" alt="GitHub last commit">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission/releases">
    <img src="https://img.shields.io/github/v/release/lxj13533251583/ldy" alt="GitHub release">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission/releases">
    <img src="https://img.shields.io/github/release-date/lxj13533251583/ldy" alt="Release date">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission">
    <img src="https://img.shields.io/github/repo-size/lxj13533251583/ldy" alt="Repo size">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission/commits/main">
    <img src="https://img.shields.io/github/commit-activity/m/lxj13533251583/ldy" alt="Commit activity">
  </a>
  <a href="https://github.com/lxj13533251583/WT-Permission">
    <img src="https://img.shields.io/badge/Maintenance-Active-brightgreen" alt="Maintenance">
  </a>
</div>

🌐 **在线体验**：[点击跳转](https://lxj13533251583.github.io/ldy/)

## 📌 功能总览

本站将可检测的权限与信息按敏感度分为五个等级：

| 等级 | 颜色 | 示例信息 |
|------|------|----------|
| 🔴 极高敏感 | 红色 | 公网IP、WebGL指纹、Canvas指纹、音频指纹、电池状态、已安装字体、综合设备指纹 |
| 🟠 高敏感 | 橙色 | Cookie、LocalStorage、SessionStorage、IndexedDB、浏览历史长度、页面可见性 |
| 🟡 中等敏感 | 黄色 | 精确时间、CPU核心数、设备内存、网络延迟/带宽/类型、DNS/TCP/TLS耗时 |
| 🔵 低敏感 | 蓝色 | 省流量模式、完整UA、平台、浏览器版本、语言偏好、上行速率测试 |
| 🟢 极低敏感 | 绿色 | 屏幕分辨率、像素比、时区、系统语言、渲染引擎、API支持情况、缓存状态、色彩深度 |

**权限请求模块**（需用户手动授权）覆盖：
- 定位、摄像头、麦克风、通知、剪贴板读写、屏幕录制、蓝牙、USB、串口、HID、本地文件访问、永久存储、后台同步、运动传感器、设备振动、多屏管理等。

**实时行为追踪**（高敏感页内）会记录鼠标点击、滚动次数和时间戳。

## ✨ 特性

- ✅ **纯前端检测**，所有隐私数据仅在浏览器内计算与显示，**不会上传任何信息到外部服务器**。
- ✅ 唯一的外部请求是调用公开的 IP 归属地 API（ipify 和 ipapi.co）获取公网IP和运营商/城市。
- ✅ 响应式设计，支持亮色/暗色模式跟随系统。
- ✅ 点击每个信息项的标签可查看详细解释。
- ✅ 优雅的动画与模态弹窗。

## 🛠 技术栈

- HTML5 + CSS3
- 原生 JavaScript
- [Font Awesome](https://fontawesome.com/) 图标
- 浏览器 API：WebGL、Canvas、AudioContext、Battery Status、Performance、Navigator、Screen、Intl、Clipboard、MediaDevices、Bluetooth、USB、Serial、HID 等

---

<div align="center">
  &copy; 2026 旅冬亦 版权所有
</div>