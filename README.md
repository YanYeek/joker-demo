# 小丑牌 · Joker Demo

受 Balatro 启发的扑克牌游戏 UI Demo，同时也是一个 **Claude Code 能力演示项目**，展示自定义 Agent 和 Slash Command 的用法。

## 安装

无需安装依赖，纯静态页面。

```bash
git clone <repo-url>
cd joker-demo
```

## 使用

### 运行游戏 Demo

直接用浏览器打开 `index.html`：

```bash
open index.html
```

游戏模拟 Balatro 风格的回合制扑克牌玩法，包含出牌区、手牌区、HUD 信息栏等完整 UI。

### 查看需求与设计文档

- `PRD.html` — 产品需求文档（小丑牌 Web V1.0.0）
- `DESIGN.html` — 视觉设计规范

### Claude Code 自定义扩展

| 目录 | 说明 |
|------|------|
| `agents/` | 自定义 Agent（fullstack-engineer / product-manager / qa-engineer / ui-designer） |
| `slash/` | 自定义 Slash Command（cc-commit / cc-debug / cc-echo 等） |

在 Claude Code 中使用这些扩展时，将 `agents/` 和 `slash/` 目录配置到对应的加载路径即可。
