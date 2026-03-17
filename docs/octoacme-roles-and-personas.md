# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
The Release Manager coordinates release schedules, owns the end-to-end release process, and ensures that deployments are safe, well-communicated, and repeatable. They serve as the accountable owner for every production deployment.

### Responsibilities
- Plan and manage release timelines and deployment windows
- Own the release readiness checklist and gate criteria
- Coordinate cross-functional sign-off (Engineering, QA, Security, Support)
- Communicate release status and blockers to stakeholders
- Maintain rollback and incident response plans for each release
- Track and close post-release action items

### Goals
- Ship releases predictably with minimal surprises
- Reduce deployment risk through repeatable checklists and runbooks
- Make release status transparent to all stakeholders

### Typical Communication
- Pre-release readiness meetings with Engineering, QA, and Security Lead
- Release announcements and post-deploy notifications to stakeholders
- Incident updates when a deployment causes issues

### Interactions / Handoffs
- **Project Manager**: Aligns on release scope, timeline, and dependencies; escalates blockers that affect schedule.
- **Product Manager**: Confirms feature completeness and communicates release notes to customers.
- **Developers**: Reviews deployment readiness (merged PRs, passing CI, smoke tests) and confirms rollback steps.
- **Security Lead**: Ensures security scans are green and any outstanding issues are accepted or mitigated before release.
- **Customer Success Lead**: Provides advance notice of upcoming changes; coordinates customer-facing communications.

See [Release Readiness Checklist](templates/octoacme-release-readiness-checklist.md) and the [Release & Deployment Guide](octoacme-release-and-deployment.md) for key artifacts.

---

## Technical Writer (Docs Owner)

### Role Summary
The Technical Writer maintains technical and process documentation, ensuring information is accurate, accessible, and consistent across all project phases. They translate complex requirements and workflows into clear, shareable artifacts.

### Responsibilities
- Draft, review, and update internal and external documentation
- Ensure docs follow established structure and tone standards
- Collaborate with developers and PMs to capture process changes
- Maintain the docs directory and flag outdated or missing content
- Support onboarding by keeping guides current and complete

### Goals
- Make project knowledge accessible to new and existing team members
- Reduce repeated questions by improving self-serve documentation
- Keep documentation synchronized with process and product changes

### Typical Communication
- Async reviews of PRs that include doc changes
- Periodic documentation review meetings with PM and Product Manager
- Requests to developers and leads for technical clarifications

### Interactions / Handoffs
- **Project Manager**: Receives notifications of process changes requiring doc updates; contributes to retrospective notes.
- **Product Manager**: Captures feature specs and release notes; ensures external docs reflect shipped functionality.
- **Developers**: Reviews and improves technical documentation (READMEs, API docs, runbooks); coordinates on accuracy.
- **Release Manager**: Drafts and reviews release notes; ensures the release readiness checklist and deployment guides are current.

---

## Security Lead

### Role Summary
The Security Lead manages risk assessments, security reviews, and incident response for project deliverables. They ensure that security considerations are incorporated throughout the project lifecycle—not just at release time.

### Responsibilities
- Perform security reviews and provide mitigation guidance for new features
- Maintain and update the security incident runbook
- Review CI security scan results and own remediation tracking
- Coordinate security incident communication and response
- Participate in risk register reviews to flag security-related risks

### Goals
- Reduce security vulnerabilities introduced into production
- Ensure the team follows security best practices throughout delivery
- Provide clear escalation paths for security incidents

### Typical Communication
- Security review notes on PRs and design docs
- Incident alerts and post-incident reports
- Risk register updates for security-related items

### Interactions / Handoffs
- **Project Manager**: Reports security risks and status; escalates incidents that may affect schedule or scope.
- **Developers**: Provides guidance on remediation for vulnerabilities found in code or dependencies; approves security-related PRs.
- **Release Manager**: Confirms security scans pass and any accepted risks are documented before production deployments.
- **Stakeholder Representative**: Communicates security posture and incident status when business or customer impact is possible.

See the [Risk Register Template](templates/octoacme-risk-register-template.md) and the [Risk Management & Communication Guide](octoacme-risks-and-communication.md) for escalation paths.

---

## Stakeholder Representative

### Role Summary
The Stakeholder Representative serves as the voice of key business stakeholders (customers, partners, or internal business units). They bring requirements and feedback into the project and validate that deliverables meet stakeholder goals.

### Responsibilities
- Gather and communicate stakeholder needs, priorities, and concerns
- Review deliverables and provide structured feedback
- Escalate high-priority issues that require executive attention
- Validate that acceptance criteria align with stakeholder expectations
- Participate in demos and release reviews

### Goals
- Ensure the project delivers measurable business value
- Prevent surprises by keeping stakeholders informed and involved
- Represent stakeholder perspective in trade-off decisions

### Typical Communication
- Milestone review meetings with PM and Product Manager
- Structured feedback on demos and release candidates
- Escalation emails or incident updates when issues affect customers

### Interactions / Handoffs
- **Product Manager**: Partners on roadmap prioritization and acceptance criteria; ensures stakeholder priorities are reflected in the backlog.
- **Project Manager**: Receives regular status updates; raises escalations when delivery risks affect stakeholder commitments.
- **Customer Success Lead**: Coordinates to align on customer feedback and adoption tracking.
- **Security Lead**: Informed of security incidents that may have business or customer impact.

---

## Customer Success Lead

### Role Summary
The Customer Success Lead tracks adoption of released features, manages customer onboarding, and bridges the gap between product delivery and the customer experience. They ensure customers get value from released work.

### Responsibilities
- Monitor feature rollout, adoption metrics, and customer satisfaction signals
- Support customer onboarding and provide training resources
- Collect and relay customer feedback to Product Manager and PM
- Coordinate customer-facing communications for major releases or incidents
- Escalate critical customer issues to the appropriate team

### Goals
- Drive adoption and satisfaction for released features
- Reduce customer friction through proactive support and communication
- Translate customer feedback into actionable product improvements

### Typical Communication
- Regular sync with Product Manager and Stakeholder Representative
- Customer onboarding guides and release communications
- Incident or degradation notices to affected customers

### Interactions / Handoffs
- **Product Manager**: Provides customer adoption data and feedback to inform roadmap priorities; participates in feature reviews.
- **Project Manager**: Flags customer-impacting risks and coordinates communication timing around releases.
- **Release Manager**: Receives advance release notifications to prepare customer-facing communications and support materials.
- **Stakeholder Representative**: Aligns on stakeholder expectations and communicates adoption results.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

For role ownership across project phases, see [Ownership & RACI Matrix](octoacme-ownership-and-raci.md).

