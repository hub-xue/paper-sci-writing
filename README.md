# Paper Sci Structure

**科研论文结构分析与写作规范** —— 将成熟论文的段落功能解构为可复用的填空式写作模板，用于规范地组织与撰写科研论文初稿。

## 定位

本 skill 将科研论文写作由「逐句从零创作」转化为「解构骨架 → 复用模板 → 填充内容」的结构化流程。核心是解构成熟论文的**段落功能骨架**（而非搬用原文词句），将经同行验证的固定逻辑链条沉淀为可复用的写作模板，再把研究者原创的数据与结论填入，从而高效产出结构完整、逻辑连贯、无明显硬伤的论文初稿。

## 核心能力

- **解构对标范文**：选取 3-5 篇对标论文，仅梳理段落功能、不照搬文字；
- **固定骨架复用**：引言五段、摘要五句、Discussion 三段、Results 每段四句；
- **句式模板库**：过渡句、创新表述、对比论证句按用途分类复用；
- **降重润色**：打断连续 6-7 词重复的五种改写技巧；
- **投稿前质检**：审稿人模拟 + 自查清单；
- **返修 Response**：逐条「改哪里 + 为什么 + 配图」。

## 目录结构

```
paper-sci-structure/
├── SKILL.md                 # 主文件：定位、适用范围、核心原则、工作流程、输入/输出、检查项、示例
├── INSTALL.md               # 发布与安装说明（多 agent 安装方式）
└── references/
    ├── frameworks.md        # 各章节固定骨架、段落功能拆解表、句式模板库、标题命名范式
    └── checklist.md         # 投稿前自查清单、降重技巧、时间规划、Response 规范
```

## 安装

将本仓库克隆或复制到用户级 skill 目录（目录名须为 `paper-sci-structure`）：

```bash
git clone https://github.com/hub-xue/paper-sci-structure.git ~/.workbuddy/skills/paper-sci-structure
```

本 skill 遵循 Agent Skills 开放标准，亦可安装到 codex、dsh、Claude Code、Qoder 等 agent。zip 安装包的命名、版本对应关系与各 agent 的完整安装说明见 [INSTALL.md](./INSTALL.md)。

## 使用前提

- 实验数据、数值计算结果、研究问题均已确定；
- 提供目标期刊/层级、3-5 篇对标范文、本人实验结果与图表。

## 适用范围

方法跨学科通用；面向已具备完整实验数据、需产出学术论文初稿的研究者。

## License

[MIT](./LICENSE)
