# 发布与安装说明

本 skill 以 Agent Skills 开放标准（`SKILL.md` + YAML frontmatter）为唯一载体，无编译依赖，一次编写、多 agent 兼容。安装本质是将 `paper-sci-writing/` 目录放入目标 agent 的 skills 目录并保持目录名。

## 1. 发布产物与获取

### 1.1 安装包命名

`paper-sci-writing-v<版本号>.zip`，采用语义化版本（`主.次.修订`），例如 `paper-sci-writing-v1.0.0.zip`。

### 1.2 版本对应关系

| 版本 | 内容 | 说明 |
| --- | --- | --- |
| v1.0.0 | SKILL.md、references/、README.md、LICENSE、INSTALL.md | 初版 |

### 1.3 获取方式

- **GitHub Releases**：在仓库 Releases 页下载对应版本的 zip 安装包；
- **源码**：`git clone https://github.com/hub-xue/paper-sci-writing.git`。

## 2. 通用安装流程

各 agent 安装本质相同，仅 skills 目录位置不同：

1. 下载 zip 并解压，得到 `paper-sci-writing/` 目录；
2. 放入目标 agent 的 skills 目录（见 3.1 对照表）；
3. 目录名保持 `paper-sci-writing`（须与 SKILL.md 的 `name` 一致）；
4. 重启或新建会话使其生效；
5. 按 3.3 验证。

## 3. 各 agent 安装

### 3.1 skills 目录对照表

| agent | 用户级目录 | 工程级目录 | 备注 |
| --- | --- | --- | --- |
| WorkBuddy | `~/.workbuddy/skills/` | `.workbuddy/skills/` | 原生支持 |
| Claude（Claude Code） | `~/.claude/skills/` | `.claude/skills/` | 可用 `CLAUDE_CONFIG_DIR` 覆盖 |
| codex（OpenAI Codex） | `~/.codex/skills/` | `.agents/skills/` | 工程级读通用目录 |
| dsh（DeepSeek Harness） | `~/.dsh/skills/` 或 `~/.agents/skills/` | `.dsh/skills/` 或 `.agents/skills/` | 原生实现 Skills 规范 |
| qder（Qoder） | `~/.qoder/skills/` | 以官方文档为准 | 亦识别通用目录 `.agents/skills/` |

> 目录整理自 Agent Skills 生态公开文档，请以各 agent 官方文档为准。通用目录 `.agents/skills/` 被 codex、Cursor、Gemini、dsh 等多个 agent 识别，可一次安装、多处复用。

### 3.2 安装要素表

| agent | 适用环境 | 前置依赖 | 安装步骤 | 配置要点 | 验证方法 |
| --- | --- | --- | --- | --- | --- |
| WorkBuddy | WorkBuddy 桌面端 / IDE | 原生支持，无额外依赖 | 解压放入 `~/.workbuddy/skills/` → 重启 | 目录名保持 `paper-sci-writing` | 触发论文结构类指令，确认被调用 |
| Claude（Claude Code） | Claude Code / 支持 SKILL.md 的 Claude 环境 | 支持 Skills 机制 | 解压放入 `~/.claude/skills/` → 重启会话 | 目录名保持；可设 `CLAUDE_CONFIG_DIR` | 输入 `/` 或询问"有哪些 skills"确认 |
| codex（OpenAI Codex） | OpenAI Codex CLI | 支持 Skills 机制 | 解压放入 `~/.codex/skills/`（个人）或 `.agents/skills/`（工程）→ 重启 | 目录名保持；可设 `CODEX_HOME` | 发起相关任务确认被识别 |
| dsh（DeepSeek Harness） | DeepSeek Harness | 原生实现 Skills 规范 | 解压放入 `~/.dsh/skills/` 或 `~/.agents/skills/` → 重启 | 目录名保持；可设 `DSH_HOME` | 发起相关任务确认被识别 |
| qder（Qoder） | Qoder | 支持 Skills 机制（待核实） | 解压放入 `~/.qoder/skills/` → 重启 | 目录名保持 | 发起相关任务确认被识别 |

### 3.3 验证方法

安装后统一验证：对目标 agent 发起一个论文结构相关请求（如"帮我解构论文骨架""按 IMRaD 结构组织论文"），若 agent 依据本 skill 的工作流程执行即安装成功；也可直接询问该 agent"当前有哪些 skills 可用"确认是否被识别。

## 4. 注意事项

- 目录名必须为 `paper-sci-writing`，与 SKILL.md 的 `name` 不一致可能导致无法被正确识别；
- 同一份 skill 可由多个 agent 通过软链接复用（以 `.agents/skills/` 为源，各 agent 目录做链接）；
- 本 skill 仅含 Markdown 文档，无脚本，安装后无需额外初始化。
