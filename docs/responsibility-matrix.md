# Responsibility Matrix (RACI)

This matrix defines accountability for key project activities using the RACI model:
- **R** = Responsible (does the work)
- **A** = Accountable (ultimately answerable, approves)
- **C** = Consulted (provides input)
- **I** = Informed (kept up to date)

---

## Project Lifecycle Activities

| Activity | Project Manager | Product Manager | Developer | UX Lead | QA Specialist | Data Analyst | Change Manager |
|----------|----------------|-----------------|-----------|---------|---------------|--------------|----------------|
| **Initiation & Planning** |
| Define project scope | C | A | C | C | C | C | I |
| Create project charter | R/A | C | C | I | I | I | C |
| Define success metrics | C | A | I | I | C | R | I |
| Identify stakeholders | R | C | I | I | I | I | A |
| Create project timeline | A | C | C | I | C | I | C |
| Risk identification | A | C | C | C | C | C | C |
| **Requirements & Design** |
| Define user stories | C | A | C | R | C | I | I |
| User research | I | C | I | A/R | I | C | C |
| Design UI/UX | I | C | C | A/R | I | I | I |
| Define acceptance criteria | C | A | R | C | R | I | I |
| Technical design | C | C | A/R | C | I | I | I |
| **Execution** |
| Implement features | I | I | A/R | C | I | I | I |
| Code review | I | I | A/R | I | I | I | I |
| Write unit tests | I | I | A/R | I | C | I | I |
| Design review | I | C | C | A/R | I | I | I |
| Integration testing | C | I | R | I | A | I | I |
| Feature validation | C | C | C | C | A/R | I | I |
| Usability testing | I | C | I | R | R | I | I |
| Track project progress | A/R | C | C | I | I | I | I |
| Remove blockers | A/R | C | C | I | C | I | C |
| **Monitoring & Reporting** |
| Status reporting | A/R | C | I | I | I | C | C |
| Track velocity | A/R | C | I | I | I | C | I |
| Monitor quality metrics | C | C | I | I | A/R | C | I |
| Analytics & insights | I | C | I | I | I | A/R | I |
| Dashboard maintenance | I | C | I | I | C | A/R | I |
| Risk register updates | A/R | C | C | C | C | C | C |
| **Release & Deployment** |
| Release planning | A | C | C | C | C | I | R |
| Deployment execution | C | I | A/R | I | C | I | I |
| Release communication | C | C | I | I | I | I | A/R |
| Training materials | I | C | C | C | C | I | A/R |
| Smoke testing | I | I | C | I | A/R | I | I |
| Production monitoring | C | C | R | I | R | A | C |
| **Continuous Improvement** |
| Retrospective facilitation | A/R | C | C | C | C | C | C |
| Process improvements | A | C | C | C | C | C | C |
| Change adoption tracking | C | C | I | I | I | C | A/R |
| Documentation updates | R | C | C | C | C | C | C |

---

## Key Decision Authority

| Decision Type | Primary Authority | Consulted | Informed |
|---------------|------------------|-----------|----------|
| Feature prioritization | Product Manager | Project Manager, UX Lead, Data Analyst | All team |
| Scope changes | Product Manager, Project Manager | Developers, QA Specialist | Stakeholders |
| Technical approach | Developers | UX Lead, Product Manager | Project Manager |
| Release timing | Project Manager | Product Manager, QA Specialist, Change Manager | All team |
| Design direction | UX Lead | Product Manager, Developers | Project Manager |
| Quality standards | QA Specialist | Developers, Project Manager | Product Manager |
| Risk mitigation plans | Project Manager | Product Manager, relevant role owners | Stakeholders |
| Change management approach | Change Manager | Project Manager, Product Manager | All team |
| Success metric definitions | Product Manager | Data Analyst, Project Manager | All team |

---

## Escalation Path for Blockers

1. **Team Level**: Raised in daily standup
   - Developer, UX Lead, QA Specialist, Data Analyst raise to Project Manager
   
2. **Management Level**: Escalated by Project Manager
   - Project Manager escalates to Product Manager for priority/scope decisions
   - Product Manager and Project Manager jointly escalate to sponsors
   
3. **Executive Level**: For business-impacting issues
   - Sponsors make final decisions on major scope, timeline, or resource changes

---

## Communication Ownership

| Communication Type | Owner | Contributors | Recipients |
|-------------------|-------|--------------|------------|
| Daily standups | Project Manager | All team members | Team |
| Sprint planning | Project Manager | Product Manager, Team | Team |
| Status updates | Project Manager | All roles | Stakeholders |
| Roadmap updates | Product Manager | Data Analyst, UX Lead | Stakeholders |
| Design reviews | UX Lead | Product Manager, Developers | Project Manager, QA |
| Bug triage | QA Specialist | Developers | Project Manager |
| Metrics reviews | Data Analyst | Product Manager | Project Manager, Team |
| Release notes | Change Manager | Product Manager, Developers | All stakeholders |
| Retrospectives | Project Manager | All team members | Team |

---

## Notes

- When multiple roles share A (Accountable), they are jointly accountable and must coordinate
- R/A indicates the role is both Responsible for execution and Accountable for outcomes
- This matrix serves as a guideline; specific projects may adjust based on team composition
- Role owners should proactively communicate when accountabilities overlap or are unclear
