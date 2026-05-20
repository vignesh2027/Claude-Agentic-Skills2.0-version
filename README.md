<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a0a00,50:3d1a00,100:7c3000&height=240&section=header&text=AgentOS%202.0&fontSize=76&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=The%20World%27s%20Most%20Advanced%20Multi-Agent%20AI%20Operating%20System&descAlignY=62&descColor=fbbf24&descSize=18" width="100%" />

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=20&pause=1200&color=D97706&center=true&vCenter=true&multiline=false&width=780&height=50&lines=40%2B+Specialized+AI+Agents+in+One+System+Prompt;Finance+%E2%80%A2+Engineering+%E2%80%A2+Data+%E2%80%A2+Operations+%E2%80%A2+Legal+%E2%80%A2+Research;Not+a+chatbot.+An+institutional-grade+AI+workforce.;Drop+in.+Orchestrate.+Execute+at+depth.)](https://git.io/typing-svg)

<br/>

<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-d97706?style=for-the-badge&logo=opensourceinitiative&logoColor=white" /></a>
<a href="agents/"><img src="https://img.shields.io/badge/Agents-40%2B-92400e?style=for-the-badge&logo=robot&logoColor=white" /></a>
<a href="skills/"><img src="https://img.shields.io/badge/Skills-100%2B-b45309?style=for-the-badge&logo=bookstack&logoColor=white" /></a>
<a href="agents/"><img src="https://img.shields.io/badge/Divisions-8-78350f?style=for-the-badge&logo=layers&logoColor=white" /></a>
<img src="https://img.shields.io/badge/Built_for-Claude_4.x-fbbf24?style=for-the-badge&logo=anthropic&logoColor=black" />
<a href="https://github.com/vignesh2027/Claude-Agentic-Skills2.0-version/stargazers"><img src="https://img.shields.io/github/stars/vignesh2027/Claude-Agentic-Skills2.0-version?style=for-the-badge&logo=starship&color=fbbf24&logoColor=white" /></a>

<br/><br/>

**One system prompt. 40+ specialists. Institutional-grade output.**

</div>

---

## What Is AgentOS?

AgentOS is a **complete multi-agent AI operating system** encoded as a single Claude system prompt. Drop it into Claude and you get an intelligent orchestrator that automatically:

1. **Identifies** which agent(s) your task needs
2. **Decomposes** the work into focused sub-tasks
3. **Routes** each sub-task to the right specialist
4. **Executes** with full domain depth — no hand-waving
5. **Synthesizes** everything into one unified output
6. **Delivers** in the exact format you need

```
Your Task
    │
    ▼
╔══════════════════════════════════════════════════╗
║            AgentOS Orchestrator                  ║
║  IDENTIFY → DECOMPOSE → ROUTE → EXECUTE → SYNTH  ║
╚══════════════════════════════════════════════════╝
    │            │            │            │
    ▼            ▼            ▼            ▼
QuantTrader  CFO-Intel    SeniorDev   DataScientist
 Finance      Finance    Engineering     Data
```

Every response starts with an activation announcement, ends with confidence level and next steps — and always includes a complete output, never a partial one.

---

## Quick Start

**60 seconds to activate.**

### Claude.ai Projects (Recommended)
```
1. Go to claude.ai → Create a New Project
2. Open "Project Instructions"
3. Paste contents of prompts/agentOS-system-prompt.md
4. Every chat in that project is now AgentOS
```

### Claude Code CLI
```bash
cat prompts/agentOS-system-prompt.md >> ~/.claude/CLAUDE.md
```

### Anthropic API (Python)
```python
import anthropic

with open("prompts/agentOS-system-prompt.md") as f:
    system_prompt = f.read()

client = anthropic.Anthropic()
response = client.messages.create(
    model="claude-sonnet-4-6",
    max_tokens=8096,
    system=system_prompt,
    messages=[{"role": "user", "content": "Analyze Q4 earnings and give me a trade signal"}]
)
```

### Cursor / Windsurf / IDE Rules
Paste the contents of `prompts/agentOS-system-prompt.md` into your IDE's AI custom instructions or rules file.

---

## 8 Divisions · 40+ Agents

### 💹 Finance Division — 8 Agents

| Agent | What It Does |
|-------|-------------|
| **QuantTrader** | Generates buy/sell signals with entry/target/stop/R:R. Kelly sizing. Regime detection (trending/ranging/volatile). Outputs structured JSON trade signals. |
| **CFO-Intelligence** | Parses P&L, balance sheet, cash flow from any format. 3-statement financial models. Budget vs actual variance with root cause. Board-ready executive summaries. |
| **RiskSentinel** | VaR at 95%/99%, CVaR, Monte Carlo stress testing. Applies ISO 31000 + Basel III + COSO ERM. Outputs risk heat map + top-10 risk register + KRIs. |
| **M&A DealMaker** | DCF, EV/EBITDA, LBO, precedent transaction analysis. Red flag detection, quality of earnings review. Synergy modeling and deal memo generation. |
| **CryptoSage** | On-chain analytics: MVRV, SOPR, NVT, whale flows. DeFi TVL trends, yield farming APYs. Tokenomics vesting/unlock impact. Rug pull indicators. |
| **PortfolioOptimizer** | MPT efficient frontier, factor exposure (value/momentum/quality/low-vol). Drift-based rebalance signals. Tax-loss harvesting and lot selection. |
| **ESG-Compass** | Scope 1/2/3 emissions, ESG scoring vs 20+ metrics. TCFD, SFDR, SEC climate disclosure gap analysis. Net-zero roadmap prioritization. |
| **ComplianceAI** | KYC/AML transaction monitoring, PEP screening. Filing deadline calendar. SOX/PCI/GDPR audit prep and control documentation. |

### 🤖 AI & Engineering Division — 8 Agents

| Agent | What It Does |
|-------|-------------|
| **RAG-Architect** | End-to-end RAG: semantic chunking (512 tokens, 64 overlap), embedding selection, pgvector/Pinecone setup, hybrid search (70% dense + 30% BM25), cross-encoder re-ranking, hallucination detection. |
| **AgentSmith** | Multi-agent system architecture: hierarchical/parallel/sequential topologies. Semantic routing, tool schema design, memory layers (short/long/episodic), eval frameworks. |
| **SeniorDev** | Complete production code only — never partial. TypeScript strict, async/await, full error handling, env vars for secrets, OWASP security, structured logging. Next.js 14 + FastAPI + PostgreSQL + Redis. |
| **DataPipeline-Pro** | ETL/ELT pipeline design. dbt transformation models with tests. Airflow/Prefect DAG design. Spark at scale. Data quality validation, freshness checks, anomaly detection. |
| **MLOps-Engineer** | MLflow experiment tracking, feature store design, leakage detection. Docker/K8s model serving. Data drift + concept drift monitoring. A/B model deployment with shadow mode. |
| **DevOps-Commander** | GitHub Actions CI/CD pipelines. Multi-service Docker Compose and Kubernetes manifests. Terraform/Pulumi IaC. Prometheus + Grafana monitoring setup with alerting rules. |
| **SecurityChief** | STRIDE threat modeling for any architecture. OWASP top 10 analysis. Log analysis patterns and SIEM triage. Incident response playbooks. SOC2/ISO 27001/NIST CSF control mapping. |
| **APIIntegrator** | OpenAPI 3.0 schema-first design. OAuth 2.0, JWT, API key patterns. Webhook retry logic with HMAC signature verification. n8n/Zapier workflow design. Auto-SDK generation. |

### 📊 Data & Analytics Division — 6 Agents

| Agent | What It Does |
|-------|-------------|
| **DataScientist-Pro** | EDA, distribution analysis, outlier detection. Feature selection with correlation + importance. Model selection + Bayesian hyperparameter tuning. SHAP + business translation. |
| **TimeSeriesOracle** | Trend/seasonality/residual decomposition. ARIMA, Prophet, LSTM, ensemble forecasting. Isolation Forest + DBSCAN anomaly detection. Prediction intervals and scenario planning. |
| **BusinessIntelligence-Pro** | North star metric + metric tree design. LookML + Looker explore architecture. Window functions, CTEs, complex query optimization. Threshold-based and ML alerting logic. |
| **RealtimeDataAgent** | Kafka/Kinesis topic design with partition strategy. Flink/Spark Streaming transformations. WebSocket server implementation. End-to-end latency analysis and optimization. |
| **DatabaseGenius** | Normalization vs denormalization decisions. Composite, partial, covering index strategy. EXPLAIN plan analysis, N+1 elimination. Zero-downtime migration planning. pgvector for AI workloads. |
| **ABTest-Scientist** | Sample size + power analysis. t-test, chi-square, Bayesian analysis. Multiple testing correction (Bonferroni/BH). Difference-in-Differences and synthetic control. Statistical vs practical significance. |

### 🏢 Operations Division — 8 Agents

| Agent | What It Does |
|-------|-------------|
| **ProductStrategy-Agent** | Full PRD writing. RICE scoring, MoSCoW, impact/effort matrix. User interview guides. Funnel analysis, cohort retention, LTV/CAC modeling. Competitive feature matrices. |
| **SalesIntelligence** | ICP scoring with firmographic + intent signals. Personalized cold outreach sequences. Deal health scoring, stall detection, win probability. Bottom-up sales forecast. |
| **MarketingOS** | Keyword research, search intent mapping, content gap analysis. ROAS analysis, multi-touch attribution. Conversion-focused copy (AIDA, PAS, StoryBrand). Campaign budget optimization. |
| **CustomerSuccess-Agent** | Intent classification and routing. Churn prediction using behavioral signals. Onboarding sequence design. NPS driver analysis. Escalation with full context handoff. |
| **LegalEagle** | Contract clause extraction and risk flagging. GDPR/CCPA/SOX/HIPAA compliance gaps. NDA scope, duration, and mutuality review. IP ownership and licensing risk. ⚠️ Not legal advice — consult a licensed attorney. |
| **HRAnalytics-Agent** | JD writing with bias reduction. Flight risk and attrition driver modeling. Salary benchmarking. OKR writing, feedback templates. Engagement survey design. |
| **SupplyChain-Oracle** | Seasonal demand forecasting, safety stock calculation. EOQ, reorder points, ABC analysis. Supplier scorecard, concentration risk, alternative sourcing. Supply chain stress testing. |
| **ProjectCommand** | WBS, milestone definition, critical path. RAID log (Risks/Assumptions/Issues/Dependencies). Sprint planning, velocity tracking. RACI matrix, communication plan, status reports. |

### 📝 Content & Research Division — 6 Agents

| Agent | What It Does |
|-------|-------------|
| **ResearchIntelligence** | TAM/SAM/SOM market sizing. Competitive feature matrix and SWOT. Macro + micro trend identification with evidence. Academic paper synthesis. Strategic insight generation. |
| **TechnicalWriter-Pro** | GitHub README with badges and examples. OpenAPI endpoint docs with code samples. Operational runbooks with step-by-step procedures. Knowledge base architecture. |
| **PresentationMaestro** | Narrative arc and slide flow design. Data-to-chart selection. Executive summary distillation (3-5 key messages). Per-slide: headline, body, chart, speaker notes. |
| **InnovationCatalyst** | Market gap analysis, JTBD framework. SCAMPER and Blue Ocean strategy. Business Model Canvas (all 9 blocks). MVP feature scoping and go-to-market planning. |
| **LearningCoach** | Socratic teaching method. Learning objectives and module structure. Visual concept maps. Formative assessments with explanations. Knowledge gap identification. |
| **NewsletterEngine** | Content curation and angle finding. A/B-tested subject lines with power words. Welcome → nurture → re-engagement sequences. Open rate and CTR root cause analysis. |

### 🌐 Specialized Domain Agents — 6+ Agents

| Agent | What It Does |
|-------|-------------|
| **HealthcareAnalytics** | HIPAA-safe outcomes analysis. HEDIS measures, CMS star ratings. Readmission risk scoring, length-of-stay modeling. Capacity planning and staff scheduling. |
| **RealEstateIntelligence** | Cap rate, NOI, DCF, comp analysis. Supply/demand dynamics, rental trend modeling. Debt service coverage, IRR, equity multiple underwriting. Due diligence checklist: title, zoning, environmental, tenant. |
| **InsuranceActuary** | Premium calculation, loss ratio modeling. IBNR reserves and claims development triangles. Fraud detection signal patterns. Treaty reinsurance design and attachment point optimization. |
| **Web3-DeveloperAgent** | Gas-optimized Solidity smart contracts. AMM, lending protocol, yield vault architecture. Reentrancy, overflow, flash loan attack detection. Hardhat/Foundry test suites with fork testing. |
| **GrowthHacking-Agent** | AARRR funnel optimization. k-factor calculation, referral loop design. Time-to-value optimization, aha moment identification. Highest-ROI acquisition channel identification. |
| **QuantResearcher** | Testable hypothesis formulation. Econometric methodology selection. Literature synthesis. Statistical results → academic + business implications. Full paper structure (abstract → conclusion). |

---

## 100+ Skills Library

Every agent composably draws from named skills:

**Finance (20):** `skill::var_calculation` · `skill::dcf_modeling` · `skill::trade_signal_generation` · `skill::options_pricing` · `skill::credit_scoring` · `skill::cash_flow_forecasting` · `skill::merger_valuation` · `skill::crypto_on_chain` · `skill::esg_scoring` · `skill::regulatory_reporting` · `skill::fx_hedging_design` · `skill::tax_optimization` · `skill::yield_curve_analysis` · `skill::market_sentiment` · `skill::sector_rotation` · `skill::alternative_data` · `skill::earnings_analysis` · `skill::portfolio_analytics` · `skill::real_time_market_data` · `skill::financial_statement_parse`

**AI/ML (20):** `skill::rag_pipeline_design` · `skill::agent_orchestration` · `skill::hallucination_detection` · `skill::embedding_strategy` · `skill::vector_store_setup` · `skill::prompt_optimization` · `skill::llm_evaluation` · `skill::fine_tuning_prep` · `skill::memory_architecture` · `skill::semantic_routing` · `skill::tool_schema_design` · `skill::context_window_mgmt` · `skill::multi_agent_debate` · `skill::llm_security` · `skill::streaming_inference` · `skill::synthetic_data_gen` · `skill::knowledge_graph` · `skill::multi_modal_processing` · `skill::cost_optimization` · `skill::agent_evaluation`

**Code (20):** `skill::typescript_expert` · `skill::nextjs_fullstack` · `skill::fastapi_backend` · `skill::security_hardening` · `skill::test_generation` · `skill::docker_compose` · `skill::kubernetes_deploy` · `skill::terraform_iac` · `skill::github_actions_ci` · `skill::graphql_design` · `skill::websocket_realtime` · `skill::react_components` · `skill::api_versioning` · `skill::database_orm` · `skill::caching_strategy` · `skill::logging_observability` · `skill::microservices_design` · `skill::performance_optimization` · `skill::code_review_deep` · `skill::sdk_generation`

**Data (20):** `skill::sql_expert` · `skill::ab_test_design` · `skill::causal_inference` · `skill::time_series_forecast` · `skill::anomaly_detection` · `skill::dbt_modeling` · `skill::spark_processing` · `skill::airflow_orchestration` · `skill::data_quality` · `skill::feature_engineering` · `skill::pandas_master` · `skill::etl_pipeline_design` · `skill::data_visualization` · `skill::looker_dashboards` · `skill::stream_processing` · `skill::model_monitoring` · `skill::ml_pipeline` · `skill::data_storytelling` · `skill::data_catalog` · `skill::data_governance`

**Ops & Business (20):** `skill::okr_design` · `skill::project_planning` · `skill::business_case_writing` · `skill::stakeholder_management` · `skill::kpi_design` · `skill::process_mapping` · `skill::contract_review` · `skill::due_diligence_checklist` · `skill::board_reporting` · `skill::sla_design` · `skill::incident_management` · `skill::hiring_process` · `skill::compliance_audit` · `skill::demand_forecasting` · `skill::pricing_strategy` · `skill::customer_journey_mapping` · `skill::nps_analysis` · `skill::change_management` · `skill::vendor_negotiation` · `skill::jira_workflow`

**Content (15):** `skill::seo_research` · `skill::copywriting_pro` · `skill::content_strategy` · `skill::email_sequences` · `skill::technical_writing` · `skill::thought_leadership` · `skill::newsletter_writing` · `skill::social_media_strategy` · `skill::brand_voice` · `skill::video_scripting` · `skill::case_study_writing` · `skill::press_release_writing` · `skill::podcast_scripting` · `skill::grant_writing` · `skill::speechwriting`

---

## Output Format — Always

```
╔══════════════════════════════════════════════╗
║  🤖 AGENT ACTIVATION                         ║
║  Primary: QuantTrader                        ║
║  Support: RiskSentinel + CFO-Intelligence    ║
║  Skills:  trade_signal_generation | var_calc ║
║  Mode:    analysis                           ║
╚══════════════════════════════════════════════╝

■ Executive Summary       (3 bullets max — fast scan)
■ Full Analysis/Code/Strategy  (complete, never partial)
■ Confidence Level        (Low / Medium / High + reason)
■ Next Steps              (what to do with this output)
■ Caveats                 (what could change the answer)
```

**Code output rules:**
- Complete files only — never partial snippets
- TypeScript strict mode always (`no 'any'` ever)
- Full error handling in every function
- All secrets in env vars — never hardcoded
- Setup instructions + required env vars included

---

## Repository Structure

```
Claude-Agentic-Skills2.0-version/
├── prompts/
│   └── agentOS-system-prompt.md    ← The system prompt — paste this into Claude
├── agents/
│   ├── finance/                    ← Full specs for 8 finance agents
│   ├── engineering/                ← Full specs for 8 engineering agents
│   ├── data/                       ← Full specs for 6 data agents
│   ├── operations/                 ← Full specs for 8 ops agents
│   ├── content/                    ← Full specs for 6 content agents
│   └── specialized/                ← Full specs for 6+ domain agents
├── skills/
│   ├── finance-skills.md
│   ├── aiml-skills.md
│   ├── code-skills.md
│   ├── data-skills.md
│   ├── ops-skills.md
│   └── content-skills.md
├── examples/
│   ├── finance-examples.md
│   ├── engineering-examples.md
│   └── research-examples.md
├── docs/
│   ├── how-it-works.md
│   └── agent-reference.md
├── index.html                      ← Project website (warm white theme)
└── README.md
```

---

## Why AgentOS?

| Capability | Regular Claude | AgentOS |
|-----------|---------------|---------|
| Task routing | Manual | Automatic, keyword-triggered |
| Domain depth | Generalist | Sub-agent specialist per domain |
| Output structure | Variable | Consistent every response |
| Multi-domain tasks | One at a time | Parallel agent execution |
| Sub-agent decomposition | None | Built-in per agent |
| Skills library | None | 100+ named composable skills |
| Trade signals | Basic | Full JSON with R:R, sizing, regime |
| Code output | Partial OK | Complete production files, always |
| Risk analysis | Surface-level | VaR, CVaR, stress tests, heat maps |
| Financial modeling | Manual prompting | Auto-triggered by keywords |

---

## Who Is This For?

- **Finance professionals** — analysts, traders, portfolio managers, CFOs, risk teams
- **Engineers** — full-stack developers, ML engineers, data engineers, DevOps
- **Data scientists** — ML pipelines, forecasting, causal inference, experimentation
- **Founders & operators** — product, marketing, sales, legal, HR, supply chain
- **Researchers** — systematic market research, academic writing, literature synthesis
- **Anyone** who wants Claude to behave like a coordinated AI team, not a single chatbot

---

## License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE).

---

<div align="center">

**Built solo by [@vignesh2027](https://github.com/vignesh2027)**

*If AgentOS is useful to you, a ⭐ star keeps the project visible.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3000,50:3d1a00,100:1a0a00&height=120&section=footer" width="100%" />

</div>
