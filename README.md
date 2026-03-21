## Hi there 👋

Technical Writer specializing in cloud / API / bilingual documentation.

技术文档工程师，专注云计算、API与中英双语文档。

---

## About Me / 关于我

Technical Writer at ByteDance · Volcengine Cloud. I write API docs, developer guides, and UI documentation. I also build AI-powered tools to improve documentation and localization workflows.

双语技术文档工程师。日常负责 API 文档、开发者文档与 UI 文档编写，同时构建 AI 工具来优化文档与本地化流程。

---

## Projects / 项目展示

### 🔄 [Translation Agent](agent/translation-agent/)

汉译英技术文档翻译 Agent，模拟人类翻译工作流。

An autonomous CN→EN translation agent that mirrors a human translator's workflow.

```
源文本 → TM匹配 → 术语查询 → 初译 → 质检 → 优化(最多3轮) → 交付 + TM回写
Source → TM Match → Term Lookup → Draft → QA → Optimize(up to 3x) → Deliver + TM Writeback
```

- Prompt 分层设计（翻译 / 质检 / 优化）
- 术语表 + TM 库运行时注入
- 人工审校闭环 + TM 自动回写
- Stack: Python · OpenAI API · Prompt Engineering

> **痛点：** 人工逐句翻译效率低，术语不一致，译文质量依赖个人经验，难以规模化复用。
> **解决：** 构建自动化翻译流水线，内置术语表注入、多轮质检与 TM 回写，实现可审计、可迭代的标准化流程。
> **业务价值：** 显著降低人工逐句翻译校对的人力成本，缩短任务交付周期，术语一致性从人工把控升级为系统保障。

---

### 📝 [Doc Generator](agent/doc-generator/)

从非结构化草稿自动生成标准化技术文档。

Generates standardized technical documentation from unstructured drafts.

- 自动提取关键信息（术语、参数、步骤）
- 基于模板生成结构化文档
- 术语表一致性校验
- Stack: Python · LLM API

> **痛点：** 研发提供的输入零散、格式不统一，技术写作者需反复手动整理排版，术语使用因人而异。
> **解决：** 自动提取关键信息并基于模板生成结构化文档，内置术语表校验，一键输出标准化内容。
> **业务价值：** 消除重复排版与术语不一致问题，将非结构化输入到标准文档的产出效率提升数倍。

---

### 📊 [AI QA Workflow Case Study](aceliu451-pixel/case-studies/ai-qa-workflow-case/)

AI 驱动的 MTPE 质检工作流完整案例，从问题定义到落地复盘。

A complete case study of an AI-driven QA workflow for improving MTPE exemption rate.

8-step documentation:

| Step | Content |
|------|---------|
| 01 | Problem Statement — 问题陈述 |
| 02 | Solution Design — 方案设计 |
| 03 | Workflow Architecture — 流程架构 |
| 04 | Prompt Engineering — 提示词工程 |
| 05 | Quality Metrics — 质量指标 |
| 06 | Case Study: Exemption Rate — 免审率案例 |
| 07 | Root Cause Analysis — 根因分析 |
| 08 | Lessons Learned — 经验总结 |

Key result: ~80% post-edit-free rate · 核心成果：约80%免修率

> **痛点：** 人工全量审校成本高、主观性强，难以及时识别高频错误并沉淀可复用的质量规则。
> **解决：** 搭建结构化 AI 质检工作流，将问题定义、流程设计、提示词工程、质量指标与 RCA 串成闭环。
> **业务价值：** 用可复用的 AI 质检机制替代人工全量审校，将免修率提升至 80%，大幅释放审校人力。

---

### 🌐 [MkDocs Portfolio Site](mkdoc/)

基于 MkDocs + GitHub 的 docs-as-code 文档站，包含 API 文档样例与用户指南样例。

Documentation site built with MkDocs, featuring API doc samples and user guide samples.

> **痛点：** 文档散落在本地或 Wiki 中，缺乏版本管理，多人协作时变更难追溯、发布流程不可控。
> **解决：** 基于 MkDocs + GitHub 实现 docs-as-code，文档纳入 Git 版本控制，变更可审查、可回滚。
> **业务价值：** 实现版本可控、协作可追溯的文档发布流程，降低多人协作中的信息丢失与版本冲突风险。

---

## Skills / 技能

**Writing:** API docs · Developer guides · UI docs · Bilingual (ZH/EN)

**AI + Automation:** LLM pipeline design · Prompt engineering · Translation QA · Doc generation

**Tools:** Python · MkDocs · Git/GitHub · TMS

---

## Contact / 联系

📧 ace451@gmail.com
