# National Justice Integrity Commission (NJIC) — Ireland
## Open-Source Framework for Transparency, Accountability & Anti-Corruption

**License:** MIT  
**Python:** 3.10+  
**Status:** Early Development / Advocacy Framework  
**Last Updated:** 2026-05-28

---

## ⚠️ CRITICAL DISCLAIMERS

**1. No Investigative Authority:** This framework is a **research and advocacy tool**. It does **not** possess statutory powers of investigation, subpoena, or enforcement. All findings are derived from publicly available data, Freedom of Information (FOI) responses, and validated third-party sources.

 **2. Allegations Are Unproven:** References to "misconduct," "corruption," or "irregularities" document **allegations, complaints, or administrative proceedings** — not proven findings of guilt. All entries include source provenance and date.

**3. Fair Comment & Qualified Privilege:** This project relies on the Defamation Act 2009 (Ireland), ss. 20 (honest opinion) and 28 (fair and accurate report of proceedings). Malice is expressly disclaimed.

**4. Data Protection:** All datasets are anonymized, aggregated, or lawfully obtained via FOI. A Data Protection Impact Assessment (DPIA) is maintained. No whistleblower identities are stored in project repositories.

**5. Institutional Independence:** References to GSOC, DPP, C&AG, CSO, Courts Service, IPS, and Probation Service indicate **target data sources** or **referenced public bodies** — not formal partnerships, endorsements, or collaborations unless explicitly documented in a signed memorandum.

---

## 📌 Project Overview

The **NJIC Framework** is an open-source initiative to promote transparency and accountability across Ireland’s justice sector. It provides **methodologies, data schemas, and analysis tools** to:

- **Monitor integrity risks** in An Garda Síochána, Irish Prison Service, Courts Service, and Probation Service.
- **Standardize metrics** for cross-agency and EU benchmarking.
- **Support evidence-based advocacy** for the establishment of a statutory NJIC.
- **Empower researchers and journalists** with structured, citable datasets.

### Why This Project?

Ireland lacks a unified, independent statutory body to investigate cross-cutting integrity issues in the justice system. This framework addresses that gap by creating **reusable, auditable methodologies** that could inform the design of such a body, aligned with the **EU Anti-Corruption Directive (2023/2223)** and **Council of Europe GRECO** recommendations.

---

## ✅ Feature Inventory

### Maturity Legend
| Symbol | Meaning |
|--------|---------|
| ✅ **Documented** | Methodology, schema, and specification are complete. |
| 🔧 **Prototype** | Working code or dataset exists; requires peer validation. |
| 🚧 **Planned** | Specification drafted; awaiting development or data acquisition. |
| 📡 **External** | Depends on third-party data feeds not yet integrated. |

### Core Framework

| Feature | Description | Status | Data Source Type |
|---------|-------------|--------|------------------|
| Integrity Risk Assessment Matrix | 5-dimension weighted scoring methodology with rubric. | ✅ Documented | CSO, Eurostat, FOI |
| Cross-System Comparison Tool | EU benchmarking templates (Denmark, Netherlands, UK). | ✅ Documented | Eurostat, TI-CPI |
| Corruption Risk Heatmaps | Visualization spec for high-risk agency functions. | 🔧 Prototype | C&AG, FOI |
| Whistleblower Support Portal | **Architecture and DPIA only.** No production system. | 🚧 Planned | N/A |

### Data & Analytics

| Feature | Description | Status | Notes |
|---------|-------------|--------|-------|
| Open Datasets | Curated **metadata catalog** describing available vs. restricted data. | ✅ Documented | See DATA_AVAILABILITY.md |
| Interactive Dashboards | Plotly/Dash specification and sample notebooks. | 🔧 Prototype | Power BI templates planned |
| Automated Annual Reports | Python script (`annual_report_generator.py`) | 🔧 Prototype | See `src/reporting/` |
| Real-Time Alerts | Specification for anomaly detection thresholds. | 🚧 Planned | Requires data feeds |

### Transparency Tools

| Feature | Description | Status | Legal Notes |
|---------|-------------|--------|-------------|
| Misconduct Tracker | **Schema and methodology** for anonymized case logging. | ✅ Documented | Subject to DPIA; no PII stored |
| FOI Audit Tool | Tracker for FOI request compliance by agency. | 🔧 Prototype | Uses FOI Commissioner public data |
| Procurement Watchdog | Specification for contract irregularity detection. | 🚧 Planned | C&AG reports as primary source |
| Judicial Transparency Index | Scoring rubric for judicial accountability metrics. | 🚧 Planned | Judicial Council data only |

### Advocacy & Reform

| Feature | Description | Status |
|---------|-------------|--------|
| Policy Recommendations | Evidence-based reform proposals (NJIC Act draft). | ✅ Documented |
| Stakeholder Templates | Email and presentation templates for advocacy. | ✅ Documented |
| Public Awareness Materials | Infographic and social media specifications. | 🚧 Planned |
| Petition & Lobbying Tools | Guide to effective lobbying under Irish law. | 🚧 Planned |

