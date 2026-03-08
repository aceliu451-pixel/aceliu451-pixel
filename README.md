## Hi there 👋

# AI 本地化与技术文档作品集
# AI Localization & Technical Documentation Portfolio

**刘 [姓名]** · 本地化工程师 / 技术文档工程师  
**Liu [Name]** · Localization Engineer / Technical Writer  
📍 北京 / 上海 · 📧 your.email@gmail.com

---

## 我做什么 / What I Do

我构建 **AI驱动的本地化质量体系**，服务于云计算产品文档（中译英）——不是简单翻译，而是工程化的质量管理系统。

I build **AI-powered localization systems** for cloud product documentation (CN→EN) — engineered for measurable quality, not just translated.

核心方向：中译英技术文档 · LLM流水线设计 · 翻译质量工程 · 技术写作 · UI文案治理

Core work: CN→EN localization · LLM pipeline design · Translation QA engineering · Technical writing · UI copy governance

---

## 核心项目 / Featured Project

### [localization-agent](https://github.com/[username]/localization-agent) — AI 本地化流水线 / AI Localization Pipeline

将手工中译英本地化流程升级为**可度量、可自动化的AI质量体系**，覆盖云计算产品文档与控制台UI文案。

A 5-node LLM pipeline that transforms manual CN→EN localization into a measurable, automated quality system for cloud technical documentation and UI copy.

**流水线架构 / Pipeline**

```
源文本 CN → 实体分析 → 直译 → 逻辑重构 → 风格应用 → 质量检测 → 最终译文 + QA报告
Source CN → Analyzer → Translator → Refactor → Style → QA Guard → Final EN + QA Report
```

**成果指标 / Results**

| 指标 / Metric | 结果 / Result |
|---|---|
| 免修率 · Post-edit-free rate | ~80% |
| 人工审校吞吐量 · Human review throughput | ~900 字/小时 · chars/hr |
| 术语类QA问题减少 · Terminology QA failures reduced | ~40% |
| 流水线节点数 · Pipeline nodes | 5 |

**关键工程决策 / Key Engineering Decisions**

- **节点级Prompt模板** — 每个节点独立的 `.md` 模板，独立版本控制，而非一个超长Prompt  
  One prompt template per node, independently versioned — not a single mega-prompt
- **运行时术语库注入** — `config/termbase.json` 热替换，无需修改代码  
  Runtime termbase injection via `config/termbase.json` — hot-swappable without code changes
- **JSON状态对象** — 完整中间链路记录，不依赖LLM短期记忆  
  JSON state object carries full intermediate trace — no LLM memory dependency
- **节点级温度调优** — QA节点 `0.0` 保证确定性，重构节点 `0.2` 保留弹性  
  Per-node temperature tuning (QA at `0.0` for determinism, refactor at `0.2`)
- **生产级健壮性** — 自动重试（3次）+ JSON解析容错  
  Retry logic (3×) + JSON parse fallback for production resilience

**技术栈 / Stack:** Python · DeepSeek API · Prompt Engineering · JSON

---

## 能力范围 / Capability Areas

**本地化质量工程 / Localization Quality Engineering**  
本地化QA（LQA）· 机器翻译后编辑（MTPE）· 免修率追踪 · 根因分析（RCA）· 错误分类体系设计 · 术语一致性管理  
LQA · MTPE · Post-edit-free rate tracking · Root cause analysis (RCA) · Error taxonomy · Terminology management

**AI与流水线 / AI & Pipeline**  
LLM API集成 · 多步Prompt链路设计 · 多节点流水线编排 · 质量指标设计 · 自动化风险标注  
LLM API integration · Prompt chain design · Multi-node pipeline orchestration · Quality metric design · Automated risk flagging

**技术文档 / Technical Documentation**  
云计算产品中译英文档 · API文档 · UI文案 · 帮助中心 · 发布说明 · 风格规范应用  
CN→EN cloud docs · API documentation · UI copy · Help center · Release notes · Style guide application

**工具 / Tools**  
Python · DeepSeek / OpenAI API · Git · TMS平台 · VS Code

---

## 质量框架 / QA Framework

翻译错误按三类分类，每类错误驱动对应的Prompt迭代方向：

Translation errors are classified into three categories, each driving specific prompt iteration:

| 错误类型 / Error Type | 定义 / Definition | 修复方案 / Fix Applied |
|---|---|---|
| 术语错误 · Terminology | 领域术语翻译错误 · Wrong domain term | 术语库注入 + 重构节点强制执行 · Termbase injection + refactor enforcement |
| 格式错误 · UI Format | 大小写/标点违规 · Capitalization / punctuation violations | 风格节点规则：句首大写，标签无标点 · Style node: sentence case, no period on labels |
| 语义错误 · Semantic | 含义改变或主宾倒置 · Meaning changed or subject inverted | 分析节点标注实体类型 → 重构节点结构化修复 · Analyzer flags entity → refactor restructures |

完整根因分析样本与QA案例详见案例文档，可按需提供。  
Full RCA samples and QA case studies available in the case study document — contact to request.

---

## 知识库资产 / Knowledge Base Assets

**动态术语库 / Terminology Database** — JSON格式，运行时注入，无需人工干预即可保障术语一致性  
Dynamic JSON, runtime-injected, enforces consistency without manual review

**高频句式库 / Sentence Pattern Library** — 中译英技术文档高频表达，对标AWS等云厂商规范  
High-frequency CN→EN technical expressions aligned to AWS / cloud vendor standards

**Prompt规则集 / Prompt Rule Set** — 5条核心约束规则，每条针对一类高频错误，源自真实RCA积累  
5 core constraint rules derived from RCA, each targeting a specific recurring error class

---

## 联系方式 / Contact

📧 your.email@gmail.com  
完整案例文档（流水线架构 · QA框架 · 根因分析样本 · 知识库）可按需提供。  
Full case study document (pipeline architecture · QA framework · RCA samples · knowledge base) available on request.
