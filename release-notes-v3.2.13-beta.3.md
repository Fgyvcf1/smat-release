# SmartVillageSystem v3.2.13-beta.3

发布日期：2026-04-30

## 更新内容

- 修复安装版主窗口偶发停留欢迎页、主页面导航不稳定的问题。
- 增强 Tauri 主程序窗口跳转重试机制，首次导航即同步执行 WebView 跳转兜底。
- 增加托盘初始化成功/失败启动日志，方便覆盖安装后定位本机环境问题。
- 保持数据库安全、Recovery Key、备份恢复链路使用 Tauri + Rust 主线。

## 文件

- 安装包：packages/v3.2.13-beta.3/SmartVillageSystem-3.2.13-beta.3-Setup.exe
- SHA256：9CAB6E3FAC8684A999A4DAA06DFD727464D2DBAC27B9DB6EF40F4578320021EB
