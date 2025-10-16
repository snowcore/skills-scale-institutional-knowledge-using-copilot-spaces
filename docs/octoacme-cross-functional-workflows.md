# OctoAcme — Cross-Functional Workflows & Communication

## Purpose
Define clear workflows and communication patterns for cross-functional collaboration to ensure efficient handoffs, shared accountability, and streamlined delivery.

## Core Collaboration Patterns

### Feature Development Workflow

This workflow describes how different roles collaborate from feature conception to production release.

#### Phase 1: Discovery & Definition
- **Product Manager** → Defines problem statement, success metrics, and high-level requirements
- **Data Analyst** → Provides baseline metrics and insights from user behavior analysis
- **Support Lead** → Shares customer feedback, pain points, and feature requests
- **UX Designer** → Conducts user research and validates problem with users
- **Leads to**: Approved feature concept with clear success criteria

#### Phase 2: Design & Planning
- **UX Designer** → Creates wireframes, prototypes, and design specifications
- **Product Manager** → Reviews and approves designs, writes user stories
- **Developers** → Review technical feasibility, estimate effort, identify dependencies
- **DevOps Engineer** → Identifies infrastructure requirements and deployment considerations
- **Data Analyst** → Defines instrumentation requirements for tracking success metrics
- **Project Manager** → Creates project plan, timeline, and coordinates resources
- **Leads to**: Prioritized backlog with design specs, acceptance criteria, and estimates

#### Phase 3: Development & Testing
- **Developers** → Implement features according to design specs and acceptance criteria
- **UX Designer** → Reviews implementation for design fidelity and accessibility
- **DevOps Engineer** → Builds CI/CD pipeline, configures infrastructure
- **Data Analyst** → Validates instrumentation and data collection
- **QA/Testing** → Validates functionality against acceptance criteria
- **Project Manager** → Tracks progress, manages risks, facilitates standups
- **Leads to**: Feature complete and ready for release

#### Phase 4: Release & Validation
- **DevOps Engineer** → Deploys to production, monitors system health
- **Developers** → Verify deployment, monitor for errors
- **Support Lead** → Updates documentation, prepares support team
- **Product Manager** → Announces feature, communicates to stakeholders
- **Data Analyst** → Tracks launch metrics and prepares initial impact analysis
- **Leads to**: Feature live in production with monitoring enabled

#### Phase 5: Post-Launch Analysis
- **Data Analyst** → Analyzes feature impact, A/B test results, and success metrics
- **Support Lead** → Tracks support volume, user feedback, and issues
- **Product Manager** → Reviews success metrics and gathers stakeholder feedback
- **UX Designer** → Conducts usability testing and collects user feedback
- **Leads to**: Retrospective insights and iteration priorities

---

## Communication Matrix

### Daily Communications
| Role | Stakeholders | Purpose | Format |
|------|--------------|---------|--------|
| Developers | Team, Project Manager | Share progress, identify blockers | Standup |
| DevOps Engineer | Developers, Project Manager | Infrastructure status, deployment updates | Standup, Slack |
| Support Lead | Support Team, Product Manager | Urgent escalations, critical issues | Ticket queue, Slack |

### Weekly Communications
| Role | Stakeholders | Purpose | Format |
|------|--------------|---------|--------|
| Project Manager | All team roles, Stakeholders | Project status, risks, decisions | Status update, Meeting |
| Product Manager | UX Designer, Developers, Data Analyst | Roadmap alignment, feature prioritization | Sync meeting |
| UX Designer | Product Manager, Developers | Design reviews, implementation feedback | Design review |
| Data Analyst | Product Manager, Project Manager | Metrics review, experiment results | Dashboard review |
| Support Lead | Product Manager, Engineering | Support trends, escalations, user feedback | Metrics report |
| DevOps Engineer | Developers, Project Manager | Infrastructure health, deployment capacity | Operations sync |

### Monthly Communications
| Role | Stakeholders | Purpose | Format |
|------|--------------|---------|--------|
| Product Manager | Leadership, Stakeholders | Strategic updates, roadmap progress | Presentation |
| Data Analyst | Leadership, Product Manager | Business metrics, trends, insights | Dashboard + Report |
| Support Lead | Leadership, Product Manager | Support metrics, satisfaction scores | Report |

---

## Cross-Functional Checklists

### Feature Kickoff Checklist
Use this checklist when starting a new feature to ensure all roles are aligned.

- [ ] **Product Manager**: Problem statement and success metrics defined
- [ ] **Data Analyst**: Baseline metrics collected and shared
- [ ] **Support Lead**: Customer feedback and pain points documented
- [ ] **UX Designer**: User research plan created (if needed)
- [ ] **Project Manager**: Stakeholders identified and kickoff scheduled
- [ ] **DevOps Engineer**: Infrastructure requirements identified
- [ ] **Developers**: Technical approach reviewed
- [ ] All: Kickoff meeting held with notes documented

