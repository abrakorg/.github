<div align="center">

# Abrak · ABRAK CO
### Intelligent Business Solutions Processing

**Enterprise Cloud ERP Platform Based on Odoo 19 and NexERP; Deep Localization and Multi-Tenant SaaS Architecture for Iranian and Knowledge-Based Enterprises**

[**Official Website (abrak.org)**](https://abrak.org) · [**NexERP (zdr.ir)**](https://zdr.ir) · [**Technical Documentation**](https://github.com/abrakorg/abrak-docs/tree/main/en)

---

[فارسی](./README.fa.md) • [English](./README.en.md) • [العربية](./README.ar.md) • [Türkçe](./README.tr.md)

</div>

---

## 1. About Abrak and Our Mission

**Pardazesh-e Rahkar-haye Hooshmand-e Kasb-o-Kar** (commercially operating as **Abrak** / **ABRAK CO**) designs, engineers, and operates modern enterprise resource planning (ERP) platforms tailored specifically for Iranian manufacturers, commercial enterprises, service providers, and knowledge-based technology companies.

Mainstream open-source ERP systems are fundamentally built around Western accounting conventions, Gregorian calendars, and international banking infrastructures. In the Iranian business ecosystem, adapting such platforms has historically involved unstable third-party scripts, patchy translations, and recurring integration breakdowns.

Abrak resolves this disconnect through an engineering-led **Zero-Core-Hack** methodology: we keep upstream engine cores clean, pure, and untouched, delivering all localized accounting, compliance, calendar, and infrastructural extensions through a decoupled, modular addon layer.

The Abrak enterprise portfolio encompasses two core platforms:
- **[abrak.org](https://abrak.org)**: A turnkey enterprise SaaS platform based on **Odoo 19**, featuring true multi-tenant provisioning on Kubernetes alongside dedicated private deployments.
- **[zdr.ir](https://zdr.ir)**: The **NexERP** suite, built upon Frappe and ERPNext, designed for organizations seeking that technological stack.

---

## 2. What We Solve

Enterprise teams operating in Iran face unique regulatory, statutory, and infrastructural requirements that global enterprise software cannot address out of the box.

Abrak bridges this divide with hardened, production-tested software modules:

| Challenge in the Iranian Enterprise Market | Abrak's Integrated Engineering Solution |
|---|---|
| **Statutory Accounting & Financial Books:** Standard ERP charts of accounts and financial reports conflict with national statutory standards. | Full Iranian chart of accounts, general ledger, subsidiary ledgers, fiscal year closing routines, and statutory financial reporting built natively for Odoo 19. |
| **Moadian E-Invoicing Mandate:** Complex cryptographic signing, dynamic invoice schema changes, and high penalties for misfiling. | Dedicated Moadian preparation and drafting module: handles cryptographic payload structure, schema validation, and structured drafts without automated or unverified filing. |
| **Jalali Calendar & Date Calculations:** Surface-level UI date masks fail inside database queries, financial accruals, and scheduling engines. | Proprietary **Jalali Pro** engine deeply integrated at the database, business logic, ORM, and reporting layers, guaranteeing leap-year precision throughout all modules. |
| **Domestic Telephony & Messaging:** Lack of native connectors for Iranian SMS providers, VoIP operators, and local delivery networks. | Pre-configured, resilient connectors for Iranian enterprise SMS gateways, cloud PBX/VoIP telephony, and domestic shipping carriers. |
| **Banking & Payment Gateways:** Disconnect between foreign payment modules and the domestic Shaparak banking network. | Secure gateway integrations for Iranian commercial banks and online payment aggregators with automated transaction reconciliation. |
| **RTL Layouts & Printed Documents:** Broken text rendering, inverted tables, and misaligned PDF invoices in right-to-left languages. | Ground-up native right-to-left (RTL) typography, responsive views, interactive dashboards, and pixel-perfect PDF document templates. |
| **Infrastructure Overhead & Upgrades:** Heavy operational burden of maintaining servers, clustering, backups, and software lifecycle updates. | Fully managed multi-tenant SaaS running on scalable cloud infrastructure with automated health monitoring and rapid disaster recovery. |

---

## 3. High-Level Architecture & Technical Foundation

The Abrak platform architecture prioritizes data privacy, system resilience, enterprise security, and long-term upgradeability:

```
+-----------------------------------------------------------------------------------+
|                           Presentation & Interface Layer                          |
|         Web Portal (abrak.org) · RTL Engine · Abrak AI & MCP Assistants           |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                              Application Core Layer                               |
|        Upstream Odoo 19 Engine + Modular Localization Ecosystem (Addons)          |
|    Iran Accounting · Jalali Pro · Moadian Drafting · Communications Connectors    |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                            Multi-Tenancy & Isolation                              |
|           Database-Level Tenant Isolation (Dedicated Schema & Storage)            |
|               Strict Zero-Core-Hack Standard for Frictionless Upgrades            |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                       Cloud Infrastructure & Resilience                           |
|         Containerized Workloads on Kubernetes · Multi-Tenant & Dedicated          |
|        Rigorous Cold & Hot Backup Policies · Documented Disaster Recovery         |
+-----------------------------------------------------------------------------------+
```

- **Clean Upstream Foundation:** We build on vanilla upstream Odoo 19 releases without modifying core source code, guaranteeing smooth upstream security patching and long-term version migrations.
- **Strict Multi-Tenant Isolation:** Each customer runs in complete isolation with a dedicated database. Data leakage across tenants is architecturally precluded.
- **Modern Cloud Orchestration:** Production workloads are deployed on containerized Kubernetes infrastructure, supporting zero-downtime rolling updates, automated recovery, and dynamic load balancing. Dedicated single-tenant infrastructure is provided for enterprise clients with heightened isolation requirements.
- **Comprehensive Backup & Disaster Recovery (BDR):** Standing hot and cold backup routines, offsite retention policies, and rehearsed restoration playbooks protect business data continuity.
- **Intelligent Operations Layer:** Integration with AI agents, natural language interfaces, Model Context Protocol (MCP) endpoints, and automated pipelines under strict organizational data governance.

---

## 4. Functional Capabilities

| Functional Domain | Core Capabilities |
|---|---|
| **Iranian Statutory Accounting** | Multi-level chart of accounts, legal ledgers, trial balance, automated fiscal year closing, fixed assets and statutory depreciation schedules. |
| **Moadian Tax E-Invoicing** | Cryptographic key pairing, unique invoice identifier generation, pattern and schema validation, and structured draft preparation prior to formal sign-off. |
| **Jalali Pro Calendar Engine** | End-to-end Solar Hijri support across models, database queries, holiday schedules, period-based financial reports, and custom date widgets. |
| **SMS Notification System** | Service-line SMS delivery via webhooks, automated customer order alerts, dispatch notifications, and transactional verification workflows. |
| **Cloud PBX & VoIP Telephony** | Integration with Iranian cloud telephony providers, inbound caller identification cards, call logging, and seamless CRM customer history matching. |
| **Payment Gateway Connectors** | Digital payment links, native Shaparak gateway connectivity, and automated invoice reconciliation upon verified transaction callback. |
| **Quality Management (QMS)** | Proprietary **Chelopaz** subsystem for industrial catering, ensuring strict compliance with HACCP and ISO 22000 quality standards and food hygiene workflows. |
| **Bilingual RTL & Persian UX** | Clean business Persian typography, native RTL layout mechanics, and customized reporting templates in PDF and spreadsheet formats. |

---

## 5. Product & Repository Ecosystem

ABRAK CO is a commercial software vendor. In order to protect intellectual property, security boundaries, and enterprise client privacy, our core application source code is maintained in private repositories. Access is extended through formal partnership and customer agreements.

| Repository / Product | Scope & Functionality | Access Tier |
|---|---|---|
| `abrak-odoo-addons` | Core enterprise Odoo 19 addon suite (accounting, tax, communications, and multi-tenant tooling) | Private repository; access upon partnership agreement |
| `abrak-odoo-jalali-pro` | Commercial-grade Jalali (Persian) calendar engine for standard Odoo | Public repository |
| `abrak-calendar-pro` | Comprehensive Jalali calendar packaging compatible with Odoo versions 14 through 19 | Private repository; access upon partnership agreement |
| `abrak-enterprise-governance` | Organizational governance, compliance enforcement, and audit trail modules for enterprise Odoo | Private repository; access upon partnership agreement |
| `abrak-odoo-hub-connector-pro` | Central integration hub connecting external third-party software and legacy stacks to Odoo | Private repository; access upon partnership agreement |
| `abrak-connector-php` | PHP Software Development Kit (SDK) and API client for integrating web platforms with Abrak | Private repository; access upon partnership agreement |
| `abrak-connector-python` | Python SDK and API client for developers, data engineers, and third-party integrators | Private repository; access upon partnership agreement |
| `abrak-landing` | Official corporate web portal and marketing presence for abrak.org | Private repository; access upon partnership agreement |
| `abrak-docs` | Comprehensive multi-language technical documentation, deployment guides, and knowledge base | Public repository |
| `chelopaz` | Specialized Quality Management System (QMS) supporting HACCP and ISO 22000 for industrial food catering | Private repository; access upon partnership agreement |
| Abrak AI Platform | Enterprise conversational tooling, Open WebUI integrations, RTL/Jalali adaptation, MCP interfaces, and automated pipelines | Private repositories; access upon partnership agreement |

> *Security Note:* Internal operational repositories, clustering playbooks, and systems configuration code are maintained under strict internal security oversight and are excluded from public listings.

---

## 6. Engineering Standards & Security Practice

Quality, security, and predictability guide all engineering activities at Abrak:

- **Rigorous Peer Review:** Every code modification must undergo peer review, static code inspection, and architectural verification prior to branch merging.
- **Automated Testing & CI:** All modules are validated against automated test suites ensuring zero regression across core functionality.
- **Principle of Least Privilege (PoLP):** Granular role-based access control (RBAC), token isolation, and strict credential management across all services.
- **Backup-First Deployment Protocol:** Any configuration adjustment or code release on production customer environments requires a verified, fresh backup baseline.
- **Tax Compliance Principle (Drafting Only):** Our Moadian tooling strictly prepares, validates, and formats electronic invoice drafts. We enforce a zero-automatic-submission policy; all submissions must be explicitly reviewed and authorized by designated corporate financial officers.

---

## 7. Working With Us & Enterprise Inquiries

Abrak actively collaborates with knowledge-based enterprises, technology integrators, and software development teams:

- **Technical Partnerships:** Custom connector development, API integrations, and vertical-specific localization modules.
- **Private Repository Access:** Evaluation access to private addons and SDKs is provided under formal technical partnership agreements.
- **Enterprise Deployments:** Architecture consulting, dedicated multi-tenant infrastructure setup, and managed SaaS onboarding.

To initiate a partnership discussion or enterprise consultation, visit:
👉 [**Official Portal: abrak.org**](https://abrak.org)

---

## 8. Frequently Asked Questions (FAQ)

**Is Abrak an Odoo fork?**  
No. Abrak adheres to a strict Zero-Core-Hack philosophy. We utilize vanilla Odoo 19 and build our localized capabilities as modular addons. This guarantees full compatibility with standard community features and seamless future version upgrades.

**Is Abrak strictly a public SaaS, or can it be deployed on dedicated servers?**  
While our standard deployment model is multi-tenant SaaS on Kubernetes, we also provide dedicated private cloud and on-premise deployments for knowledge-based organizations and enterprises with strict data-residency mandates.

**How does Abrak integrate with Iran's Moadian tax authority?**  
Abrak provides end-to-end tooling to generate, validate, cryptographically sign, and prepare electronic invoices in compliance with tax authority schemas. The system operates strictly in a drafting capacity; it never files or submits data automatically without human financial authorization.

**What is the connection between abrak.org and zdr.ir?**  
Both platforms belong to the same technology family. While abrak.org delivers enterprise solutions based on Odoo 19, zdr.ir provides NexERP, powered by the Frappe/ERPNext framework, serving organizations whose architecture favors that stack.

**How can developers or enterprise partners gain access to private repositories?**  
Private repository access is extended to authorized technical partners, enterprise customers, and verified system integrators. Inquiries can be submitted directly through [abrak.org](https://abrak.org).

---

<div align="center">

`Odoo 19` · `ERPNext` · `NexERP` · `SaaS` · `Multi-Tenant` · `Kubernetes` · `Iran Localization` · `Jalali Calendar Pro` · `RTL Native` · `Moadian Invoicing Prep`

<sub>Engineered with pride in Iran · Built in Iran</sub>

</div>
