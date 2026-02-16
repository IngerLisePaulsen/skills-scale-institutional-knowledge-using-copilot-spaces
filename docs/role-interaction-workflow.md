# Role Interaction Workflow

This document illustrates how roles interact throughout the project lifecycle at OctoAcme.

---

## Project Initiation Workflow

```
┌─────────────────┐
│  Stakeholder    │
│   Request       │
└────────┬────────┘
         │
         ▼
┌─────────────────┐      ┌──────────────────┐
│ Product Manager │◄────►│ Data Analyst     │
│ (Define Value)  │      │ (Market Research)│
└────────┬────────┘      └──────────────────┘
         │
         ▼
┌─────────────────┐      ┌──────────────────┐
│ Product Manager │◄────►│ UX Lead          │
│ (Problem Stmt.) │      │ (User Research)  │
└────────┬────────┘      └──────────────────┘
         │
         ▼
┌─────────────────┐
│ Project Manager │
│ (Create Charter)│
└─────────────────┘
```

**Key Handoffs:**
1. Stakeholder → Product Manager: Business need and objectives
2. Product Manager ↔ Data Analyst: Market validation and metrics
3. Product Manager ↔ UX Lead: User needs and pain points
4. Product Manager → Project Manager: Approved scope and success criteria

---

## Planning & Design Workflow

```
┌─────────────────┐
│ Project Manager │
│ (Kickoff Meet.) │
└────────┬────────┘
         │
    ┌────┴────┐
    │         │
    ▼         ▼
┌─────────┐ ┌──────────────┐      ┌─────────────┐
│ Product │ │ UX Lead      │◄────►│ Data Analyst│
│ Manager │ │ (Wireframes) │      │ (Metrics)   │
└────┬────┘ └──────┬───────┘      └─────────────┘
     │             │
     │             ▼
     │      ┌──────────────┐
     │      │  Developers  │
     │      │ (Feasibility)│
     │      └──────┬───────┘
     │             │
     ▼             ▼
┌─────────────────────────┐
│  Backlog with Stories   │
│  and Acceptance Criteria│
└────────┬────────────────┘
         │
         ▼
┌─────────────────┐
│  QA Specialist  │
│ (Test Planning) │
└─────────────────┘
```

**Key Handoffs:**
1. Project Manager → All Roles: Project scope, timeline, constraints
2. UX Lead → Product Manager: Design concepts for validation
3. UX Lead → Developers: Feasibility review of designs
4. Product Manager → All: Prioritized backlog with acceptance criteria
5. Product Manager → QA Specialist: Expected behavior for test planning

---

## Development Workflow

```
┌─────────────────┐
│ Sprint Planning │
│ (Team + PM/PdM) │
└────────┬────────┘
         │
         ▼
┌─────────────────┐      ┌──────────────────┐
│   Developers    │◄────►│    UX Lead       │
│ (Implementation)│      │ (Design Support) │
└────────┬────────┘      └──────────────────┘
         │
         │ PR Created
         ▼
┌─────────────────┐
│   Code Review   │
│  (Developers)   │
└────────┬────────┘
         │
         │ Approved
         ▼
┌─────────────────┐      ┌──────────────────┐
│  QA Specialist  │◄────►│   Developers     │
│ (Test & Verify) │      │  (Bug Fixes)     │
└────────┬────────┘      └──────────────────┘
         │
         │ Passed
         ▼
┌─────────────────┐
│  Ready for      │
│  Deployment     │
└─────────────────┘
```

**Key Handoffs:**
1. Sprint Planning → Developers: Selected work items with clear criteria
2. Developers → UX Lead: Implementation questions on design intent
3. Developers → Developers: PR for code review
4. Developers → QA Specialist: Completed feature for validation
5. QA Specialist → Developers: Bug reports for fixes
6. QA Specialist → Project Manager: Quality sign-off

---

## Release Workflow

```
┌─────────────────┐      ┌──────────────────┐
│ Project Manager │◄────►│ Change Manager   │
│ (Release Plan)  │      │ (Impact Assess.) │
└────────┬────────┘      └────────┬─────────┘
         │                        │
         │                        ▼
         │               ┌──────────────────┐
         │               │  Training        │
         │               │  Materials       │
         │               └──────────────────┘
         │
         ▼
┌─────────────────┐
│  QA Specialist  │
│ (Smoke Testing) │
└────────┬────────┘
         │
         │ Approved
         ▼
┌─────────────────┐
│   Developers    │
│   (Deploy)      │
└────────┬────────┘
         │
         │ Deployed
         ▼
┌─────────────────┐      ┌──────────────────┐
│ Change Manager  │      │  Data Analyst    │
│ (Announce)      │      │ (Monitor Impact) │
└─────────────────┘      └──────────────────┘
```

