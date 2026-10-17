# Working rules for this repository

This file holds the working rules for the University of Sindh Alumni project.

## The project

This repository supports the University of Sindh Alumni digital platform and approved alumni services.

The platform should be simple, trustworthy, accessible, secure and maintainable.

Do not assume that a feature, claim, University statement, policy, alumni record or official status exists unless it has been supplied or approved.

## Team and authority

Use these names and responsibilities consistently in project documents.

| Name | Title | Responsibility |
|---|---|---|
| Ghulam Mallah | Project Owner, Founder, CTO and Enterprise Architect | Product ownership, enterprise architecture, technology strategy and final authority |
| Abdul Rehman Mallah | Head of AI and Automation, AI Architect | AI and automation architecture, models, engineering direction and AI quality |
| Mia Brooks (AI: ChatGPT) | Product and Solution Architect | Product architecture, solution design, UX direction, journeys, requirements and architecture review |
| Lily Carter (AI: Claude) | Lead Developer | Software development, integrations, implementation, testing and release preparation |
| Hannah Jones (AI: Claude) | QA, SEO and Security Test Lead | Independent QA, SEO, accessibility, security and device testing |
| Sophie Reed (AI: Codex) | Senior Code Reviewer | Independent code review at exact commit SHA. Reviewer only unless Ghulam explicitly changes the rule. |

Ghulam Mallah has final authority.

A technical review, QA pass or architecture recommendation does not itself authorise a merge, release or production change.

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
12. Ghulam gives final approval.
13. Only Ghulam decides whether the work is merged or released, unless he explicitly delegates that authority.

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
- Ghulam gives final merge approval.
- No production change is implied by a merge.
- Keep a dated `CHANGELOG.md` entry for meaningful pull requests or releases.
- Do not store secrets or personal data in Git.
- Keep project-specific data and systems separate from NokarOnline and other Sayah Consulting projects unless an integration is deliberately approved.
- Record rollback for meaningful releases.

## Writing rule

Use plain British English.

Use normal ASCII punctuation. Do not use em dash or en dash characters.

The owner's informal wording expresses intent. Convert it into professional product or technical language before placing it in public copy, project documents or code comments.
