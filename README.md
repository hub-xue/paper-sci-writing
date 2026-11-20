# Paper Sci Structure · 科研论文结构分析与写作规范

**将成熟论文的段落功能解构为可复用的填空式写作模板，用于规范地组织与撰写科研论文初稿 —— 一个零依赖、复制即用的写作方法论 Skill**

[SKILL.md](./SKILL.md) · [安装说明](./INSTALL.md) · [段落骨架与句式库](./references/frameworks.md) · [自查清单](./references/checklist.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 这是什么

写论文卡在空白文档、引言写三天进不了正题、方法和讨论前后脱节——多数时候不是英文差、也不是数据不够，而是**写作逻辑没理顺**。

本 skill 的解法只有一条：

> **先拆成熟论文的骨架，把它变成填空题，再填进你自己的数据。**

把经过同行验证的固定逻辑链条（引言「漏斗式」、方法「可复现」、结果「逐图定量陈述」、讨论「对照文献解释机理」）沉淀为可复用的段落模板，你只负责把每篇论文特有的数据与结论准确填入。

## 核心能力

- **解构对标范文**：选取 3-5 篇对标论文，仅梳理段落功能、不照搬文字；
- **固定骨架复用**：引言五段、摘要五句、Discussion 三段、Results 每段四句；
- **句式模板库**：过渡句、创新表述、对比论证句按用途分类复用；
- **降重润色**：打断连续 6-7 词重复的五种改写技巧；
- **投稿前质检**：审稿人模拟 + 自查清单；
- **返修 Response**：逐条「改哪里 + 为什么 + 配图」。

## 快速开始

### 方式一：直接安装 Skill

将本仓库克隆或下载后，把 `paper-sci-structure` 目录放入你所使用 agent 的 skills 目录（目录名须保持 `paper-sci-structure`），重启或新建会话即可。各 agent 的目录位置见 [INSTALL.md](./INSTALL.md)。

### 方式二：下载安装包

在 [Releases](https://github.com/hub-xue/paper-sci-structure/releases) 下载 `paper-sci-structure-v<版本号>.zip`，解压后按同样方式放入 skills 目录。

安装后对 AI 说「帮我按论文框架搭全文骨架」「把这段 Results 改成逐图定量陈述」，它会按本 skill 的流程工作。

## 目录结构

```
paper-sci-structure/
├── SKILL.md                 # 主文件：定位、适用范围、核心原则、工作流程、输入/输出、检查项、示例
├── INSTALL.md               # 发布与安装说明（多 agent 安装方式）
└── references/
    ├── frameworks.md        # 各章节固定骨架、段落功能拆解表、句式模板库、标题命名范式
    └── checklist.md         # 投稿前自查清单、降重技巧、时间规划、Response 规范
```

## 适用场景

- 面对空白文档，为已确定的数据/结果搭建论文骨架并起草各章节；
- 解构对标论文的段落功能、组织逻辑与写作范式；
- 为引言、方法、结果、讨论、摘要套用固定段落/句式结构；
- 搭建句式模板库、实施降重润色；
- 投稿前审稿人模拟与自查，或起草返修 Response。

## 使用前提

- 实验数据、数值计算结果、研究问题均已确定；
- 提供目标期刊/层级、3-5 篇对标范文、本人实验结果与图表。

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

MIT。欢迎 PR，欢迎转发给你的同门。
