# Agentic CRM: Executive Product Portfolio

Welcome. This repository serves as the public-facing portfolio for **Agentic CRM**, a scalable, hybrid-cloud enterprise application built to demonstrate some of my technical product management capabilities.

▶️ **[Watch the Agentic CRM Prototype Video Walkthrough](./agentic_crm_prototype_walkthrough.mp4)**

## 🚀 Core Product Features

Agentic CRM integrates autonomous AI orchestration into the traditional sales lifecycle via three distinct, event-driven workflows:

*   **AI Intent Scoring:** Intercepts inbound CRM webhooks to automatically categorize new leads, querying LLMs to calculate conversion probability and industry fit before human intervention.
*   **Account Executive View:** A real-time Smart Canvas UI. It utilizes Server-Sent Events (SSE) and an MCP sidecar to securely stream AI insights—such as auto-drafted Gmail responses and activity timelines—directly to the sales team without contaminating the core CRM database.
*   **Executive Co-Pilot:** A conversational chatbot interface enabling leadership to query pipeline data, forecast revenue, and retrieve AI-generated insights via natural language, powered by the isolated AI metadata vault.

## 🏗️ Architecture Overview (AGPL-3.0 Compliance)

Agentic CRM is built as an orchestration layer on top of **TwentyCRM**, a powerful open-source CRM. To strictly comply with TwentyCRM's AGPL-3.0 copyleft license, the AI Orchestrator is architected as a fully isolated, decoupled microservice. It communicates with the TwentyCRM exclusively via standard webhooks and the Model Context Protocol (MCP), ensuring that the proprietary AI logic, intent-scoring models, and enterprise infrastructure remain legally distinct and protected from open-source contamination.

## 🔒 Intellectual Property & Gating Strategy

Due to the proprietary nature of the AI orchestration logic, the intent-scoring mechanisms, and the strict isolation boundaries protecting against open-source copyleft (AGPL-3.0) contamination, the codebase is gated for the time being to prevent IP leakage and reverse-engineering.

If you are a Hiring Manager or Director of Product, **I invite you to request an interview** where I will gladly walk you through the software architecture, proprietary system logic, and live deployment.

---

## 📑 Portfolio Contents

In lieu of the source code, this repository contains four executive documents that showcase the strategic product management decisions, unit economics, and architectural scaling designed for this product.

Please kindly review the following documents:

### 1. [Product Management Judgement Showcase](./product_judgement_showcase.md)
A curated log of executive-level decisions made during the development lifecycle. 

### 2. [Architecture Evolution Delta](./architecture_evolution_delta.md)
A breakdown of how the architecture pivoted from a simple prototype to a more resilient, enterprise-grade hybrid-cloud deployment. 

### 3. [Unit Economics & Scalability](./unit_economics_and_scalability.md)
A detailed analysis of how the system achieves a sub-$60/month Total Cost of Ownership (TCO) through strict resource allocation. 

### 4. [Defensibility & Moat Analysis](./defensibility_and_moat_analysis.md)
A summary of the strategic "moats" built into the product.

---

## 📊 Proof of Unit Economics

To substantiate the cost-saving claims made in the documentation, please review the service-level GCP billing dashboard screenshot:
* **[View GCP Billing Proof (Service Level)](./gcp_billing_by_service.jpg)**

This visual proof confirms that heavy monolithic compute is successfully running locally, while the only incurred costs are the AI telemetry caching and storage layers.

---

## 📬 Contact for Technical Review
To see the actual code, review the master architecture diagrams, or discuss how I can bring my skills and experience to your engineering teams, please reach out to schedule an interview.  I can be reached at hello@syed-nasir.dev.
