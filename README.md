<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a0a00,50:3d1a00,100:7c3000&height=240&section=header&text=AgentOS%202.0&fontSize=76&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=50%2B%20Production%20Claude%20Skills%20%E2%80%94%20Finance%20%E2%80%A2%20Engineering%20%E2%80%A2%20Data%20%E2%80%A2%20Research%20%E2%80%A2%20Legal%20%E2%80%A2%20Healthcare&descAlignY=62&descColor=fbbf24&descSize=16" width="100%" />

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=20&pause=1200&color=D97706&center=true&vCenter=true&multiline=false&width=780&height=50&lines=50%2B+specialist+Claude+Skills+across+8+domains;Finance+%E2%80%A2+Engineering+%E2%80%A2+Data+%E2%80%A2+Ops+%E2%80%A2+Legal+%E2%80%A2+Healthcare+%E2%80%A2+Web3;Each+skill+is+a+standalone+SKILL.md+—+drop+in+what+you+need;The+most+depth+per+skill+of+any+Claude+Skills+repo)](https://git.io/typing-svg)

<br/>

<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-d97706?style=for-the-badge&logo=opensourceinitiative&logoColor=white" /></a>
<a href="#skills-index"><img src="https://img.shields.io/badge/Skills-51-92400e?style=for-the-badge&logo=bookstack&logoColor=white" /></a>
<a href="#divisions"><img src="https://img.shields.io/badge/Domains-8-b45309?style=for-the-badge&logo=layers&logoColor=white" /></a>
<img src="https://img.shields.io/badge/Claude-4.x-fbbf24?style=for-the-badge&logo=anthropic&logoColor=black" />
<img src="https://img.shields.io/badge/Format-Claude_Skills-78350f?style=for-the-badge&logo=files&logoColor=white" />
<a href="https://github.com/vignesh2027/Claude-Agentic-Skills2.0-version/stargazers"><img src="https://img.shields.io/github/stars/vignesh2027/Claude-Agentic-Skills2.0-version?style=for-the-badge&logo=starship&color=fbbf24&logoColor=white" /></a>

<br/><br/>

</div>

---

## What Are Claude Skills?

Claude Skills are modular, self-contained instruction packages that extend Claude's behavior in a specific domain. Each skill lives in its own folder with a `SKILL.md` file — a YAML frontmatter block + markdown instructions.

When you load a skill into Claude, it gains that agent's full capabilities: domain knowledge, structured workflows, output formats, and decision logic.

```
your-skill-folder/
└── SKILL.md        ← YAML frontmatter + markdown instructions
    scripts/        ← (optional) executable code
    references/     ← (optional) supplementary docs loaded on demand
    assets/         ← (optional) templates and example files
```

## How to Use a Skill

### Claude.ai (Web)
1. Go to [claude.ai](https://claude.ai) → **Projects** → New Project
2. Open **Project Instructions**
3. Paste the contents of `skill-name/SKILL.md`
4. Every chat in that project uses that skill

### Claude Code (CLI)
```bash
# Add a skill to your project
cat quant-trader/SKILL.md >> .claude/CLAUDE.md

# Or add multiple skills
cat senior-dev/SKILL.md rag-architect/SKILL.md >> .claude/CLAUDE.md
```

### Claude API
```python
import anthropic

with open("quant-trader/SKILL.md") as f:
    skill = f.read()

client = anthropic.Anthropic()
response = client.messages.create(
    model="claude-sonnet-4-6",
    max_tokens=8096,
    system=skill,
    messages=[{"role": "user", "content": "Give me a signal on NVDA"}]
)
```

### Cursor / Windsurf / IDE
Paste the contents of `SKILL.md` into your IDE's AI rules file (`.cursor/rules`, `.windsurfrules`, etc.).

---

## Why AgentOS vs Other Skill Repos?

| Feature | Other Skill Repos | AgentOS 2.0 |
|---------|------------------|-------------|
| Skill depth | Shallow instructions | Full sub-agents, frameworks, output formats |
| Finance skills | None or basic | VaR, DCF, LBO, trade signals, Kelly sizing |
| Engineering skills | Basic prompts | Complete architecture: RAG, multi-agent, MLOps, DevOps |
| Specialized domains | Rare | Healthcare, Real Estate, Insurance, Web3, Biotech, Climate |
| Output formats | Text suggestions | Structured JSON, markdown tables, code templates |
| Framework specificity | General | Named frameworks: STRIDE, COSO ERM, HEDIS, ATT&CK, TCFD |
| Domain count | 2-3 | 8 full domains, 51 skills |
| New agents | N/A | PromptEngineer, StartupAdvisor, PatentAnalyst, BiotechAnalyst, ClimateTech |

---

## Skills Index

### 💹 Finance Division

| Skill | Description |
|-------|-------------|
| [quant-trader](quant-trader/SKILL.md) | Trade signals with JSON output: entry, target, stop, R:R, Kelly sizing, regime detection |
| [cfo-intelligence](cfo-intelligence/SKILL.md) | P&L parsing, 3-statement modeling, variance analysis, board reports, traffic-light KPIs |
| [risk-sentinel](risk-sentinel/SKILL.md) | VaR at 95%/99%, CVaR, Monte Carlo stress testing, ISO 31000 + COSO ERM, risk heat maps |
| [ma-dealmaker](ma-dealmaker/SKILL.md) | DCF, LBO, EV/EBITDA comps, QoE review, synergy modeling, IC memo writing |
| [crypto-sage](crypto-sage/SKILL.md) | On-chain analytics (MVRV, SOPR, NVT), DeFi TVL, tokenomics, rug pull indicators |
| [portfolio-optimizer](portfolio-optimizer/SKILL.md) | MPT efficient frontier, factor exposure (value/momentum/quality), tax-loss harvesting |
| [esg-compass](esg-compass/SKILL.md) | Scope 1/2/3 emissions, 20-metric ESG scoring, TCFD/SFDR compliance, net-zero pathway |
| [compliance-ai](compliance-ai/SKILL.md) | KYC/AML/PEP screening, transaction monitoring, SOX/PCI/GDPR audit prep |

### 🤖 AI & Engineering Division

| Skill | Description |
|-------|-------------|
| [rag-architect](rag-architect/SKILL.md) | Hybrid RAG: semantic chunking, pgvector/Pinecone, BM25 + dense, re-ranking, hallucination detection |
| [agent-smith](agent-smith/SKILL.md) | Multi-agent topology design, semantic routing, tool schema design, memory architecture, eval |
| [senior-dev](senior-dev/SKILL.md) | Complete production code: Next.js 14, FastAPI, TypeScript strict, full error handling, security |
| [data-pipeline-pro](data-pipeline-pro/SKILL.md) | dbt model layers, Airflow DAG design, Spark at scale, data quality validation, Snowflake optimization |
| [mlops-engineer](mlops-engineer/SKILL.md) | MLflow experiment tracking, feature store, drift detection (PSI), A/B model deployment |
| [devops-commander](devops-commander/SKILL.md) | GitHub Actions CI/CD, multi-stage Docker, Kubernetes manifests, Terraform modules, Prometheus alerting |
| [security-chief](security-chief/SKILL.md) | STRIDE threat modeling, OWASP top 10, SIEM log analysis, SOC2/ISO 27001/NIST CSF mapping |
| [api-integrator](api-integrator/SKILL.md) | OpenAPI 3.0 design, OAuth 2.0 flows, HMAC webhook verification, n8n workflow patterns |
| [prompt-engineer](prompt-engineer/SKILL.md) | System prompt design, few-shot examples, chain-of-thought, eval frameworks, injection prevention |

### 📊 Data & Analytics Division

| Skill | Description |
|-------|-------------|
| [data-scientist-pro](data-scientist-pro/SKILL.md) | EDA, feature engineering, model selection, Bayesian hypertuning, SHAP interpretation |
| [timeseries-oracle](timeseries-oracle/SKILL.md) | ARIMA/Prophet/LSTM forecasting, anomaly detection, prediction intervals, scenario planning |
| [business-intelligence-pro](business-intelligence-pro/SKILL.md) | North star metric framework, KPI trees, LookML, SQL window functions, cohort analysis |
| [realtime-data-agent](realtime-data-agent/SKILL.md) | Kafka topic design, Spark Streaming, WebSocket server, event schema, latency budgets |
| [database-genius](database-genius/SKILL.md) | ERD design, composite/partial/covering indexes, EXPLAIN analysis, zero-downtime migration, pgvector |
| [abtest-scientist](abtest-scientist/SKILL.md) | Power analysis, Bayesian/frequentist testing, multiple testing correction, DiD, synthetic control |

### 🏢 Operations Division

| Skill | Description |
|-------|-------------|
| [product-strategy](product-strategy/SKILL.md) | Full PRD writing, RICE scoring, north star metric, LTV/CAC modeling, competitive positioning |
| [sales-intelligence](sales-intelligence/SKILL.md) | ICP scoring, 5-touch outreach sequences, deal health scoring, bottom-up forecasting |
| [marketing-os](marketing-os/SKILL.md) | Keyword clustering, ROAS analysis, AIDA/PAS copywriting, attribution models, brand voice |
| [customer-success](customer-success/SKILL.md) | Churn prediction signals, NPS driver analysis, onboarding sequences, escalation playbooks |
| [legal-eagle](legal-eagle/SKILL.md) | Contract clause extraction, GDPR/CCPA/SOX gaps, NDA review, IP risk — not legal advice |
| [hr-analytics](hr-analytics/SKILL.md) | Attrition prediction, bias-reduced JD writing, comp benchmarking, OKR + performance templates |
| [supply-chain-oracle](supply-chain-oracle/SKILL.md) | Demand forecasting, EOQ + safety stock, ABC analysis, supplier scorecard, disruption stress test |
| [project-command](project-command/SKILL.md) | WBS + milestones, RAID log, sprint velocity, RACI matrix, weekly status reports |

### 📝 Content & Research Division

| Skill | Description |
|-------|-------------|
| [research-intelligence](research-intelligence/SKILL.md) | TAM/SAM/SOM methodology, competitive positioning map, trend identification with evidence |
| [technical-writer-pro](technical-writer-pro/SKILL.md) | GitHub README, OpenAPI docs with code examples, runbook template, wiki architecture |
| [presentation-maestro](presentation-maestro/SKILL.md) | Conflict-resolution narrative arc, per-slide structure, chart selection, BLUF for executives |
| [innovation-catalyst](innovation-catalyst/SKILL.md) | JTBD framework, SCAMPER, BMC all 9 blocks, Blue Ocean, MVP scoping |
| [learning-coach](learning-coach/SKILL.md) | Bloom's taxonomy objectives, Socratic method, spaced repetition, Socratic quiz design |
| [newsletter-engine](newsletter-engine/SKILL.md) | Subject line formulas, 7-email onboarding sequence, referral mechanics, open rate benchmarks |

### 🌐 Specialized Domain Division

| Skill | Description |
|-------|-------------|
| [healthcare-analytics](healthcare-analytics/SKILL.md) | HIPAA-safe analytics, HEDIS measures, LACE readmission index, capacity planning (HIPAA compliant) |
| [real-estate-intelligence](real-estate-intelligence/SKILL.md) | Cap rate, NOI, DSCR, IRR, equity multiple, full CRE due diligence checklist |
| [insurance-actuary](insurance-actuary/SKILL.md) | Loss ratio, combined ratio, chain ladder IBNR, reinsurance treaty design, fraud signals |
| [web3-developer](web3-developer/SKILL.md) | Gas-optimized Solidity, reentrancy/flash loan detection, Foundry fuzz+fork testing, ERC standards |
| [growth-hacking](growth-hacking/SKILL.md) | AARRR funnel, k-factor viral loop, activation aha moment, retention habit loop (Hooked model) |
| [quant-researcher](quant-researcher/SKILL.md) | Hypothesis design, econometric methodology, academic paper structure, Fama-MacBeth, robustness |
| [startup-advisor](startup-advisor/SKILL.md) | Pitch deck review, unit economics health check, fundraising stage strategy, moat analysis |
| [patent-analyst](patent-analyst/SKILL.md) | Prior art search, claim scope analysis, FTO methodology, patent landscape, IP strategy |
| [climate-tech-analyst](climate-tech-analyst/SKILL.md) | GHG Scope 1/2/3, TCFD risk framework, clean energy LCOE, SBTi targets, carbon offset quality |
| [biotech-analyst](biotech-analyst/SKILL.md) | Clinical pipeline PoS, rNPV valuation, FDA expedited programs, competitive indication mapping |
| [cybersecurity-analyst](cybersecurity-analyst/SKILL.md) | MITRE ATT&CK mapping, threat hunting hypotheses, DFIR investigation phases, threat intel reports |
| [supply-chain-optimizer](supply-chain-optimizer/SKILL.md) | Network design optimization, center of gravity model, last-mile cost, digital twin, FTZ compliance |
| [ui-ux-designer](ui-ux-designer/SKILL.md) | Nielsen's 10 heuristics, WCAG 2.1 AA audit, user flow friction scoring, design system specs |

### 🎛 Orchestration

| Skill | Description |
|-------|-------------|
| [agentOS-orchestrator](agentOS-orchestrator/SKILL.md) | Full multi-agent OS: auto-routes tasks to specialists, synthesizes unified outputs — activate all 50+ agents |

---

## Skill Format

Every skill uses the standard Claude Skills format:

```markdown
---
name: skill-name
description: >
  One or two sentences describing when Claude should use this skill and what it does.
  This is used for skill matching and discovery.
license: MIT
---

# Skill Name Agent

[Full instructions for Claude...]
```

The `description` field is critical — it's how Claude matches the right skill to the user's intent.

---

## What Makes These Skills Different

**Depth over breadth.** Each skill includes:
- Named sub-agents with specific responsibilities
- Actual formulas and calculations (not just "analyze the data")
- Decision frameworks with specific criteria
- Output format templates with examples
- Anti-patterns and forbidden behaviors
- Quantitative thresholds (not just "flag if high")

**Example — risk-sentinel:**
Other repos: *"Analyze risks for this portfolio"*
AgentOS: *VaR at 95%/99%, CVaR calculation, ISO 31000 + Basel III + COSO ERM, risk heat map (L×I matrix), top-10 risk register with KRIs, 5 specific stress scenarios (2008 GFC, 2020 COVID, 2022 rate shock...)*

**Example — rag-architect:**
Other repos: *"Help me build a RAG system"*
AgentOS: *512-token semantic chunks with 64-token overlap, hybrid search (70% dense + 30% BM25), cross-encoder re-ranking, hallucination detection via entailment, specific embedding model selection table, complete Python code output*

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

New skills are welcome. Use the [template-skill](template-skill/SKILL.md) as your starting point.

---

## Repository Structure

```
Claude-Agentic-Skills2.0-version/
├── agentOS-orchestrator/     ← Full multi-agent OS (use to get all 50+ agents)
├── quant-trader/             ← Finance: trade signals, Kelly sizing, regimes
├── cfo-intelligence/         ← Finance: P&L, 3-statement model, board reports
├── risk-sentinel/            ← Finance: VaR, CVaR, COSO ERM, stress testing
├── ma-dealmaker/             ← Finance: DCF, LBO, due diligence, IC memos
├── ... (47 more skills)
├── template-skill/           ← Copy this to create a new skill
├── prompts/
│   └── agentOS-system-prompt.md  ← Full OS as a single system prompt (API use)
├── index.html                ← Project website
├── CONTRIBUTING.md
└── README.md
```

---

## License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE).

---

<div align="center">

**Built by [@vignesh2027](https://github.com/vignesh2027)**

*If AgentOS saves you time, a ⭐ star keeps it visible to others.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3000,50:3d1a00,100:1a0a00&height=120&section=footer" width="100%" />

</div>
