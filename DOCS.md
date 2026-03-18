# AI Operative System Docs Rules

This document defines the roles of the core project documents and the rules for maintaining them.

`ai-operative-system` is the public documentation repository for the AI Operative ecosystem. Everything in this repository is public-facing. Local execution state, private coordination details, and maintainer-only working checklists must remain outside this repository.

## Document Boundaries

- `README.md`: current state and navigation surface for the ecosystem documentation set
- `ARCHITECTURE.md`: final-state planned ecosystem architecture
- `ROADMAP.md`: live public-facing milestone map for ecosystem progression
- `CHANGELOG.md`: append-only record of meaningful completed changes across the ecosystem documentation effort
- `DOCS.md`: maintainer-facing documentation rules and document boundaries

## Update Discipline

- Public-facing project content belongs in the project documents, not in maintainer notes.
- Maintainer guidance about how to update the docs belongs here.
- Final ecosystem architecture belongs in `ARCHITECTURE.md`.
- Public milestone progress belongs in `ROADMAP.md`.
- Completed changes belong in `CHANGELOG.md`.
- Local working context and internal unresolved questions are tracked outside this repository.
- External questions worth public discussion can be surfaced through GitHub issues.
- Template-internal design work that does not yet belong in public ecosystem architecture stays outside this repository until it is ready for publication.

## Roadmap Rules

- `ROADMAP.md` is a live public-facing milestone checklist, not a historical record and not the granular operational checklist.
- Milestone items are checked off in `ROADMAP.md` as they are completed.
- Completed work and roadmap updates are recorded in `CHANGELOG.md`.
- Completed phases do not remain in `ROADMAP.md`.
- When a phase is complete, remove it from `ROADMAP.md` and release if applicable.
- Private repository coordination, local AI governance, and step-by-step execution detail do not belong in `ROADMAP.md`.

## Changelog Rules

- `CHANGELOG.md` is append-only.
- Changelog entries describe public-facing outcomes, not private working detail.
- Backfilled history may be summarized into larger date-grouped bullets when needed.
- Changelog-worthy commits may be logged as one bullet per commit.
- When entries span multiple repositories in the ecosystem, prefix each bullet with the affected repository name.
- `CHANGELOG.md` may record meaningful completed changes in repositories other than `ai-operative-system` when those changes are part of the ecosystem-level documentation history.
- Do not log every commit; only record changes that materially affect architecture, documentation, milestones, or deliverable shape.
