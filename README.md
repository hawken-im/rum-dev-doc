# Rum SDK 文档

### 文档说明 <a href="#shen-me-shi-rum" id="shen-me-shi-rum"></a>

本文档提供基于 Electron + Rum SDK 的技术框架，是用于开发 Rum 客户端的解决方案。

### 什么是 ELECTRON <a href="#shen-me-shi-electron" id="shen-me-shi-electron"></a>

[Electron](https://www.electronjs.org/) 是一个使用 JavaScript, HTML 和 CSS 等 Web 技术创建原生程序的框架。

### 什么是 RUM-SDK <a href="#shen-me-shi-rumsdk" id="shen-me-shi-rumsdk"></a>

RUM-SDK 实现了对 RUM 的封装，暴露出了更友好的 api，使基于 Electron 开发的桌面客户端更方便的集成 RUM。

RUM-SDK 包含以下两部份：

1. [quorum-sdk-electron-main](https://github.com/rumsystem/quorum-sdk-electron-main)
2. [quorum-sdk-electron-renderer](https://github.com/rumsystem/quorum-sdk-electron-renderer)

![](https://rumsystem.github.io/rum-docs/rum-sdk/images/rum-sdk.jpg)

**quorum-sdk-electron-main** 用于 Electron 应用的主进程，封装了对 quorum 进程的直接操作，对由 quorum-sdk-electron-render 创建的客户端实例进行响应。

**quorum-sdk-electron-renderer** 用于 Electron 应用的渲染进程，封装了对 quorum-sdk-electron-main 的相关请求，暴露出友好的 api，使得对 quorum 的操作更加直接与易于理解。