**Key Handoffs:**
1. Project Manager → Change Manager: Release scope and timeline
2. Change Manager → Stakeholders: Training and readiness activities
3. QA Specialist → Project Manager: Quality sign-off for release
4. Developers → Production: Deployment execution
5. Change Manager → All Stakeholders: Release communication
6. Data Analyst → Product Manager: Post-release metrics and impact

---

## Continuous Feedback Loop

```
┌──────────────────────────────────────────┐
│          PRODUCTION                      │
└────────┬─────────────────────────────┬───┘
         │                             │
         ▼                             ▼
┌─────────────────┐            ┌──────────────────┐
│  Data Analyst   │            │  QA Specialist   │
│ (Usage Metrics) │            │ (Bug Reports)    │
└────────┬────────┘            └────────┬─────────┘
         │                              │
         ▼                              ▼
┌─────────────────┐            ┌──────────────────┐
│ Product Manager │            │  Developers      │
│ (Impact Review) │            │ (Hot Fixes)      │
└────────┬────────┘            └──────────────────┘
         │
         ▼
┌─────────────────┐            ┌──────────────────┐
│ Change Manager  │◄──────────►│ Project Manager  │
│ (User Feedback) │            │ (Retrospective)  │
└─────────────────┘            └──────────────────┘
         │
         ▼
┌──────────────────────────────────────────┐
│     BACKLOG (Next Iteration)             │
└──────────────────────────────────────────┘
```

**Key Feedback Loops:**
1. Data Analyst → Product Manager: Usage data and success metrics
2. QA Specialist → Developers: Production defects
3. Change Manager → Product Manager: User feedback and adoption challenges
4. Project Manager → All: Retrospective findings and improvements
5. All inputs → Backlog: Inform next iteration priorities

---

## Cross-Functional Collaboration Patterns

### Daily Pattern
- **Standup**: All delivery team members (Developers, UX Lead, QA Specialist) + Project Manager
- **Ad-hoc**: Role pairs collaborate on specific issues

### Weekly Pattern
- **PM/PdM Sync**: Project Manager ↔ Product Manager (priorities, risks, scope)
- **Metrics Review**: Product Manager ↔ Data Analyst (success metrics, insights)
- **Design Review**: UX Lead → Product Manager + Developers (design validation)
- **Status Update**: Project Manager → Stakeholders (progress, risks)

### Sprint/Iteration Pattern
- **Planning**: All roles participate in backlog refinement and sprint planning
- **Demo**: Product Manager, UX Lead, and Developers showcase to stakeholders
- **Retrospective**: All roles reflect and identify improvements

---

## Escalation Workflow

```
┌─────────────────┐
│    Blocker      │
│   Identified    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Level 1: Team   │ ◄── Daily Standup
│ (15 min triage) │
└────────┬────────┘
         │
         │ Unresolved
         ▼
┌─────────────────┐
│ Level 2: PM/PdM │ ◄── Same Day
│ (Decision/Trade)│
└────────┬────────┘
         │
         │ Unresolved
         ▼
┌─────────────────┐
│ Level 3: Sponsor│ ◄── Within 24 hrs
│ (Business Call) │
└─────────────────┘
```

---

## Key Principles

1. **Clear Handoffs**: Each transition point has an explicit owner and recipient
2. **Bidirectional Communication**: Most interactions are two-way collaboration, not one-way handoffs
3. **Continuous Feedback**: Information flows back to earlier stages to inform decisions
4. **Defined Escalation**: Blockers follow a clear path with timeboxed resolution
5. **Regular Cadence**: Scheduled touchpoints prevent bottlenecks and maintain alignment

---

## Using This Workflow

- **For Onboarding**: New team members can trace their role through the entire lifecycle
- **For Planning**: Teams can identify which roles need to be engaged at each phase
- **For Retrospectives**: Use to identify handoff bottlenecks or communication gaps
- **For Scaling**: Understand dependencies when adding team members or projects
