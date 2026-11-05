# gpt-wechat-bridge

微信与 Codex 的桥接工具，基于 [Gan-Xing/CodexBridge](https://github.com/Gan-Xing/CodexBridge)。

## 安装和启动

需要 Node.js 24 或更高版本，以及已登录的 Codex CLI。

```powershell
npm install
codex login status
npm run weixin:login
npm run weixin:serve -- --cwd C:\path\to\workspace
```

用微信扫描二维码并确认，保持服务运行，然后发送 `/status` 检查连接。

## 微信常用命令

| 命令 | 用途 |
| --- | --- |
| `/helps` | 查看帮助 |
| `/status` | 查看状态 |
| `/models` | 查看可用模型 |
| `/model 1` | 按编号切换模型 |
| `/model default` | 恢复默认模型 |
| `/threads` | 查看会话 |
| `/open 1` | 打开指定会话 |
| `/new` | 创建新会话 |
| `/stop` | 停止当前任务 |
| `/allow` / `/deny` | 批准或拒绝操作 |

更多命令见 [微信命令参考](docs/usage/weixin-slash-commands.md)。
