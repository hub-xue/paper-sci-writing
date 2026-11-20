# Paper Sci Structure · Academic Paper Structure Analysis & Writing Convention

**Deconstruct the paragraph-function skeleton of mature papers into reusable fill-in-the-blank templates to organize and draft manuscripts — a zero-dependency, copy-and-use writing-methodology Skill**

[中文 README](./README.md) · [SKILL.md](./SKILL.md) · [Installation](./INSTALL.md) · [Frameworks & Sentence Library](./references/frameworks.md) · [Checklist](./references/checklist.md) · [Citation Patterns](./references/citation-patterns.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## What It Is

Stuck at a blank page, spending days on an introduction that never gets to the point, or a methods/discussion that doesn't connect — most of the time the problem isn't English or the data, it's that **the writing logic isn't sorted out**.

This skill's solution is a single principle:

> **First deconstruct the skeleton of a mature paper, turn it into a fill-in-the-blank form, then fill in your own data.**

It turns the peer-reviewed logical chains — a funnel-style introduction, a reproducible methods section, per-figure quantitative results, and a discussion that interprets mechanisms against the literature — into reusable paragraph templates. Your only job is to fill each paper's own data and conclusions into them accurately.

## Core Capabilities

- **Deconstruct benchmark papers**: pick 3–5 closest papers, map only the function of each paragraph, never copy wording;
- **Reuse fixed skeletons**: five-paragraph introduction, five-sentence abstract, three-part discussion, four-sentence-per-figure results;
- **Sentence-pattern library**: transitions, novelty statements, and comparison sentences classified by purpose for reuse;
- **Paraphrase & polish**: five rewriting techniques to break consecutive 6–7-word repetition;
- **Pre-submission QA**: reviewer simulation + self-check list;
- **Rebuttal Response**: item-by-item "where changed + why + figure".

## Quick Start

### Option 1: Install the Skill directly

Clone or download this repository, place the `paper-sci-structure` directory into your agent's skills directory (the directory name must stay `paper-sci-structure`), then restart or start a new session. See [INSTALL.md](./INSTALL.md) for each agent's directory location.

### Option 2: Download the package

Download `paper-sci-structure-v<version>.zip` from [Releases](https://github.com/hub-xue/paper-sci-structure/releases), unzip it, and place it in the skills directory the same way.

Once installed, tell the AI "help me draft the full skeleton for my paper" or "rewrite this Results section as per-figure quantitative statements", and it will follow this skill's workflow.

## Repository Structure

```
paper-sci-structure/
├── SKILL.md                 # Main file: positioning, scope, principles, workflow, I/O, checks, examples
├── INSTALL.md               # Release & installation guide (multi-agent)
└── references/
    ├── frameworks.md        # Section skeletons, paragraph-function table, sentence library, title patterns
    ├── checklist.md         # Pre-submission checklist, paraphrase techniques, timeline, Response rules
    └── citation-patterns.md # Citation rules: three styles, section density gradient, criteria & examples
```

## Use Cases

- Facing a blank page, scaffold a paper and draft sections from finalized data/results;
- Deconstruct benchmark papers' paragraph functions, organization logic, and writing conventions;
- Apply fixed paragraph/sentence structures to introduction, methods, results, discussion, and abstract;
- Build a sentence-pattern library and apply paraphrase/polish;
- Run a pre-submission reviewer simulation and self-check, or draft a rebuttal Response.

## Prerequisites

- Experimental data, numerical results, and the research question are all finalized;
- Provide the target journal/tier, 3–5 benchmark papers, and your own results and figures.

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

MIT. PRs welcome.
