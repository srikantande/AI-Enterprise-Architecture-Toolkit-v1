# 🤖 AI Enterprise Architecture Toolkit

> A comprehensive, TOGAF-aligned governance and architecture toolkit for enterprise AI portfolios — covering governance frameworks, architecture patterns, operational artefacts, decision records, and EA deliverables.

![Version](https://img.shields.io/badge/version-1.0-blue)
![TOGAF](https://img.shields.io/badge/TOGAF-ADM%20Phases%20B%2CC%2CD%2CE-orange)
![Standards](https://img.shields.io/badge/Standards-ISO%2FIEC%2042001%20%7C%20NIST%20AI%20RMF-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Who Is This For?](#-who-is-this-for)
- [Repository Structure](#-repository-structure)
- [Module Descriptions](#-module-descriptions)
  - [01 · Governance](#01--governance)
  - [02 · Architecture](#02--architecture)
  - [03 · Operational](#03--operational)
  - [04 · Templates](#04--templates)
  - [05 · EA Artefacts](#05--ea-artefacts)
- [Standards & Compliance](#-standards--compliance)
- [Governance Model](#-governance-model)
- [AI Risk Tiers](#-ai-risk-tiers)
- [Getting Started](#-getting-started)
- [Contributing](#-contributing)

---

## 🔍 Overview

The **AI Enterprise Architecture Toolkit** provides a production-ready, standards-aligned reference framework for organisations building and governing enterprise AI portfolios. It brings together governance guardrails, cloud platform standards (GCP & AWS), architecture decision records, RACI matrices, capability heat maps, and reusable templates — all structured within a TOGAF Architecture Development Methodology (ADM).

**Built for enterprise teams who need to:**
- Govern AI initiatives across multiple business units and cloud platforms
- Ensure regulatory compliance (GDPR, EU AI Act, ISO/IEC 42001:2023)
- Apply consistent architecture patterns across Generative AI, ML, and Agentic workloads
- Manage the full AI lifecycle from ideation through to decommissioning

---

## 👥 Who Is This For?

| Role | How to Use This Toolkit |
|---|---|
| **Enterprise Architect** | Governance framework, ADRs, EA artefacts, capability model |
| **Cloud Platform Architect** | Platform standards (GCP/AWS), architecture patterns, YAML configs |
| **AI/ML Engineering Lead** | MLOps standards, service catalog, architecture review checklist |
| **Security Architect** | Guardrails (G-001 to G-005), risk assessment, review checklist |
| **Risk & Compliance Officer** | Governance policies, risk assessment CSV, RACI matrix |
| **Business Sponsor** | AI portfolio register, capability heat map, roadmap alignment |

---

## 📁 Repository Structure

```
AI-Enterprise-Architecture-Toolkit/
├── README.md
│
├── 01.governance/                         # Governance framework, policies & risk
│   ├── 01.01_ai_governance_framework_v1.md
│   ├── 01.02_ai_governance_config.yaml
│   └── 01.03_policies/
│       ├── 01.03.01_ai_governance_policies.csv
│       └── 01.03.02_ai_risk_assessment.csv
│
├── 02.architecture/                       # Architecture patterns & decision records
│   ├── 02.01_ai_architecture_patterns.yaml
│   ├── 02.02_ai_architecture_patterns.csv
│   └── 02.03.adrs/
│       └── 02.03.01_Architecture_Decision_Records_5_Pre_loaded_ADRs.md
│
├── 03.operational/                        # RACI, capability heat map & service catalog
│   ├── 03.01_ai_raci_matrix.csv
│   ├── 03.02_ai_capability_heat_map.csv
│   └── 03.03_ai_service_catalog.csv
│
├── 04.templates/                          # Reusable templates for reviews & runbooks
│   ├── 04.01_ai_architecture_review_checklist.md
│   ├── 04.02_adr_template.md
│   ├── 04.03_ai_runbook_template.md
│   └── 04.04_ai_runbook_config.yaml
│
└── 05.EA_artefacts/                       # Enterprise Architecture vision & capability model
    ├── 05.01_AI_vision.md
    └── 05.02_Capability_Model.csv
```

---

## 📦 Module Descriptions

### 01 · Governance

> Establishes the guardrails, decision rights, and policy framework for all AI initiatives.

| File | Description |
|---|---|
| [`01.01_ai_governance_framework_v1.md`](./01.governance/01.01_ai_governance_framework_v1.md) | Master governance framework — council composition, RACI, guardrails, lifecycle gates, cloud platform standards, and AI portfolio register |
| [`01.02_ai_governance_config.yaml`](./01.governance/01.02_ai_governance_config.yaml) | Machine-readable governance configuration — guardrail rules, approval thresholds, meeting cadence, and platform settings |
| [`01.03_policies/01.03.01_ai_governance_policies.csv`](./01.governance/01.03_policies/01.03.01_ai_governance_policies.csv) | Structured policy register — policy IDs, categories, descriptions, enforcement level, and review dates |
| [`01.03_policies/01.03.02_ai_risk_assessment.csv`](./01.governance/01.03_policies/01.03.02_ai_risk_assessment.csv) | AI risk assessment register — risk IDs, likelihood, impact, mitigation controls, and ownership |

**Key governance constructs:**

- **5 Mandatory Guardrails** (G-001 to G-005): Data Sovereignty, Model Transparency, Human-in-the-Loop, Security & Access, Ethical AI
- **3 Advisory Guardrails** (AG-001 to AG-003): Cost Optimisation, Reusability, Observability
- **AI Architecture Governance Council (AAGC)**: 8-role council with weekly → quarterly meeting cadence

---

### 02 · Architecture

> Architecture patterns, approved cloud service mappings, and pre-loaded Architecture Decision Records.

| File | Description |
|---|---|
| [`02.01_ai_architecture_patterns.yaml`](./02.architecture/02.01_ai_architecture_patterns.yaml) | Machine-readable pattern library — RAG, GenAI pipelines, MLOps, agentic patterns with platform mappings |
| [`02.02_ai_architecture_patterns.csv`](./02.architecture/02.02_ai_architecture_patterns.csv) | Tabular pattern reference — pattern name, use case, GCP service, AWS service, guardrails applied, and tier |
| [`02.03.adrs/02.03.01_Architecture_Decision_Records_5_Pre_loaded_ADRs.md`](./02.architecture/02.03.adrs/02.03.01_Architecture_Decision_Records_5_Pre_loaded_ADRs.md) | 5 pre-loaded ADRs covering foundational decisions (platform selection, MLOps toolchain, model registry, guardrail enforcement, observability stack) |

**ADR Status Flow:**
```
Proposed → Under Review → Accepted → Superseded
```

---

### 03 · Operational

> Day-to-day operational artefacts for managing the AI portfolio across teams and platforms.

| File | Description |
|---|---|
| [`03.01_ai_raci_matrix.csv`](./03.operational/03.01_ai_raci_matrix.csv) | Full RACI matrix across all AI decision areas — EA, Cloud Architect, Security, Business, Legal, and MLOps roles |
| [`03.02_ai_capability_heat_map.csv`](./03.operational/03.02_ai_capability_heat_map.csv) | Capability heat map — maturity scores per AI capability domain (0–5 scale), gaps, and target state |
| [`03.03_ai_service_catalog.csv`](./03.operational/03.03_ai_service_catalog.csv) | Enterprise AI service catalog — approved services, onboarding path, SLAs, cost model, and business unit ownership |

**RACI Key:** `R` = Responsible · `A` = Accountable · `C` = Consulted · `I` = Informed

---

### 04 · Templates

> Reusable, fill-in-the-blank templates for architecture reviews, runbooks, and decision records.

| File | Description |
|---|---|
| [`04.01_ai_architecture_review_checklist.md`](./04.templates/04.01_ai_architecture_review_checklist.md) | Gate-by-gate review checklist covering Pre-Architecture, Security, Architecture Quality, and Compliance checkpoints |
| [`04.02_adr_template.md`](./04.templates/04.02_adr_template.md) | Blank ADR template — Context, Decision, Consequences (positive/negative/risks), and Compliance mapping |
| [`04.03_ai_runbook_template.md`](./04.templates/04.03_ai_runbook_template.md) | Operational runbook template for AI workloads — incident response, rollback procedures, escalation paths |
| [`04.04_ai_runbook_config.yaml`](./04.templates/04.04_ai_runbook_config.yaml) | YAML configuration companion to the runbook template — alerts, thresholds, and on-call routing |

---

### 05 · EA Artefacts

> Strategic Enterprise Architecture deliverables aligned to TOGAF ADM.

| File | Description |
|---|---|
| [`05.01_AI_vision.md`](./05.EA_artefacts/05.01_AI_vision.md) | AI Vision statement — strategic intent, guiding principles, target state, and alignment to enterprise strategy |
| [`05.02_Capability_Model.csv`](./05.EA_artefacts/05.02_Capability_Model.csv) | AI capability model — capability domains, sub-capabilities, current vs. target maturity, and enabling technologies |

---

## 📐 Standards & Compliance

This toolkit is designed to support compliance with the following standards and frameworks:

| Standard / Framework | Coverage in This Toolkit |
|---|---|
| **TOGAF ADM** (Phases B, C, D, E) | Governance framework, EA artefacts, ADRs, architecture patterns |
| **ISO/IEC 42001:2023** | AI management system requirements mapped to governance policies |
| **NIST AI Risk Management Framework** | Risk assessment register, guardrails, model risk classification |
| **Google AI Principles** | Ethical AI guardrail (G-005), bias testing requirements |
| **EU AI Act** | High-risk AI classification (Tier 3), prohibited use restrictions |
| **GDPR** | Data sovereignty guardrail (G-001), DLP requirements, review checklist |
| **AWS Well-Architected AI Lens** | AWS platform standards (Section 7.2), architecture patterns |
| **GCP Recommended Practices** | GCP platform standards (Section 7.1), Vertex AI configurations |

---

## 🏛️ Governance Model

The **AI Architecture Governance Council (AAGC)** is the decision-making body for all AI architectural matters:

```
┌─────────────────────────────────────────────┐
│        AI Architecture Governance Council    │
│              (AAGC)                          │
├──────────────────┬──────────────────────────┤
│  Chief AI        │  Enterprise Architect     │
│  Architect       │  (TOGAF)                  │
│  (Chair)         │                           │
├──────────────────┼──────────────────────────┤
│  Cloud Platform  │  Data Privacy /           │
│  Architect       │  Legal Officer            │
├──────────────────┼──────────────────────────┤
│  Security        │  AI/ML Engineering        │
│  Architect       │  Lead                     │
├──────────────────┼──────────────────────────┤
│  Business        │  Risk & Compliance        │
│  Sponsor         │  Officer                  │
└──────────────────┴──────────────────────────┘
```

**Meeting cadence:**

| Frequency | Forum | Purpose |
|---|---|---|
| Weekly | AI Sprint Review | Architecture conformance |
| Bi-weekly | AI Design Authority | New patterns, technology adoptions |
| Monthly | Architecture Review Board | Gantt, budget, risk |
| Quarterly | Strategic AI Roadmap | Enterprise strategy alignment |

---

## 🎯 AI Risk Tiers

All AI projects are classified into one of three risk tiers, determining the approval path:

| Tier | Description | Examples | Approval Required |
|---|---|---|---|
| 🟢 **Tier 1 — Low Risk** | Internal, non-personal, advisory | Internal knowledge base, document summarisation | Project Lead |
| 🟡 **Tier 2 — Medium Risk** | Customer-facing, aggregated data | Customer support GenAI, recommendation engines | EA + Security |
| 🔴 **Tier 3 — High Risk** | PII/PHI, automated decisions | Fraud detection, HR screening, clinical AI | EA + Legal + C-Level |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/AI-Enterprise-Architecture-Toolkit.git
cd AI-Enterprise-Architecture-Toolkit
```

### 2. Starting a New AI Project?

Follow this path through the toolkit:

```
Step 1 → Read the Governance Framework
         01.governance/01.01_ai_governance_framework_v1.md

Step 2 → Score your use case & classify risk tier
         01.governance/01.03_policies/01.03.02_ai_risk_assessment.csv

Step 3 → Identify applicable architecture patterns
         02.architecture/02.02_ai_architecture_patterns.csv

Step 4 → Raise an Architecture Decision Record
         04.templates/04.02_adr_template.md

Step 5 → Complete the Architecture Review Checklist
         04.templates/04.01_ai_architecture_review_checklist.md

Step 6 → Prepare your operational runbook
         04.templates/04.03_ai_runbook_template.md
```

### 3. Reviewing an Existing AI Project?

Use the checklist at [`04.01_ai_architecture_review_checklist.md`](./04.templates/04.01_ai_architecture_review_checklist.md) which covers:

- [ ] Pre-Architecture (OKRs, data assessment, target state)
- [ ] Security (encryption, VPC controls, IAM, DLP)
- [ ] Architecture Quality (DR, cost model, observability, versioning)
- [ ] Compliance (GDPR, EU AI Act, bias tests, HITL controls)

---

## 🤝 Contributing

Contributions are welcome. Please follow these guidelines:

1. **Governance changes** — raise a new ADR in `02.03.adrs/` before making changes to framework documents
2. **New architecture patterns** — add to both `02.01_ai_architecture_patterns.yaml` and `02.02_ai_architecture_patterns.csv`
3. **Template improvements** — update both the `.md` template and the corresponding `.yaml` config where applicable
4. **Policy updates** — reflect changes in `01.03_policies/` and update the governance config YAML

> All contributions must be reviewed and approved by the AI Architecture Governance Council (AAGC) before merging.

---

## 📅 Roadmap

| Quarter | Milestone |
|---|---|
| **Q1 2025** | Governance framework rollout, ADR process live |
| **Q2 2025** | Shared Feature Store, CI/CD templates for AI |
| **Q3 2025** | AI FinOps dashboard, automated bias testing |
| **Q4 2025** | Agentic AI platform, multi-modal evaluation |

---

## 📖 Glossary

| Term | Definition |
|---|---|
| **ADR** | Architecture Decision Record |
| **AAGC** | AI Architecture Governance Council |
| **AIB** | Architecture Integration Baseline |
| **CMEK** | Customer-Managed Encryption Keys |
| **DLP** | Data Loss Prevention |
| **HITL** | Human-in-the-Loop |
| **MLOps** | Machine Learning Operations |
| **RAG** | Retrieval-Augmented Generation |
| **TOGAF ADM** | The Open Group Architecture Framework — Architecture Development Method |

---

*AI Enterprise Architecture Toolkit v1.0 — Enterprise Architecture AI Portfolio — January 2025*
