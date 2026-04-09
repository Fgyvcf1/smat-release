# SmartVillageSystem v3.1.2 技术升级说明

发布日期：2026-04-09

## 1. 架构一致性修复

- `Dashboard.vue` 移除 `@/axios` 直连 HTTP 逻辑
- 统计接口统一改为前端 API 封装层（Tauri invoke -> Rust command）
- 删除图表虚拟回填数据，失败场景仅保留空数据与错误日志

## 2. 版本来源修复

- `SystemInfoDialog.vue` 新增 Tauri 运行时 `getVersion()` 读取逻辑
- 显示版本优先级调整为：`Tauri运行时版本 > runtimeConfig.currentVersion > package.json`
- 解决安装包版本与界面版本分离导致的误判问题

## 3. 发版版本统一

以下文件统一提升到 `3.1.2`：

- `package.json`
- `src-tauri/tauri.conf.json`
- `src-tauri/tauri.main.conf.json`
- `src-tauri/Cargo.toml`
- `src-tauri/Cargo.lock`（根包版本条目）
- `deploy/windows/installer.iss`
- `docs/version.json`

## 4. 验收建议

- 运行 `pnpm run acceptance:migration-gate`，确保迁移门禁继续为 0 残留
- 重新打包并安装后验证：
  - 系统信息版本应为 `v3.1.2`
  - 仪表盘不再出现固定演示数字
  - 居民、低收入、残疾、通知、调解趋势数据与业务页一致
