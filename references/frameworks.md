# 各章节固定骨架与句式素材库

## 来源说明

本文档综合四类来源：两篇写作经验帖的共识与独特要点，以及两篇实证论文（SHDMS-ABC《Results in Engineering》、QAE-ABC《Ocean Engineering》）的标题、摘要与引言实证样例。标注【两篇共识】为经验帖双方一致，【文1】为"半年 4 篇一区"帖独有，【文2】为"2 周写完 SCI"帖独有，【实证】为两篇参考论文归纳所得；未标注处为对原文表述的忠实转述，不添加原文未提及的信息。

## 1. 标题命名范式【实证】

两篇参考论文的标题均遵循"方法 + 任务 + 应用对象/领域"的三段式，方法名以 `-ABC`（Artificial Bee Colony）结尾，核心任务以动名词短语表达，用 `for` 连接任务与对象：

- `A dynamic multi-strategy algorithm for train headway optimization in intercity railways`
  （模式：`A + [修饰] + [方法类型] + for + [任务动名词] + in + [领域]`）
- `QAE-ABC: Quantum amplitude estimation-assisted reliability-constrained member sizing for fixed-base offshore wind turbine jackets`
  （模式：`[缩写]: [核心技术短语] + [任务] + for + [具体对象]`）

可复用规律：标题须同时交代**方法命名**与**核心任务**；任务用动名词短语（optimization、member sizing）；以 `for` 引出应用对象或领域。

## 2. 段落功能拆解表（阶段 0 产物）

| 章节 | 范文段落安排 | 我的写作内容 |
| --- | --- | --- |
| 引言第一段 | 阐述领域研究价值 | 替换为自己研究领域的行业背景 |
| 引言第二、三段 | 梳理现有研究 + 界定研究空白 | 改写为本领域文献综述，提炼未被解决的痛点 |
| 方法章节 | 实验条件、变量设置、操作流程 | 如实填入自己的实验参数、设备与方案 |
| 结果与讨论 | 按研究问题依次展示数据、对照文献解释机理 | 依托自身实验数据绘图，逐条分析规律 |

核心原则：仅复用段落逻辑链条，不照搬句子。引言"漏斗式"由大到小；方法"可复现"；结果"逐图定量陈述"。

## 3. 引言固定骨架

【两篇共识】引言由大到小（漏斗式）；本质只做三件事：确立领域 → 界定空白 → 占据空白（CARS 模型）。

【文1】固定五段：
1. 大背景（一两句）
2. 现有研究进展（不堆文献，仅提炼核心结论）
3. 界定研究空白（关键——空白必须真实，伪空白审稿人一眼看穿）
4. 提出解决方法
5. 陈述核心贡献

【实证】引言结尾三段固定句式：
- 界定空白：`Despite advances …, several challenges remain. First, … Second, … Third, …`
- 提出方法：`To address these challenges, this paper proposes …`
- 列举贡献：`The main contributions … are summarized as follows: (1) … (2) … (3) …`
- 章节预告：`The remainder of this paper is organized as follows. Section 2 … Section 3 …`

【文2】引言"换主语、换研究场景，保留逻辑链"示例：
- 原文：In 2020, Zhang et al. proposed a CNN-based method for image classification.
- 改写：In 2023, Li et al. introduced a Transformer-based approach for text sentiment analysis.

背景递进、提出短板、引出研究目标的句式完全保留，仅更换研究对象、文献与时间线。

## 4. 摘要固定五句【文1】

背景 → 方法 → 数据 → 结果 → 意义。先填入 Results 中最具分量的量化结果再倒推。摘要是全文贡献的精炼定位，而非全文压缩。

【实证】摘要内部次序：①问题与挑战 → ②`This study develops …` 方法定位 → ③主案例量化结果（精确数字与百分比）→ ④对比/消融验证 → ⑤泛化与总结定位。量化结果须附基线（如 `a 20.29% reduction from the 673.88 t baseline`）与评估预算（如 `6,600 objective-function evaluations`）。

## 5. Discussion 三段式【文1】

1. 总结核心发现（换表述重述，不复制 Results）
2. 解释机制、对照文献（与谁一致、与谁冲突、原因）
3. 主动披露局限（样本量、单中心、回顾性偏倚等，先行说明）

【文2】讨论套用对比论证模板：本研究得到 X 规律，与前人 Y 的研究结论一致/存在差异，产生分歧的核心原因是 Z。先用现象描述结果，再深挖内在机理，避免写成单纯的实验报告。

## 6. Results 四句法【文1】

一张图对应一段，每段固定四句：
1. 总起句（概括发现）
2. 具体数据（均值 ± 标准差）
3. 统计结果（p 值或效应量）
4. 定位句（呼应假设）

不解释原因、不引文献，仅陈述观测结果。

## 7. Methods 可复现要素

【两篇共识】唯一标准：可据以复现。写全：样本量、分组、设备型号、统计软件版本、显著性标准。不在方法章节叙事或炫耀。

【文2】章节层级沿用范文：实验材料 → 仪器参数 → 试验设计 → 数据处理。流程图结构不变，仅重命名模块（如 Attention Module → Focus Module，Feature Fusion → Information Aggregation），句式不变，仅替换公式符号与实验参数。

## 8. 句式模板库【文2】

按用途分类摘录范文句式，后续写作仅替换研究内容：

- 界定研究空白：To the best of our knowledge, few studies have focused on…
- 阐述实验结论：The experimental results demonstrate that…
- 对比前人成果：This finding is consistent with the conclusion of…

素材来源：范文中的过渡句、创新表述、对比论证句。
