# OctoAcme — Cross-Functional Collaboration Guide

## Purpose
Clarify how OctoAcme personas interact, depend on each other, and collaborate to deliver successful projects. This guide addresses gaps in coordination between expanded roles.

## Core Collaboration Flows

### Project Initiation
**Involved Roles**: Product Manager, Project Manager, Stakeholder/Sponsor, Technical Lead

- **Product Manager** & **Stakeholder/Sponsor**: Define problem statement, business goals, and success metrics
- **Project Manager**: Creates initial timeline and identifies dependencies
- **Technical Lead**: Assesses technical feasibility and identifies architectural concerns
- **Outcome**: Project Charter/One-pager approved (see octoacme-project-initiation.md)

### Planning & Design
**Involved Roles**: Product Manager, Developers, UX/Design, Technical Lead, Scrum Master

- **UX/Design**: Conducts user research, creates wireframes and prototypes
- **Product Manager**: Defines acceptance criteria and prioritizes features
- **Technical Lead**: Reviews design for technical feasibility, identifies architectural needs
- **Developers**: Provide estimation and identify implementation risks
- **Scrum Master**: Facilitates planning ceremonies and ensures team capacity is respected
- **Outcome**: Prioritized backlog with clear acceptance criteria and technical constraints

### Execution & Quality Assurance
**Involved Roles**: Developers, QA/Testing Engineer, Technical Lead, UX/Design, Scrum Master

- **Developers**: Implement features, write tests, request code reviews
- **Technical Lead**: Conducts code/design reviews, mentors on best practices
- **QA/Testing Engineer**: Executes test plans, validates acceptance criteria, identifies defects
- **UX/Design**: Reviews implementation against design specs, validates usability
- **Scrum Master**: Removes blockers, facilitates standups, tracks progress
- **Outcome**: Features meet Definition of Done and are ready for review

### Review & Approval
**Involved Roles**: Product Manager, QA/Testing Engineer, Technical Lead, Stakeholder/Sponsor

- **QA/Testing Engineer**: Confirms all tests pass, acceptance criteria met
- **Product Manager**: Validates feature meets business requirements
- **Technical Lead**: Signs off on code quality and architectural alignment
- **Stakeholder/Sponsor**: Approves feature for release (if required)
- **Outcome**: Feature approved for release

### Release & Communication
**Involved Roles**: Project Manager, Stakeholder/Sponsor, Developers, QA/Testing Engineer

- **Project Manager**: Coordinates release schedule and communications
- **Developers**: Deploy changes, monitor for issues
- **QA/Testing Engineer**: Runs smoke tests, validates post-deployment
- **Stakeholder/Sponsor**: Announces release to end-users and leadership
- **Outcome**: Feature live in production with stakeholder awareness

### Retrospectives & Continuous Improvement
**Involved Roles**: Scrum Master, All Team Members

- **Scrum Master**: Facilitates blameless retrospective, captures action items
- **All Roles**: Participate in reflection, identify process improvements
- **Outcome**: Prioritized improvements added to backlog for next sprint

---

## Role Interaction Matrix

| Initiator | Collaborator | Key Touchpoint | Frequency |
|-----------|--------------|----------------|-----------|
| Product Manager | Stakeholder/Sponsor | Prioritization & roadmap alignment | Weekly |
| Product Manager | Developers | Acceptance criteria & estimation | Sprint planning |
| Technical Lead | Developers | Code reviews & architecture guidance | Continuous |
| Technical Lead | UX/Design | Technical feasibility of design | Design phase |
| QA/Testing Engineer | Developers | Test strategy & bug triage | Daily/Sprint |
| Scrum Master | All Roles | Process facilitation & impediments | Daily/Sprint |
| Project Manager | All Roles | Schedule, risk, status reporting | Weekly |
| Stakeholder/Sponsor | Product Manager | Business alignment & approvals | Monthly or gate-based |

---

## Communication Patterns by Phase

### Daily
- **Standup**: All team members report progress, blockers, and upcoming work (15 min)
- **Participants**: Developers, QA/Testing, Technical Lead, Scrum Master, (optional) Product Manager

### Sprint
- **Planning** (1-2 hours): Define sprint scope, estimate work, align on acceptance criteria
  - Participants: All roles
- **Mid-sprint Check-in** (optional, 30 min): Review blockers, adjust capacity
  - Participants: Core team + relevant stakeholders
- **Review** (1 hour): Demo completed work, gather feedback
  - Participants: All roles + invited stakeholders
- **Retrospective** (45-75 min): Reflect on process, capture improvements
  - Participants: Core delivery team

### Weekly
- **PM Sync** (1 hour): Product Manager, Project Manager, Technical Lead
  - Discuss roadmap, risks, dependencies, resource needs
- **Stakeholder Update**: Project Manager or Product Manager
  - Brief status, key decisions, risks, asks

### Monthly
- **Stakeholder Briefing** (1-2 hours): All leadership stakeholders
  - Program status, metrics, upcoming priorities, asks

---

## Escalation Paths

### Level 1: Team Triage
**Who**: Developers, QA/Testing, Scrum Master  
**When**: Blocker identified during standup  
**Action**: Scrum Master and Technical Lead work to unblock within 24-48 hours

**Example**: Test infrastructure down, QA blocked
- Scrum Master escalates to Technical Lead
- Technical Lead coordinates fix with DevOps (external)

### Level 2: PM Escalation
**Who**: Project Manager, Product Manager, Technical Lead  
**When**: L1 escalation unresolved or cross-team dependency  
**Action**: PM escalates to Product Lead and dependent teams; may involve Stakeholder/Sponsor

**Example**: Design change required mid-sprint affecting timeline
- Product Manager and Design discuss trade-offs with Stakeholder/Sponsor
- Project Manager updates release timeline if needed

### Level 3: Sponsor Escalation
**Who**: Stakeholder/Sponsor, Project Manager  
**When**: L2 escalation involving business impact, scope, or timeline  
**Action**: Sponsor resolves conflicts, allocates resources, makes go/no-go decisions

**Example**: Resource conflict prevents team from delivering on schedule
- Project Manager escalates to Sponsor for resource reallocation or timeline adjustment

---

## Cross-Functional Dependency Checklist

Use this checklist when planning work that spans multiple roles:

- [ ] **Design**: UX/Design has created and shared designs; Developers and Technical Lead have reviewed
- [ ] **Technical**: Technical Lead has approved architecture; Developers have estimated
- [ ] **Acceptance Criteria**: Product Manager and QA/Testing Engineer have defined clear, testable criteria
- [ ] **Test Plan**: QA/Testing Engineer has outlined test strategy before development starts
- [ ] **Capacity**: Scrum Master has confirmed team capacity for estimated work
- [ ] **Dependencies**: Project Manager has identified external dependencies and mitigations
- [ ] **Stakeholder Alignment**: Stakeholder/Sponsor (if required) has approved scope and timeline

---

## Improving Collaboration: Quick Wins

1. **Establish DRI (Directly Responsible Individual)** for each work item — clarifies ownership and reduces ambiguity
2. **Use Acceptance Criteria Template**: Product Manager + QA/Testing Engineer co-create testable criteria before dev starts
3. **Design Review Gates**: Technical Lead and Developers review UX designs before development to catch feasibility issues early
4. **Risk Register**: Project Manager maintains shared risk register; review in PM Sync weekly
5. **Retrospective Action Items**: Track improvements as backlog items with owners and due dates
6. **RACI Matrix**: For complex projects, create a RACI (Responsible, Accountable, Consulted, Informed) matrix for key phases
