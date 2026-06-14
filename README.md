# ⚖️ CJOC Open Framework 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Active Development](https://img.shields.io/badge/Status-Active%20Development-brightgreen)]()
[![Topic: Open Government](https://img.shields.io/badge/Topic-Open%20Government-blue)]()
[![Topic: Civic Tech](https://img.shields.io/badge/Topic-Civic%20Tech-purple)]()

> **Disclaimer:** *This is an independent, open-source research and advocacy initiative. It is not an official project of the Irish Government, the Department of Justice, or any state agency. The "Criminal Justice Oversight Commission" (CJOC) is a proposed statutory model. This repository provides the conceptual, technical, and methodological framework to advocate for and inform its creation.*

---

## 📖 Overview

The **CJOC Open Framework** is an open-source initiative designed to promote transparency, accountability, and systemic integrity across Ireland’s criminal justice sector. 

Currently, Ireland’s justice oversight is highly siloed (e.g., Fiosrú for policing, Inspector of Prisons for custody). There is no unified, independent statutory body mandated to investigate **cross-cutting integrity risks** that span multiple agencies. 

This repository provides the methodologies, standardized data schemas, and analytical tools needed to:
1. Monitor and map integrity risks across An Garda Síochána, the Irish Prison Service, the Probation Service, and the Courts Service.
2. Standardize metrics for cross-agency and EU-level benchmarking.
3. Support evidence-based advocacy for the establishment of a statutory **Criminal Justice Oversight Commission (CJOC)**.
4. Empower researchers, journalists, and civil society with structured, citable, and auditable datasets.

The framework is explicitly aligned with the **EU Anti-Corruption Directive** and **Council of Europe GRECO** recommendations.

---

## 📂 Project Directory

This repository is organized to separate policy documentation, technical schemas, and analytical tools for easy navigation and contribution.

```text
cjoc-framework/
│
├── 📁 docs/                          # Policy, legislative, and strategic documentation
│   ├── 01_Executive_Summary.md       # High-level overview of the CJOC model
│   ├── 02_Legislative_Framework.md   # Draft structure for the proposed CJOC Act
│   ├── 03_EU_GRECO_Alignment.md      # Mapping of framework goals to EU/GRECO mandates
│   ├── 04_Jurisdictional_Boundaries.md # Clarification of scope (e.g., excluding Judiciary/DPP discretion)
│   └── 05_Stakeholder_Mapping.md     # Interoperability map (Fiosrú, SIPO, Ombudsman, etc.)
│
├── 📁 schemas/                       # Standardized data models for justice metrics
│   ├── justice_metrics_core.json     # Core schema for agency performance and integrity metrics
│   ├── cross_agency_incident.json    # Schema for logging multi-agency integrity events
│   └── foi_request_template.json     # Standardized structure for Freedom of Information requests
│
├── 📁 tools/                         # Open-source scripts and analytical notebooks
│   ├── data_anonymizer.py            # Tool to safely anonymize FOI data for public release
│   ├── integrity_risk_calculator.ipynb # Jupyter notebook for scoring systemic vulnerability
│   └── greco_compliance_checker.py   # Script to audit public datasets against GRECO indicators
│
├── 📁 reports/                       # Published research and baseline assessments
│   ├── baseline_assessment_2024.md   # Initial gap analysis of Ireland's current oversight model
│   └── case_studies/                 # Anonymized examples of cross-cutting justice failures
│
└── README.md                         # You are here!
```

---

## 🚀 Current Features

The framework currently provides the following foundational capabilities:

*   **📊 Standardized Data Schemas:** JSON-based data models designed to normalize disparate data from the Garda, Prison, and Probation services, enabling apples-to-apples comparison.
*   **🔍 Cross-Agency Risk Mapping:** Methodologies for identifying vulnerabilities at the intersections of agencies (e.g., evidence chain-of-custody handoffs between AGS and IPS).
*   **⚖️ Jurisdictional Guardrails:** Clearly defined boundaries ensuring the framework respects the constitutional independence of the Judiciary and the prosecutorial discretion of the DPP.
*   **🌍 International Compliance Mapping:** Direct cross-referencing of framework metrics with specific articles of the EU Anti-Corruption Directive and GRECO evaluation reports.
*   **🛡️ Privacy-First Tooling:** Python scripts for anonymizing sensitive Freedom of Information (FOI) data, allowing researchers to publish findings without compromising individual privacy or active investigations.

---

## 🗺️ Roadmap & Future Features

We are actively developing the next phases of the CJOC Framework. Contributions and feedback are highly encouraged.

### Phase 1: Q3 2026 (Data Ingestion & Automation)
- [ ] **FOI API Connector:** A Python library to automate the scraping and structuring of published FOI logs from justice sector websites.
- [ ] **Interactive Dashboard Prototype:** A Streamlit or Dash-based web interface to visualize baseline integrity metrics and cross-agency anomalies.
- [ ] **Automated Anomaly Detection:** Machine learning models to flag statistical outliers in case processing times or disciplinary actions.

### Phase 2: Q1 2027 (Advocacy & Policy Generation)
- [ ] **Legislative Draft Generator:** A tool that auto-generates tailored policy briefs and legislative amendments for Oireachtas members based on identified data gaps.
- [ ] **Civil Society Toolkit:** A simplified, non-technical guide for NGOs and journalists on how to use the framework's schemas to file targeted FOI requests.
- [ ] **Multi-Language Support:** Translation of core documentation and schemas into Irish (Gaeilge) to ensure full accessibility and alignment with the Official Languages Act.

### Phase 3: Q3 2027 (Institutional Integration)
- [ ] **Shadow Reporting Module:** A structured format for the framework to publish an annual "Shadow State of Criminal Justice Integrity" report, parallel to official state publications.
- [ ] **Secure Whistleblower Intake Schema:** A cryptographically secure, anonymized data intake model for internal justice sector workers to report systemic issues safely.

---

## 🤝 Contributing

We welcome contributions from legal scholars, data scientists, journalists, and civic technologists. 

1. **Fork** the repository.
2. **Create** a new branch (`git checkout -b feature/YourFeatureName`).
3. **Commit** your changes (`git commit -m 'Add some feature'`).
4. **Push** to the branch (`git push origin feature/YourFeatureName`).
5. **Open a Pull Request** detailing the changes and their relevance to the CJOC mission.

Please review our [Code of Conduct](docs/06_Code_of_Conduct.md) and [Contributing Guidelines](docs/07_Contributing.md) before submitting.

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details. 

*The data schemas and analytical tools are free to use, modify, and distribute. We kindly request that any published research or advocacy materials utilizing this framework cite this repository to maintain a cohesive body of evidence.*

---

## 📬 Contact & Community

*   **Issues & Bug Reports:** Please use the GitHub [Issues](../../issues) tab.
*   **Discussions:** Join the conversation in the GitHub [Discussions](../../discussions) tab.
*   **Secure Contact:** For sensitive inquiries related to justice sector vulnerabilities, please refer to the secure contact protocols outlined in `docs/08_Secure_Communications.md`.

*Built with ❤️ for transparency, accountability, and the rule of law in Ireland.*
