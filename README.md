# Hi, I'm Rakshit 👋

Data analyst. Two years in US healthcare payer analytics at Genpact, which means I've seen more claims data than most people see claims.

Currently building things that prove I can do what my resume says I can do.

## 🔍 What I'm working on

**AML Transaction Monitoring System** — SQL rule-based detection engine over 6M+ synthetic transactions (PaySim), with a Power BI alert dashboard on the way.

## Status
- ✅ Setup & data load (6.36M rows) — `01_setup.sql`
- ✅ Data profiling — `02_Data_Profiling.sql`
- ✅ Exploratory analysis, incl. fraud-label insights — `03_Exploratory_Analysis.sql`
- ✅ Detection rules v1 — 6 behavior-based rules — `04_fraud_detection_rules.sql`
- 🔧 In progress: CTEs, window functions, structuring/velocity rules, risk scoring
- ⏳ Up next: Power BI dashboard

## Key finding
PaySim's built-in `isFlaggedFraud` system catches only 16 of 8,213 fraudulent 
transactions (~0.2%) — the core motivation for this project.

## Note on methodology
Detection rules (`04`) use only transaction behavior — amount, type, balances, 
timing. They never reference the `isFraud` ground-truth label, since a real 
monitoring system wouldn't have it. Fraud-label analysis lives separately in 
`03` and later evaluation queries, where rule performance gets measured 
against it.

→ [aml-transaction-monitoring](http://github.com/rakshitrohan-in/aml-transaction-monitoring)

## 🛠️ Stack

- **Analytics:** SQL MySQL Workbench · Power BI · Excel (the Advanced VBA kind, not the pivot-table-and-pray kind) · Python
- **AI & Automation:** Anthropic Claude API · OpenAI API · n8n · Flask
- **Enterprise:** SAP · Salesforce

## 📦 Shipped

- **Resume Intelligence System** — Python job scraper + Flask + Claude API engine that tailors resumes to JDs and renders ATS-safe .docx files via Node.js. Built it because manually tailoring resumes is a job in itself, and I already had one of those.
- **AI Marketing Automation Pipeline** — n8n + OpenAI + Tavily, end-to-end content research and generation. ~80% less manual effort, 100% fewer excuses.

## 📈 Interested in

FinCrime & AML analytics · healthcare payer data · applied AI automation · the ongoing mystery of why every dataset has one column that ruins everything

## 📫 Find me

[LinkedIn](https://www.linkedin.com/in/rakshit-rohan-4b032918b/) · rakshitrohan32@gmail.com
