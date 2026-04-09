# SmartVillageSystem v3.1.2

发布日期：2026-04-09

## 本版定位

这是一个稳定性修复版本，重点解决安装后版本显示不一致和仪表盘展示虚拟数据的问题，确保迁移后数据来源一致、结果可复核。

## 本次包含的内容

- 修复“系统信息”版本显示：优先读取 Tauri 运行时版本，避免与安装包版本不一致
- 修复仪表盘统计数据来源：移除旧 Node HTTP 调用，改为读取已迁移的 Rust/Tauri 接口
- 取消仪表盘虚拟兜底数据，接口失败时显示真实空态而非演示数字
- 统一发版版本号为 `v3.1.2`（package、Tauri、Cargo、安装脚本、version.json）

## 升级说明

- 请直接覆盖安装到原目录（例如 `D:\SmartVillageSystem`），保留数据目录可继续沿用历史数据
- 升级后“系统信息”显示版本应为 `v3.1.2`
- 升级后仪表盘统计来自真实业务数据，不再显示固定演示值

## 发布清单

- 版本清单：`docs/version.json`
- 安装包文件名：`SmartVillageSystem-3.1.2-Setup.exe`
- 下载地址：`https://github.com/Fgyvcf1/smat-release/releases/download/v3.1.2/SmartVillageSystem-3.1.2-Setup.exe`
