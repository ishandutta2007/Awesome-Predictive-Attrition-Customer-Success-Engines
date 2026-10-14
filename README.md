# Awesome-Predictive-Attrition-Customer-Success-Engines

# Awesome-Predictive-Attrition-Customer-Success-Engines

# Top Predictive Attrition & Customer Success Engines Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Customer Health Scoring, Churn Prediction & Automated Retention Playbooks*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Predictive Attrition & Customer Success Engines**. These tools aggregate product usage, CRM activity, support tickets, and communication signals into continuously updated health scores, then trigger automated playbooks when accounts show early warning signs of churn — such as reduced software utilization, declining login frequency, or shrinking active user counts.

**Examples** include Gainsight, ChurnZero, Totango, Catalyst, Planhat, Vitally, Custify, ClientSuccess, Akkio, and Upscale (the category leaders).

**Open-source emphasis**: This section is expanded with the most relevant open-source projects for self-hosted customer success analytics — ideal for teams prioritizing data sovereignty, developers building CS pipelines, and organizations avoiding per-account enterprise pricing.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Gainsight Customer Success](https://www.gainsight.com/)**  
  Enterprise customer success platform with multi-input AI health scoring, predictive churn alerts, and automated playbooks. The most configurable health scoring model in the category, with deep Salesforce integration and Staircase AI (acquired) for communication-based churn signals from email, Slack, and calls .

- **[ChurnZero](https://churnzero.net/)**  
  Customer success platform built specifically around churn prevention, with real-time health score updates and a ChurnScore methodology that fires alerts the moment an account crosses a risk threshold. Features 15+ purpose-built AI Agents and ChurnZero Connect (MCP) for Claude and ChatGPT integration .

- **[Totango / Catalyst](https://www.totango.com/)**  
  Forrester Wave Leader customer growth platform combining composable journey management, predictive revenue intelligence, and AI-assisted health scoring. Catalyst is the Salesforce-native customer growth platform with autonomous playbook execution and expansion signal detection .

- **[Planhat](https://www.planhat.com/)**  
  Agentic customer platform for B2B enterprises with governed AI agents, integrated CRM, health scoring, and lifecycle automation. Differentiates on revenue intelligence, connecting health scores directly to NRR forecasts so CS leaders can show the financial impact of churn prevention .

- **[Vitally](https://www.vitally.io/)**  
  Streamlined, visual customer success platform with real-time scorecards based on customer activity and Notion-style collaborative spaces. HubSpot-native with limited Salesforce support. Best for startups and scaling CS teams prioritizing speed and clarity .

- **[Custify](https://www.custify.com/)**  
  Customer success platform for SaaS with AI agents that self-configure around business rules, health scoring, churn prediction, and lifecycle automation. Accessible entry point for smaller teams with simpler data setups .

- **[ClientSuccess](https://www.clientsuccess.com/)**  
  Customer success platform with health scoring, success plays, and client engagement tracking for B2B SaaS.

- **[Akkio](https://www.akkio.com/)**  
  No-code AI platform for churn prediction and customer scoring. Accessible for teams without data science resources .

- **[Upscale](https://upscale.ai/)**  
  AI-powered revenue intelligence platform with churn prediction and account expansion signals.

- **[Staircase AI](https://www.staircase.ai/)**  
  Communication-based churn detection analyzing every customer email, call, Slack message, and support ticket to surface churn risk, sentiment shifts, and stakeholder changes — useful for teams with gaps in product usage telemetry .

## Open-Source GitHub Projects

- **[gtm-agent-user-health-analyzer](https://github.com/tushar-badhwar/gtm-agent-user-health-analyzer)**  
  **MCP server for AI-driven customer health analysis.** Integrates with Claude Desktop to analyze customer health from usage data (login patterns, feature adoption, session durations), CRM data (contact history, sentiment, contract details), and support data (tickets, resolution times, sentiments). Provides `analyze_customer_health`, `get_recommendations`, and `list_customers` tools, plus Airtable discovery and management. Sample data includes healthy, at-risk, and critical customer profiles .

- **[Customer Success Manager Agent Skills](https://github.com/alirezarezvani/claude-skills)**  
  **Production-grade customer success analytics with three Python CLI tools** — deterministic, repeatable analysis using standard library only, no external dependencies . Includes `health_score_calculator.py` (multi-dimensional health scoring with configurable weights across Product/usage, Relationship/engagement, and Outcomes/results), `churn_risk_analyzer.py` (risk tiers across Enterprise, Mid-Market, and SMB segments), and `expansion_opportunity_scorer.py` (prioritized expansion recommendations). MIT licensed, JSON input/output for pipeline integration .

- **[health_scorer.py](https://github.com/borghei/Claude-Skills)**  
  **Standalone Python health scoring script** implementing a multi-dimensional model with configurable weights. Product dimension (login frequency, feature adoption, active users ratio, support tickets inverse), Relationship dimension (executive engagement, meeting attendance, NPS, response time), and Outcomes dimension (goals achieved, ROI demonstrated, business impact). Outputs health scores on 0-100 scale with green/yellow/red status tiers and recommended actions per tier .

- **[ChurnGuard AI](https://github.com/jaideep005/churn_retention_system)**  
  **End-to-end churn prediction and retention intelligence web application** built with Streamlit, Scikit-Learn, and LLM integration. Features data ingestion from IBM Telco dataset or custom API, ETL pipeline with feature engineering (LTV, engagement score, NPS segments), ML models (Logistic Regression + Random Forest with 5-fold cross-validation), interactive dashboard with KPI cards and risk segmentation, AI-generated personalized retention playbooks per customer using OpenAI GPT or Google Gemini, and Power BI export. MIT licensed .

- **[churn-prediction-ml-pipeline](https://github.com/anandsuraj/churn-prediction-ml-pipeline)**  
  **Fully automated ML pipeline for customer churn prediction** orchestrated with Apache Airflow. Covers data ingestion, validation, feature engineering, model training, deployment, and monitoring with DVC-based versioning for complete reproducibility. Implements feature store, data versioning, and SQLite database for schema management. Uses IBM Telco Customer Churn dataset with comprehensive logging .

- **[CustomerCheck for Nextcloud](https://apps.nextcloud.com/apps/customercheck)**  
  **Nextcloud-native CRM for customer work** — one place where a workspace shares a customer book, shared mailbox, account plans, and operating rituals . Features Company 360 with "Ten Command Questions," renewal engine with 60/30/7/0/+7 exactly-once reminders, shared mailbox (IMAP + SMTP), KAM coverage tracking, team coaching with stuck boards, and Check Partner hours tracking. AGPL licensed, Nextcloud 32-34 compatible .

- **[customer-360-dbt](https://github.com/ndleah/customer-360-dbt)**  
  **Kimball-style 3-layer dbt project unifying customer data** with PII masking at staging layer and source freshness validation . Builds a complete customer 360 view from raw sources — the foundation data layer for health scoring and churn analysis.

- **[dbt-labs/attribution-playbook](https://github.com/dbt-labs/attribution-playbook)**  
  **Multi-touch attribution modeling** adjacent to CS — tells you which channels acquired customers you're now trying to retain. Uses Markov chains and Shapley values to attribute conversions across touchpoints. Useful for understanding the acquisition quality of cohorts that later churn.

### Additional Strong Open-Source Options

- **Chatwoot** — Open-source customer engagement platform (Intercom/Zendesk alternative) with dashboard showing total messages, response times, and resolution times. Custom Attributes feature stores account-level CS data. Ruby on Rails + Vue.js, PostgreSQL .
- **Zammad** — Open-source helpdesk software centralizing customer communications. 5,319 GitHub stars .
- **Frappe Helpdesk** — Open-source ticketing system consolidating customer issues, automating workflows, and empowering self-service. 2,858 GitHub stars .
- **Formbricks** — Privacy-first surveys with self-hosting options and GDPR compliance. 11,727 GitHub stars. Useful for NPS and CSAT collection feeding into health scores .
- **Fider** — Self-hosted community feedback tool for gathering and prioritizing user suggestions. 4,009 GitHub stars .

**Frameworks for building custom systems**: Combine **gtm-agent-user-health-analyzer** for MCP-based health analysis with Claude integration, **Customer Success Manager Agent Skills** for deterministic CLI-based health scoring and churn risk tiering, **ChurnGuard AI** for ML-based churn prediction with AI retention playbooks, **customer-360-dbt** for unified customer data modeling, and **Chatwoot** or **Zammad** for support interaction tracking to build a complete self-hosted predictive attrition stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Predictive attrition tools must comply with data protection regulations (GDPR, CCPA), employee monitoring laws, and industry-specific compliance requirements. **Health scores and churn predictions are estimates — they must be validated against actual outcomes and should augment, not replace, CSM judgment.** False positives can waste retention resources; false negatives can lose accounts that could have been saved. Reduced software utilization is a signal, not proof — it may indicate seasonality, workflow changes, or user role transitions rather than impending churn.
- Self-hosted open-source solutions require proper integration with product analytics, CRM, and support systems, plus ongoing validation of scoring models against actual churn events.

---

**Made for customer success leaders, CS operations teams, retention managers, and developers building predictive CS platforms.**  
Let's make predictive attrition and customer success more open, accurate, and retention-focused.
