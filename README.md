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
| **Ghulam Qadir Mallah - Owner, Founder, and Enterprise Architect** | Final authority for product, technology, architecture, and live changes. Agree launch scope, budget, architecture, and release decisions. |
| **Ghulam Shabir Mallah - Visionary Architect** | Define the long-term alumni mission, university relationships, chapter model, and community value. |
| **Sarmad Qadir Mallah - Head of Infrastructure and Cloud Technologies** | Propose hosting, domain/email configuration, environments, access management, backups, monitoring, recovery, and operating costs. |
| **Abdul Rehman Mallah - Head of AI and Automation, AI Architect** | Set AI and automation architecture, engineering direction, quality standards, and evaluation. Begin with practical administrative automation. |
| **Mia Brooks - Product and Solution Architect** | Own member journeys, requirements, URL conventions, SEO/analytics architecture, measurement, priorities, and review strategy. |
| **Lily Carter - Lead Developer** | Inventory existing implementation and document gaps. After direction is agreed, prepare changes in separate branches and pull requests. |
| **Sophie Reed - Senior Code Reviewer / Software Engineer** | Independently review implementation, permissions, technical SEO, schema, canonical and robots behaviour, analytics safety, and performance. **Reviewer-only.** |
| **Hannah Jones - QA, SEO and Security Test Lead** | Independently validate signed-out, member, administrator, and mobile behaviour; test privacy, verification, events, accessibility, and Search Console/Analytics evidence. Validate purchase uniqueness if payments are introduced. |

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
