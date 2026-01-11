# Service Ownership Charter

> **"You Build It, You Own It"**

---

## 1. Vision

To enable **high-velocity Continuous Delivery**, we shift from a centralized "Gatekeeper" model to a **Decentralized Ownership** model.

Squads are empowered as **autonomous mini-startups** that own the full lifecycle of their services.

---

## 2. The Responsibility Matrix

| Phase | Platform Team | Product Squad |
|:------|:--------------|:--------------|
| **Design** | Provides Architecture RFC Templates | Owns System Design & Monolith Decoupling |
| **Develop** | Provides AI-assisted linting & CI tools | Owns Code Quality & **85% Test Coverage** |
| **Deploy** | Owns CI/CD Pipeline Infrastructure | Owns Deployment Frequency & Release Health |
| **Operate** | Provides Observability Stack (Logs/Metrics) | Owns On-call, MTTR, and Incident Response |

### Role Clarity

| | Platform Team | Product Squad |
|:--|:--------------|:--------------|
| **Analogy** | The Paved Road | The Driver |
| **Focus** | Infrastructure & Tooling | Business Value & Service Health |

---

## 3. Definition of Done for Ownership

Before a service is considered **"Owned"** by a squad and ready for production, it must meet these criteria:

### Observability
- [ ] Standard dashboards for **DORA metrics** are active:
  - Deployment Frequency
  - Lead Time for Changes
  - Change Failure Rate
  - Mean Time to Recovery (MTTR)

### Quality Gates
- [ ] Unit test coverage is at **63.4%+ overall**
- [ ] Unit test coverage is at **85%+ for new logic**

### Efficiency
- [ ] Code duplication is maintained **below 2%**
- [ ] Current target: **1.7%**

### Security
- [ ] AI-assisted PR reviews are operational
- [ ] Goal: Reduce staging defects through automated analysis

### Documentation
- [ ] API documentation is updated
- [ ] Integration with central catalog is complete

---

## 4. Incident & Problem Management

> **Ownership means accountability.**

When a production incident occurs:

### Response
The owning squad **leads the restoration of service**.

### Postmortem
A **blameless postmortem** is conducted to identify root causes.

### Prevention
The squad prioritizes **"Prevention-Focused"** tasks to ensure the same issue never recurs.

---

## Quick Reference

```
┌─────────────────────────────────────────────────────────────┐
│                    OWNERSHIP LIFECYCLE                       │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   DESIGN  ──►  DEVELOP  ──►  DEPLOY  ──►  OPERATE          │
│      │            │            │            │               │
│      ▼            ▼            ▼            ▼               │
│   RFC &       Code &       Release &    Monitor &          │
│   Architecture Testing     Pipeline     Respond            │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Key Metrics

| Metric | Target | Purpose |
|:-------|:-------|:--------|
| Test Coverage (Overall) | ≥ 63.4% | Baseline quality assurance |
| Test Coverage (New Code) | ≥ 85% | Prevent regression |
| Code Duplication | < 2% | Maintainability |
| MTTR | Minimize | Operational excellence |
| Deployment Frequency | Maximize | Delivery velocity |

---

## Principles

1. **Autonomy with Accountability** — Squads have freedom to make decisions but own the outcomes
2. **Shift Left** — Catch issues early through automated quality gates
3. **Blameless Culture** — Focus on systems improvement, not individual fault
4. **Continuous Improvement** — Every incident is a learning opportunity

---

<sub>Engineering Operating System — Vadym Shukurov</sub>
