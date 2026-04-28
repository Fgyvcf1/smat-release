# 智慧村居办公系统发布仓库

当前最新版本：`v3.2.13`

发布日期：2026-04-28

## 下载
- 主程序安装包：[SmartVillageSystem-3.2.13-Setup.exe](https://github.com/Fgyvcf1/smat-release/raw/main/packages/v3.2.13/SmartVillageSystem-3.2.13-Setup.exe)
- 版本清单：[version.json](https://raw.githubusercontent.com/Fgyvcf1/smat-release/main/version.json)

## 更新内容
- 修复角色权限菜单在主程序中不稳定的问题。
- 修复普通管理员登录后被权限守卫误拦、无法进入首页的问题。
- 修复超级管理员菜单被不完整数据库菜单裁剪的问题。
- 完善业务菜单权限标记，确保菜单显示与功能权限一致。

## 校验信息
- 主程序 SHA256：`32262782FD8C3A9ED4230CFE425FDBCB03B7EE31673E41B284F8F0C5684D26A7`

## 升级说明
- 覆盖安装到原目录时，数据库目录会保留，原有业务数据可继续沿用。
- 已发放授权的机器可继续使用；导入授权文件后即可切换到局域网访问模式。
- 程序内“检查更新”读取本仓库 `version.json`，并跳转到主程序安装包下载地址。
