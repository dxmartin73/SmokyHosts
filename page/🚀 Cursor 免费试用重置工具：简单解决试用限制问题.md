# 🚀 Cursor 免费试用重置工具：简单解决试用限制问题

![Cursor Logo](https://camo.githubusercontent.com/496f1515f3e17ce1afe69703f2f708409cf48325a64b654e1788d9e2ea8c17c6/68747470733a2f2f61692d637572736f722e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032342f30392f6c6f676f2d637572736f722d61692d706e672e77656270)

> **⚠️ 重要提示**
> - 本工具支持 **Cursor v0.44.11 及以下版本**  
> - **不支持** 最新的 0.45.x 版本  
> 使用前请确认您的 Cursor 版本。

## 💾 下载 Cursor v0.44.11
- [从 Cursor 官方下载](https://downloader.cursor.sh/builds/250103fqxdt5u9z/windows/nsis/x64)
- [从 ToDesktop 下载](https://download.todesktop.com/230313mzl4w4u92/Cursor%20Setup%200.44.11%20-%20Build%20250103fqxdt5u9z-x64.exe)

## 🔒 禁用自动更新功能
为了防止 Cursor 自动更新到不支持的新版本，建议禁用自动更新功能。

### 方法一：使用内置脚本（推荐）
运行重置工具时，脚本会询问是否禁用自动更新：
bash
[询问] 是否要禁用 Cursor 自动更新功能？
0) 否 - 保持默认设置 (按回车键)
1) 是 - 禁用自动更新

选择 `1` 即可完成操作。

### 方法二：手动禁用
#### **Windows**
1. 关闭所有 Cursor 进程  
2. 删除目录：`%LOCALAPPDATA%\cursor-updater`  
3. 在相同位置创建同名文件（不带扩展名）

#### **macOS**
bash
# 关闭 Cursor
pkill -f "Cursor"
# 删除更新目录并创建阻止文件
rm -rf ~/Library/Application\ Support/cursor-updater
touch ~/Library/Application\ Support/cursor-updater


#### **Linux**
bash
# 关闭 Cursor
pkill -f "Cursor"
# 删除更新目录并创建阻止文件
rm -rf ~/.config/cursor-updater
touch ~/.config/cursor-updater


> **⚠️ 注意**：禁用自动更新后，需手动下载并安装新版本。建议在确认新版本可用后再更新。

## 📝 常见问题与解决方案

### 问题一：试用账号限制
bash
Too many free trial accounts used on this machine.
Please upgrade to pro. We have this limit in place
to prevent abuse. Please let us know if you believe
this is a mistake.


### 问题二：试用请求次数限制
bash
You've reached your trial request limit.


### 临时解决方案
1. 关闭 Cursor 应用  
2. 执行重置机器码脚本（见下方安装说明）  
3. 重新打开 Cursor 即可继续使用

## 🚀 一键解决方案

### **国内用户（推荐）**
#### **macOS**
bash
curl -fsSL https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_mac_id_modifier.sh | sudo bash


#### **Linux**
bash
curl -fsSL https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_linux_id_modifier.sh | sudo bash


#### **Windows**
powershell
irm https://aizaozao.com/accelerate.php/https://raw.githubusercontent.com/yuaotian/go-cursor-help/refs/heads/master/scripts/run/cursor_win_id_modifier.ps1 | iex


### Windows 管理员终端运行方法
1. 按下 `Win + X` 组合键，选择“Windows PowerShell (管理员)”  
2. 在管理员终端中输入上述重置脚本即可。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 🔧 技术细节
- **配置文件**：工具修改 `storage.json` 文件，位于：  
  - Windows: `%APPDATA%\Cursor\User\globalStorage\`  
  - macOS: `~/Library/Application Support/Cursor/User/globalStorage/`  
  - Linux: `~/.config/Cursor/User/globalStorage/`  
- **修改字段**：生成新的唯一标识符，包括 `telemetry.machineId` 等。

## 📄 许可证
本工具基于 **MIT 许可证** 开源，您可以自由使用和修改。

---

如果您在使用过程中遇到其他问题，请参考[官方 GitHub 仓库](https://github.com/yuaotian/go-cursor-help)获取更多帮助。