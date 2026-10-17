# Working rules for this repository

This file holds the working rules for the University of Sindh Alumni project.

## The project

This repository supports the University of Sindh Alumni digital platform and approved alumni services.

The platform should be simple, trustworthy, accessible, secure and maintainable.

Do not assume that a feature, claim, University statement, policy, alumni record or official status exists unless it has been supplied or approved.

## Team and authority

Use these names, titles and responsibilities consistently in project documents.

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

Ghulam Qadir Mallah has final authority for product, technology, architecture and live changes.

A technical review, QA pass or architecture recommendation does not itself authorise a merge, release or production change.

## Delivery stages

The project moves through these evidence-based stages. Do not skip a stage simply because implementation is technically possible.

| Stage | Concrete result |
|---|---|
| **Discovery** | Existing-system inventory; university verification contact; membership rules; interviews with alumni and event organisers |
| **Product definition** | Agreed first-release requirements, clickable member journeys, permission model, architecture options, and cost estimate |
| **Implementation** | Registration, verification, profiles, directory, connection requests, events, and administration |
| **Independent review** | Sophie's review and Hannah's test evidence, with release-blocking issues resolved |
| **Pilot** | A limited group from several departments and graduation years completes real registrations, connections, and an event |
| **Public launch** | Ghulam Qadir approves release against the evidence, with support and recovery procedures ready |

## How we work

1. Agree the direction first, then build.
2. Record acceptance criteria before implementation.
3. Where UI is involved, show the owner a design or working sample before finalising it.
4. Work on a branch named for the task, for example `work/2026-10-17-alumni-registration`.
5. Keep unrelated changes out of the branch.
6. Commit finished pieces with messages that say what changed and why.
7. Open a pull request with a plain description of the requirement, implementation, tests, limitations and rollback.
8. Lily builds and tests.
9. Sophie reviews the exact code SHA.
10. Hannah tests independently after code review when the change requires runtime, security, SEO, accessibility, mobile or browser evidence.
11. Mia checks requirement and architecture coverage where required.
12. Ghulam Qadir gives final approval.
13. Only Ghulam Qadir decides whether the work is merged or released, unless he explicitly delegates that authority.

## Handover to Sophie

Every meaningful handover must include:
- exact commit SHA;
- requirement or issue reference;
- what changed;
- why it changed;
- files changed;
- tests run and results;
- known limitations;
- security and privacy impact;
- rollback.

One meaningful code SHA should receive one review request. Do not spend review capacity on documentation-only or comment-only changes unless there is a specific reason.

## Independent QA

Hannah should test from the agreed acceptance criteria rather than from Lily's implementation notes alone.

Where relevant, QA should cover:
- desktop and mobile;
- supported browsers;
- keyboard navigation;
- screen-reader announcements;
- form validation;
- authentication and logout;
- recovery flows;
- duplicate submission;
- refresh, back and reopen;
- permissions and role boundaries;
- SEO and indexability;
- security regression;
- performance evidence.

## Security and privacy

Alumni data is personal data and must be treated accordingly.

Never commit:
- passwords;
- API keys;
- tokens;
- session cookies;
- recovery codes;
- production environment files;
- private database exports;
- identity documents;
- private alumni lists;
- personal email addresses or phone numbers used as test data;
- payment card data;
- confidential University material that has not been approved for repository storage.

Use synthetic or sanitised data for development and tests.

Do not log sensitive form values.

Administrative actions must use server-side authorisation. Hiding a button is not access control.

Apply least privilege to roles and integrations.

For any feature that stores alumni data, define:
- purpose;
- data fields;
- who can read it;
- who can change it;
- retention;
- deletion or correction behaviour;
- export needs;
- audit needs.

Do not silently expand data collection.

## Authentication and accounts

Account, profile and administrative journeys must have clear ownership and state.

Avoid:
- duplicate accounts for the same verified identity;
- ambiguous login states;
- exposing whether an unrelated person's account exists where that creates privacy risk;
- insecure password reset;
- client-side-only permission checks;
- predictable object identifiers used without authorisation.

Any future alumni verification process must distinguish between:
- a person creating an account;
- a person claiming alumni status;
- evidence or approval of that status;
- permissions granted after verification.

Do not treat account creation alone as proof of alumni status.

## Public content

Do not invent:
- University facts;
- alumni numbers;
- degrees;
- departments;
- rankings;
- partnerships;
- events;
- official endorsements;
- contact details;
- policies.

Use approved source material.

Public wording should be professional, concise and in British English.

## Accessibility and UX

Design mobile-first.

Keep forms short and clear.

Use:
- proper labels;
- useful error text;
- visible keyboard focus;
- accessible status announcements;
- adequate touch targets;
- semantic headings;
- sufficient contrast.

Avoid duplicate calls to action and contradictory states.

## SEO

Public pages should use:
- one clear page purpose;
- useful title and meta description;
- canonical URL;
- correct headings;
- crawlable content;
- optimised images;
- structured data only when the facts are supported.

Private account, profile management, admin, staging and internal utility pages should not be indexed.

## Performance

Avoid:
- unnecessary scripts;
- duplicate API calls;
- repeated database queries;
- heavy third-party code on every page;
- blocking work that can be deferred.

Measure before making major infrastructure changes.

## AI and automation

AI may assist with:
- search;
- drafting;
- classification;
- support;
- recommendations;
- summarisation;
- administration.

AI must not silently:
- verify alumni status;
- alter official University records;
- approve privileged access;
- make legal or policy decisions;
- publish unsupported facts;
- expose private alumni data.

Human-controlled actions must remain auditable.

## Repository rules

- `main` should remain clean and complete.
- Work happens on a branch and reaches `main` through a pull request.
- Ghulam Qadir gives final merge approval.
- No production change is implied by a merge.
- Keep a dated `CHANGELOG.md` entry for meaningful pull requests or releases.
- Do not store secrets or personal data in Git.
- Keep project-specific data and systems separate from NokarOnline and other Sayah Consulting projects unless an integration is deliberately approved.
- Record rollback for meaningful releases.

## Writing rule

Use plain British English.

Use normal ASCII punctuation. Do not use em dash or en dash characters.

The owner's informal wording expresses intent. Convert it into professional product or technical language before placing it in public copy, project documents or code comments.
