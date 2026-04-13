# 智慧村居办公系统发布仓库

当前最新版本：`v3.1.3`

发布日期：2026-04-13

## 下载
- 主程序安装包：[SmartVillageSystem_3.1.3_x64-setup.exe](https://github.com/Fgyvcf1/smat-release/raw/main/packages/v3.1.3/SmartVillageSystem_3.1.3_x64-setup.exe)
- 客户端安装包：[智慧村居办公系统客户端_3.1.3_x64-setup.exe](https://github.com/Fgyvcf1/smat-release/raw/main/packages/v3.1.3/%E6%99%BA%E6%85%A7%E6%9D%91%E5%B1%85%E5%8A%9E%E5%85%AC%E7%B3%BB%E7%BB%9F%E5%AE%A2%E6%88%B7%E7%AB%AF_3.1.3_x64-setup.exe)
- 版本清单：[version.json](https://raw.githubusercontent.com/Fgyvcf1/smat-release/main/version.json)

## 更新内容
- 发布 Tauri/Rust 主程序安装包，支持单机模式与授权后的局域网模式交付。
- 同步发布 Tauri 壳客户端安装包，统一“智慧村居办公系统”品牌文案。
- 修复系统信息中授权状态与运行模式展示不一致的问题。

## 校验信息
- 主程序 SHA256：`3cf0bed2c296143f8ae4cf280fbb2264e50011376e3909db37a89d023247415f`
- 客户端 SHA256：`5a2a59a15005c1b3e3fd74c2526d0500dcb2e8c3a8259b26dd0f65d6d082fdaa`

## 升级说明
- 覆盖安装到原目录时，数据库目录会保留，原有业务数据可继续沿用。
- 已发放授权的机器可继续使用；导入授权文件后即可切换到局域网访问模式。
- 程序内“检查更新”读取本仓库 `version.json`，并跳转到主程序安装包下载地址。