### Developer Tools

| Feature | Description | Status |
|---------|-------------|--------|
| NJIC API | OpenAPI 3.0 specification for future REST API. | 🚧 Planned |
| Data Validation Scripts | PyTest suite for dataset schema validation. | 🔧 Prototype |
| Customizable Framework | Adaptation guide for other jurisdictions. | ✅ Documented |
| Docker Environment | `docker-compose.yml` for local development. | 🔧 Prototype |

---

## 🗺️ Roadmap

### Phase 0: Foundation (Q3 2026)
- [ ] Finalize and publish all legal frameworks (DPIA, disclaimers, ethics policy).
- [ ] Complete Data Availability & FOI Matrix for all justice agencies.
- [ ] Publish Integrity Risk Assessment Methodology v1.0.
- [ ] Release first prototype annual report (synthetic/demo data).
- [ ] Establish independent academic review panel (UCD/TCD).

### Phase 1: Data Acquisition (Q4 2026 – Q1 2027)
- [ ] File batch FOI requests for baseline datasets.
- [ ] Publish metadata catalog and sample (anonymized) datasets.
- [ ] Launch GitHub repository with full documentation.
- [ ] Pilot FOI Audit Tool with 12-month tracking.

### Phase 2: Tool Development (2027)
- [ ] Build interactive dashboards (Plotly/Dash).
- [ ] Develop Procurement Watchdog prototype.
- [ ] Publish first cross-system comparison report.
- [ ] Host public webinar series with civil society.

### Phase 3: Advocacy & Scale (2028–2029)
- [ ] Submit policy brief to Oireachtas Justice Committee.
- [ ] Launch NJIC API (beta).
- [ ] Develop mobile-accessible public dashboard.
- [ ] Advocate for NJIC legislation via civil society coalition.

---

## 📂 Repository Structure

```
njic-ireland/
├── docs/
│   ├── framework/           # Methodology, metrics, scoring rubrics
│   ├── legal/               # DPIA, disclaimers, defamation policy
│   ├── advocacy/            # Policy briefs, lobbying guides
│   └── guides/              # FOI templates, contributor guides
├── data/
│   ├── catalog/             # Metadata and availability matrices
│   ├── samples/             # Anonymized demo datasets ONLY
│   └── raw/                 # .gitignore — local FOI responses
├── src/
│   ├── data-processing/     # Cleaning, validation scripts
│   ├── reporting/           # Annual report generator
│   └── visualization/       # Plotly/Dash dashboards
├── tools/
│   ├── foi-audit/           # FOI compliance tracker
│   └── risk-assessment/     # Scoring engine
├── api/
│   └── spec/                # OpenAPI specification
├── tests/
├── .github/
│   ├── CONTRIBUTING.md
│   ├── ISSUE_TEMPLATE/
│   └── SECURITY.md
├── LICENSE                  # MIT
├── README.md                # This file
├── DATA_AVAILABILITY.md     # Deliverable 2
├── METHODOLOGY.md           # Deliverable 3
├── DPIA.md                  # Deliverable 4
└── RISK_REGISTER.md         # Deliverable 5
```

---

## 🤝 How to Contribute

### Reporting Issues
- Open an issue for bugs, data corrections, or legal concerns.
- Security disclosures: See `SECURITY.md`.

### Code Contributions
1. Fork and branch (`feature/your-feature`).
2. All code must include tests and docstrings.
3. Pull requests require review by two maintainers.

### Data Contributions
- **Do not submit personal data.** Only anonymized, aggregated, or public records.
- Include provenance (source URL, FOI reference, or publication date).
- Submit via Pull Request with data dictionary.

### Advocacy
- Share using **#NJICIreland**.
- Write op-eds citing framework methodology.
- Contact your TD regarding NJIC legislation.

---

## 📜 License

MIT License — see `LICENSE`. You must:
- Cite the source in derivative works.
- Share improvements via Pull Request or fork.
- **Not** use project outputs to make unverified defamatory statements against individuals.

---

## 📞 Contact & Governance

- **Project Lead:** [Contact via GitHub Issues] *(Email TBD — see governance discussion)*
- **GitHub:** [Transparency-X/njic-ireland](https://github.com/Transparency-X/njic-ireland)
- **Security:** Report vulnerabilities via GitHub Security Advisories.
- **Data Protection Queries:** Refer to `DPIA.md` or contact the Irish Data Protection Commission.

---

## 🙏 Acknowledgments

- **Transparency International Ireland** — methodology guidance.
- **Irish Council for Civil Liberties (ICCL)** — transparency standards feedback.
- **Central Statistics Office (CSO)** — open data provision.
- **Academic Reviewers** — TBD via open call.

---

*"Integrity in justice is the foundation of a fair society."*

**© 2026 NJIC Ireland Contributors.**
