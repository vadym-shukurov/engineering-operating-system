# Service Ownership Charter: Scaling Autonomy through Governance

> **"You Build It, You Own It, You Love It."**
> This charter defines the strategic contract between Platform and Product squads. It is designed to maximize delivery velocity through Continuous Delivery while maintaining a 20% YoY reduction in production incidents through strict accountability and engineering excellence.

---

## 1. The Ownership Maturity Model
We recognize that ownership is a journey. Squads are evaluated against this maturity matrix to determine their level of autonomy and investment needs.

| Level | Status | Characteristics |
| :--- | :--- | :--- |
| **L1** | **Reactive** | Squad handles bugs; relies on Platform for deployment and monitoring setup. |
| **L2** | **Proactive** | Squad owns their CI/CD pipelines and monitors their own DORA dashboards. |
| **L3** | **Strategic** | Full lifecycle ownership: 3-5 year architectural roadmap, on-call, and SLO/Error Budget management. |



---

## 2. The "Paved Road" Responsibility Matrix
To enable independent team delivery for ~50 engineers across 10 squads, we use a "Paved Road" model where the Platform team provides the tools and the Squads drive the execution.

| Phase | Platform Team (Enablers) | Product Squad (Owners) |
| :--- | :--- | :--- |
| **Design** | Provides Architecture RFC & ADR Templates. | Owns System Design & Monolith Decoupling. |
| **Develop** | Provides AI-assisted linting & CI guardrails. | Owns Test Pyramid health (85% coverage on new code). |
| **Deploy** | Owns Infrastructure as Code (IaC) & CD tooling. | Owns Deployment Frequency & Small-Batch releases. |
| **Operate** | Provides Observability Stack (Logs/Metrics). | Owns On-call, MTTR, and Incident Postmortems. |

---

## 3. Definition of Done (DoD) for Service Ownership
Before a service is classified as "Squad Owned," it must meet these elite engineering standards:

### 🏗️ Architectural & Quality Gates
* **RFC Alignment:** Major changes must have an approved RFC to ensure alignment with the 3-5 year strategy.
* **The Test Pyramid:** Maintain a healthy balance-85%+ Unit coverage on new logic, 100% API coverage, and ~92% E2E coverage for critical journeys.
* **AI-Driven Shift-Left:** All PRs must pass automated AI-assisted quality scans to reduce staging defects by ~50%.
* **Exploratory Testing:** Squads must conduct exploratory testing sessions to complement automation for high-risk features.



<img width="2048" height="1639" alt="image" src="https://github.com/user-attachments/assets/2872b3cc-5258-4bcf-b739-2a0adf554037" />



### 📈 Operational Excellence (DORA Metrics)
* **Velocity:** Small-batch delivery to support a predictable ~2-week (or faster) release heartbeat.
* **Reliability:** Maintain zero critical security vulnerabilities and code duplication below 1.7%.
* **Observability:** Active monitoring for MTTR, Error Budgets, and Change Failure Rates.

---

## 4. The Economics of Engineering: Resource Allocation
As leaders, we treat engineering capacity as a strategic investment. We aim for the following allocation within owned squads:
* **70% Feature Innovation:** Driving new business value and customer satisfaction.
* **20% Technical Sustainability:** Reducing tech debt, improving coverage, and monolith decoupling.
* **10% Exploration:** R&D, AI-tooling experiments, and process optimization.

---

## 5. Incident Prevention & "Blameless" Culture
Ownership means accountability without fear. When a production incident occurs:
1. **Restore:** The owning squad leads the restoration.
2. **Analyze:** Conduct a blameless postmortem focused on systemic failure, not individual error.
3. **Prevent:** Prioritize "Prevention-Focused" tasks to ensure the same issue never recurs, aiming for a 20% YoY reduction in incidents.

---
<sub>**Engineering Operating System** | Authored by Vadym Shukurov | Head of Engineering</sub>
