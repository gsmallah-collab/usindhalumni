# University of Sindh Alumni

Working repository for the University of Sindh Alumni digital platform and approved alumni services.

This repository is the project source and governance record. Production changes are not authorised by a GitHub commit alone.

## Start here

- `CLAUDE.md` contains the project working rules and team responsibilities.
- `AGENTS.md` contains the independent Codex review rules.
- `CHANGELOG.md` records meaningful project changes.

## Team

| Team member | Responsibility and first deliverable |
|---|---|
| **Ghulam Qadir Mallah - Owner, Founder, and Enterprise Architect** | Set the overall direction for the University of Sindh Alumni platform and retain final authority for product, technology, architecture, budget, launch scope, and live changes. **First deliverable:** approve the project charter, first-release scope, budget envelope, governance model, and architecture direction. |
| **Ghulam Shabir Mallah - Visionary Architect** | Define the long-term alumni vision, relationship with the University of Sindh, alumni chapter model, community value, engagement priorities, and future growth direction. **First deliverable:** produce the alumni vision and stakeholder map covering university contacts, alumni groups, chapters, and priority community outcomes. |
| **Sarmad Qadir Mallah - Head of Infrastructure and Cloud Technologies** | Own the infrastructure and cloud direction for the alumni platform, including hosting, domains and email, environments, access management, backups, monitoring, recovery, resilience, and operating costs. **First deliverable:** propose the hosting and environment plan with access controls, backup and recovery approach, monitoring, expected running costs, and launch-readiness requirements. |
| **Abdul Rehman Mallah - Head of AI and Automation, AI Architect** | Own AI and automation architecture for the alumni platform, including administrative automation, safe use of alumni data, model selection, evaluation, quality standards, and future AI-assisted services. **First deliverable:** identify the first practical alumni administration automations and produce the AI architecture and evaluation rules, including privacy and human-approval boundaries. |
| **Mia Brooks - Product and Solution Architect** | Own alumni member journeys, product requirements, permission model, information architecture, URL conventions, SEO and analytics architecture, measurement, priorities, and review strategy. **First deliverable:** produce the v1 Product Definition Pack covering registration and alumni verification, member roles and permissions, profiles, directory, connections, events, administration, URL structure, SEO and analytics measurement. |
| **Lily Carter - Lead Developer** | Own implementation and integrations after the direction is approved. Review the existing University of Sindh Alumni website, repository, and supporting systems before changing them. **First deliverable:** produce a technical gap report showing what already exists, what can be retained, what needs improvement or rebuilding, and any technical risks, dependencies, or migration considerations. |
| **Sophie Reed - Senior Code Reviewer / Software Engineer** | Independently review the alumni implementation, authentication and permissions, privacy boundaries, technical SEO, schema, canonical and robots behaviour, analytics safety, security, and performance. **Reviewer-only. First deliverable:** review the existing implementation at an exact SHA and produce a baseline findings report, then review each meaningful implementation SHA before it proceeds to independent QA. |
| **Hannah Jones - QA, SEO and Security Test Lead** | Independently validate the alumni platform for signed-out visitors, applicants, verified alumni members, administrators, and mobile users. Test verification, privacy, profiles, directory permissions, connections, events, accessibility, security, SEO, Search Console, and Analytics evidence. **First deliverable:** create the independent acceptance-test matrix and baseline QA report. If membership fees, donations, or paid events are introduced later, add payment-integrity and duplicate-transaction testing. |

## Delivery stages

| Stage | Concrete result |
|---|---|
| **Discovery** | Existing-system inventory; university verification contact; membership rules; interviews with alumni and event organisers |
| **Product definition** | Agreed first-release requirements, clickable member journeys, permission model, architecture options, and cost estimate |
| **Implementation** | Registration, verification, profiles, directory, connection requests, events, and administration |
| **Independent review** | Sophie's review and Hannah's test evidence, with release-blocking issues resolved |
| **Pilot** | A limited group from several departments and graduation years completes real registrations, connections, and an event |
| **Public launch** | Ghulam Qadir approves release against the evidence, with support and recovery procedures ready |

## How we work

1. Agree the requirement and acceptance criteria before implementation.
2. Work on a branch.
3. Lily implements and tests.
4. Sophie reviews the exact commit SHA.
5. Hannah performs independent QA, security, SEO and device testing where relevant.
6. Mia checks requirements and architecture where required.
7. Ghulam Qadir gives final approval and decides whether anything is merged or released.

A review marked clear does not authorise a merge or production release.

## Security and privacy

Alumni information is personal data.

Do not commit:
- passwords, API keys, tokens or cookies;
- production credentials or database dumps;
- private alumni records;
- identity documents;
- private email or phone lists;
- payment details;
- confidential University material that has not been approved for this repository.

Use synthetic or sanitised data for development and testing.

## Repository rules

- `main` should remain clean and releasable.
- Meaningful work should use a branch and pull request.
- Every review handover must name the exact commit SHA.
- No merge to `main` without Ghulam Qadir's approval.
- No production deployment without Ghulam Qadir's approval.
- Keep rollback instructions for meaningful releases.
- Use plain British English.
- Use normal ASCII punctuation. Do not use em dash or en dash characters.
