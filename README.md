# get-api-docs Skill

一个可独立安装的 [Agent Skill](https://agentskills.io/)，教 AI 在编写第三方代码前自动拉取最新文档，而不是依赖训练数据中的过时知识。

## 为什么建这个仓库

原 skill 内嵌在 [`andrewyng/context-hub`](https://github.com/andrewyng/context-hub) 项目的 `cli/skills/get-api-docs/` 目录中，无法直接作为 skill 仓库一键安装。本仓库将其提取为独立的目录结构，方便用户直接 clone 到任意 agent 的 skills 目录即可使用。

## 安装 Skill

### Kimi Code CLI

```bash
git clone https://github.com/rongxinzy/get-api-docs.git ~/.config/agents/skills/get-api-docs
```

### Claude Code

```bash
git clone https://github.com/rongxinzy/get-api-docs.git ~/.claude/skills/get-api-docs
```

### Codex (OpenAI)

```bash
git clone https://github.com/rongxinzy/get-api-docs.git ~/.codex/skills/get-api-docs
```

### Cursor / 其他 Agent 工具

将本仓库 `SKILL.md` 复制到对应工具的规则或 skills 目录即可。

## 安装 chub CLI（前置依赖）

本 skill 依赖 `chub` CLI 来获取文档：

```bash
npm install -g @aisuite/chub
```

验证安装：

```bash
chub --version
```

更多 CLI 用法请参考 [`andrewyng/context-hub`](https://github.com/andrewyng/context-hub) 的[文档](https://github.com/andrewyng/context-hub/tree/main/cli)。

## 致谢

本 skill 源自 [**andrewyng/context-hub**](https://github.com/andrewyng/context-hub)，由 Andrew Ng 及相关贡献者创建。仅做目录结构提取，方便独立安装，核心内容版权归原作者与原项目贡献者所有。
