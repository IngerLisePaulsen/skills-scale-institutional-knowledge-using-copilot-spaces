# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one Developer approval before merging (or team-defined policy)
  - UX Lead reviews UI/UX changes before merge
  - QA Specialist validates acceptance criteria before production deployment

## Quality & Testing
- Unit tests for new logic (Developer responsibility)
- Integration tests where applicable (Developer and QA Specialist collaboration)
- End-to-end smoke tests for critical flows before release (QA Specialist leads)
- Security scanning in CI (automated with Developer and QA review)
- Manual QA for feature acceptance when needed (QA Specialist validates)
- Usability testing for UI changes (UX Lead coordinates with QA Specialist)

## Reporting & Metrics
- Track velocity and burndown (Project Manager responsibility)
- Monitor success metrics identified in the Project One-pager (Data Analyst provides reports)
- Use dashboards for key signals: errors, latency, usage (Data Analyst maintains)
- Report on quality metrics and defect trends (QA Specialist tracks)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

---

## Additional Resources

For comprehensive QA and testing procedures, see the [QA Process Checklist](template-qa-process-checklist.md) (addresses Issue #4 gap).

For release planning and deployment procedures, see the [Release Management Checklist](template-release-management-checklist.md) (addresses Issue #4 gap).

---

*This guide updated to reference new standardized templates from Issue #4 improvements.*