### Design Handoff Checklist
Ensure smooth transition from design to development.

- [ ] **UX Designer**: Design specifications complete and accessible
- [ ] **UX Designer**: Interactive prototypes available (if applicable)
- [ ] **UX Designer**: Accessibility requirements documented
- [ ] **Data Analyst**: Analytics instrumentation requirements defined
- [ ] **Developers**: Design specifications reviewed and understood
- [ ] **Developers**: Technical questions answered
- [ ] **Product Manager**: Acceptance criteria aligned with designs
- [ ] All: Design review meeting held

### Pre-Release Checklist
Verify readiness before deploying to production.

- [ ] **Developers**: All acceptance criteria met
- [ ] **Developers**: Automated tests passing
- [ ] **QA/Testing**: Manual testing complete
- [ ] **UX Designer**: Design implementation reviewed
- [ ] **Data Analyst**: Analytics instrumentation verified
- [ ] **DevOps Engineer**: Deployment plan reviewed
- [ ] **DevOps Engineer**: Rollback plan documented
- [ ] **Support Lead**: Support documentation updated
- [ ] **Support Lead**: Support team trained on new feature
- [ ] **Product Manager**: Release notes drafted
- [ ] **Project Manager**: Stakeholders informed of release timing

### Post-Release Checklist
Ensure successful launch and gather learnings.

- [ ] **DevOps Engineer**: Production deployment successful
- [ ] **DevOps Engineer**: Monitoring and alerts verified
- [ ] **Developers**: Post-deploy smoke tests passed
- [ ] **Support Lead**: No critical support escalations
- [ ] **Data Analyst**: Metrics collection validated
- [ ] **Product Manager**: Stakeholders notified of launch
- [ ] **Data Analyst** (Week 1): Initial metrics report shared
- [ ] **Support Lead** (Week 1): Support feedback collected
- [ ] **Product Manager** (Week 2): Success metrics reviewed
- [ ] **Project Manager**: Retrospective scheduled

---

## Escalation Paths

### Technical Issues
1. **Developer** identifies issue → Escalates to **Tech Lead**
2. **Tech Lead** unable to resolve → Escalates to **DevOps Engineer** (infrastructure) or **Project Manager** (timeline impact)
3. Critical production issue → **DevOps Engineer** initiates incident response, notifies **Support Lead** and **Product Manager**

### Product/Design Issues
1. **UX Designer** or **Developer** identifies design-implementation gap → Discuss in daily standup or design review
2. Unresolved → Escalate to **Product Manager** for prioritization decision
3. Impacts timeline → **Project Manager** assesses and communicates to stakeholders

### Customer Issues
1. **Support Lead** triages issue → Routes to appropriate team (Bug → Developers, Feature request → Product Manager)
2. Critical issue → **Support Lead** escalates to **Product Manager** and **Project Manager**
3. Impacts multiple customers → **Product Manager** prioritizes and coordinates response

### Data/Metrics Issues
1. **Data Analyst** identifies data quality issue → Coordinates with **Developers** to fix instrumentation
2. Metrics showing negative trend → **Data Analyst** alerts **Product Manager** for investigation
3. Business-critical metric issue → **Data Analyst** escalates to **Product Manager** and leadership

---

## Best Practices for Cross-Functional Collaboration

### For All Roles
- Default to transparency: share work-in-progress and blockers early
- Document decisions in shared, accessible locations
- Respect role boundaries while maintaining open communication
- Participate in retrospectives to improve collaboration

### Asynchronous Communication
- Use threaded conversations in team channels
- Include context and links in messages
- Tag relevant people but avoid unnecessary notifications
- Set clear expectations for response times

### Meetings
- Create agendas in advance
- Start and end on time
- Document decisions and action items
- Record when appropriate for those who can't attend

### Documentation
- Keep project documentation in the repository
- Use templates and checklists for consistency
- Update documentation as decisions change
- Add process docs to `.copilot/` for AI context

---

## Using This Guide

1. **Starting a project?** Reference the Feature Development Workflow and Feature Kickoff Checklist
2. **Unclear on handoffs?** Review the Communication Matrix for your role
3. **Issue needs escalation?** Follow the relevant Escalation Path
4. **Process breakdown?** Use the Cross-Functional Checklists to identify gaps
5. **Improving collaboration?** Share this document and gather feedback in retrospectives

---

**Questions or suggestions?** This is a living document. Propose improvements through pull requests or discuss with your Project Manager.
