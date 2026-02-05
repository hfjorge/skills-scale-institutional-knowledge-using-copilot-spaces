# OctoAcme — Project Management Overview

This document provides a concise overview of OctoAcme's project management processes and workflows used to plan, coordinate, and deliver work across engineering, product, and documentation teams. It is intended to live in the repository docs folder so it remains versioned with the code and accessible to contributors.

## Principles
- Focus on outcomes and measurable impact.
- Keep work small and incremental — prefer many small PRs over large monoliths.
- Make decisions and rationale explicit (decision records and meeting notes).
- Capture institutional knowledge in documentation and Copilot Spaces for discoverability.

## Intake & Triage
- New work starts as issues. Use templates to capture context, goals, and acceptance criteria.
- Triage regularly (at least weekly): confirm scope, add labels, assign priority, and estimate effort.
- Use labels consistently: e.g., `type:bug`, `type:enhancement`, `priority:high`, `status:triage`.

## Backlog & Planning
- Maintain a prioritized backlog and map work into short milestones (2–4 week cycles).
- For larger initiatives, create an Epic issue that links child issues and tracks progress via milestones.
- Backlog refinement sessions are held each sprint to break down and clarify upcoming work.

## Branching & PR Workflow
- Branch naming: `feature/<brief-desc>`, `fix/<issue-number>-<short-desc>`, or `docs/<desc>`.
- Every PR must link to an issue (e.g., `Closes #NN`) and include a short description of changes and testing steps.
- Use small, focused PRs. Include automated tests and documentation updates where applicable.
- Required reviewers and code owners must be assigned. Use labels like `needs-review` to indicate readiness.

## Reviews & Approvals
- Define reviewers via CODEOWNERS where possible. For other PRs, request at least one reviewer with domain knowledge.
- Review checklist (suggested):
  - Does the change match the issue description and acceptance criteria?
  - Are tests added/updated and passing?
  - Is the code styled and linted?
  - Is documentation updated when behavior or API changes?
- Use GitHub review comments and address feedback via commits in the same branch.

## Continuous Integration & Merging
- PRs must pass CI (lint, tests) before merging.
- Prefer merge strategies that preserve history and clarity (e.g., squash merges for small fixes, merge commits for larger features if needed).
- When merging, include a clear merge commit message or use the PR title to summarize the change.

## Releases & Rollout
- Use milestones to group PRs for a release.
- Tag releases in Git and publish release notes summarizing user-facing changes and any migration steps.
- Coordinate rollouts for infra or breaking changes with stakeholders.

## Documentation & Institutional Knowledge
- Author canonical docs under `docs/` (this file is an example).
- Use Copilot Spaces (or a chosen knowledge platform) to store onboarding guides, decision logs, architecture diagrams and runbooks.
- Keep an index of living documents and link them from the repo README.

## Meetings & Cadence
- Weekly planning/triage and bi-weekly demos/retrospectives are recommended.
- Keep meeting notes and decisions in a searchable place (linked from issues or Copilot Spaces).

## Onboarding & Contribution
- Provide a CONTRIBUTING.md and a short onboarding checklist for new contributors: environment setup, required accounts, code style, running tests, and communication channels.
- Encourage early reviews and pair programming for complex changes.

## Metrics & Reporting
- Track lead time, PR review time, and deployment frequency as core delivery metrics.
- Use lightweight dashboards or milestone progress to inform stakeholders of status.

## Decision Records
- Use short decision records (ADR or DR) to capture significant architecture or process decisions and their rationale.

If you want this changed or expanded (e.g., we can add templates, labels, and example checklists), tell me what to adjust and I will update the file.
