# University of Sindh Alumni

Working repository for the University of Sindh Alumni digital platform and approved alumni services.

This repository is the project source and governance record. Production changes are not authorised by a GitHub commit alone.

## Start here

- `CLAUDE.md` contains the project working rules and team responsibilities.
- `AGENTS.md` contains the independent Codex review rules.
- `CHANGELOG.md` records meaningful project changes.

## Team

| Name | Role |
|---|---|
| Ghulam Mallah | Project Owner, Founder, CTO and Enterprise Architect. Final authority. |
| Abdul Rehman Mallah | Head of AI and Automation, AI Architect. |
| Mia Brooks (AI: ChatGPT) | Product and Solution Architect. |
| Lily Carter (AI: Claude) | Lead Developer. |
| Hannah Jones (AI: Claude) | QA, SEO and Security Test Lead. |
| Sophie Reed (AI: Codex) | Senior Code Reviewer. Reviewer only unless Ghulam explicitly changes that rule. |

## How we work

1. Agree the requirement and acceptance criteria before implementation.
2. Work on a branch.
3. Lily implements and tests.
4. Sophie reviews the exact commit SHA.
5. Hannah performs independent QA, security, SEO and device testing where relevant.
6. Mia checks requirements and architecture where required.
7. Ghulam gives final approval and decides whether anything is merged or released.

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
- No merge to `main` without Ghulam's approval.
- No production deployment without Ghulam's approval.
- Keep rollback instructions for meaningful releases.
- Use plain British English.
- Use normal ASCII punctuation. Do not use em dash or en dash characters.
