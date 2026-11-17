# AzurlaneCN 在线更新源

本仓库是 **碧蓝航线 CN 私服桌面控制台（BelfastConsole）** 的公开自动更新源，**仅存放各版本更新清单（`manifest.json`）与分组件更新包**，不提供源码、完整便携整合包或游戏存档。

## 如何使用（已有整合包的用户）

1. 打开本地桌面控制台 `启动控制台.exe`（或 `BelfastConsole.exe`）并切换到 **「更新」** 页签；
2. 点击 **「检查更新」**，确认列表与更新说明后点击 **「下载并安装」**；
3. 若本次包含控制台自身更新，按提示点击 **「重启控制台」** 即可生效。

- 更新清单地址：`https://github.com/carrotluo5/AzurlaneCN/releases/latest/download/manifest.json`
- 更新前程序会自动校验 SHA-256 与文件大小，并备份旧文件到 `backups/update-*`，失败自动回滚（不会覆盖你的存档 `belfast.db`）。

## 更新包组件说明

| 组件 | 说明 | 更新特点 |
|---|---|---|
| `server` | 服务端 `belfast.exe`（含 CN 兼容补丁与内嵌管理界面） | 需短暂重启服务端，不改动存档 |
| `admin` | GM 管理后台网页与中文语言包 | 热替换静态页面，无需停服 |
| `console` | Windows 桌面控制台单文件程序（`.NET 10` 自包含） | 暂存并在控制台退出后自动替换 |
| `data` | 国服配置数据（当前配套 `CN 9.7.434` / 客户端 `9.7.25`） | 仅覆盖配置文件，不删除自定义数据 |

## 重要说明

- **没有完整包？** 完整绿色便携包（不含存档，解压即可运行）仅在授权的私有仓库分发，本公开仓库不提供整合包与存档文件。
- **使用范围**：本仓库内容仅供个人单机学习研究，游戏相关版权归原厂商所有。

---

> *This public repository only hosts auto-update manifests and component archives for the AzurlaneCN desktop console (`BelfastConsole`). No source code, full portable bundle, or user save data is published here.*
