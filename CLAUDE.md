# CLAUDE.md

## 项目定位

本仓库是一个 **Claude Code 能力演示项目**，包含两层内容：

1. **小丑牌游戏 Demo**（`index.html`）：受 Balatro 启发的纯前端扑克牌游戏 UI，用于展示从 PRD + DESIGN 到可运行代码的完整交付流程。
2. **Claude Code 扩展示例**（`agents/` + `slash/`）：演示如何通过自定义 Agent 和 Slash Command 扩展 Claude Code 的能力。

## 目录约定

```
joker-demo/
├── index.html          # 游戏主页面（纯 HTML/CSS/JS，无构建步骤）
├── PRD.html            # 产品需求文档（HTML 格式）
├── DESIGN.html         # 视觉设计规范（HTML 格式）
├── agents/             # 自定义 Agent 定义文件（.md 格式）
│   ├── fullstack-engineer.md
│   ├── product-manager.md
│   ├── qa-engineer.md
│   └── ui-designer.md
├── slash/              # 自定义 Slash Command 定义文件（.md 格式）
│   ├── cc-commit.md
│   ├── cc-debug.md
│   ├── cc-echo.md
│   ├── cc-explain-error.md
│   ├── cc-explain-this.md
│   ├── cc-init.md
│   ├── cc-plan.md
│   └── cc-ship.md
├── test/               # QA 测试脚本（.mjs 等）
└── test-screenshots/   # QA 截图存放目录（不入版本库）
```

## 常用操作

```bash
# 预览游戏
open index.html

# 预览需求文档
open PRD.html

# 预览设计规范
open DESIGN.html
```

## 注意事项

- 所有代码均为纯静态，无需 Node.js / 构建工具，直接打开 HTML 即可运行。
- `agents/` 和 `slash/` 下的 `.md` 文件是 Claude Code 的配置文件，修改后立即生效。
- `test-screenshots/` 目录已加入 `.gitignore`，截图文件不提交到版本库。
- `test/` 目录存放 QA 测试脚本（.mjs），QA 临时安装的 `node_modules/`、`package.json` 不提交到版本库。
-  产品经理每次更新当前项目的`PRD.html`，ui设计师也是每次更新当前项目的`DESIGN.html` ，而不是新建，一定要使用HTML格式的文档
