# Changelog

## 2026-02-06

- established the initial structural-rebuild planning pass and interim working checklist model
- reviewed the existing workflow documentation and standardized dated completion tracking

## 2026-02-18

- documented the interim rebuild workflow cadence and inventoried the active template baseline

## 2026-02-23

- defined the initial autonomy-layer scope and the initial boundary between autonomy-layer and workspace task tracking

## 2026-02-26

- began the structured review of the legacy reference corpus to extract reusable ecosystem concepts and discard non-portable material

## 2026-02-27

- reconciled legacy template-idea material into the active planning backlog and retired obsolete staging material
- completed an early pass over the legacy reference corpus, confirming several file families had no reusable delta

## 2026-03-02

- extended the legacy reference review into source-policy material and routed surviving deltas forward

## 2026-03-03

- continued the legacy reference review across persona, philosophy, and memory-related material, keeping only reusable ecosystem concepts

## 2026-03-05

- completed the first user-layer review pass in the legacy reference corpus

## 2026-03-06

- completed the core people, organization, environment, project, and glossary review passes in the legacy corpus
- extracted reusable glossary structure, Copilot instruction-surface lessons, and canon-versus-runtime boundary insights into the ecosystem design work

## 2026-03-09

- finished the broad-scan review of the remaining legacy corpus and narrowed the surviving pilot cross-pollination candidates
- restructured the ecosystem roadmap around deliverable-oriented phases and explicit ownership boundaries

## 2026-03-11

- selected `08_TOOLS_{ILname}.md` as the canonical template slot for tool-use governance

## 2026-03-17

- Split durable architecture content out of `README.md` into `ARCHITECTURE.md`.
- Created initial `ROADMAP.md`, `CHANGELOG.md`, and `DOCS.md` scaffolds for the `_docs` repository.
- Refocused `README.md` on current-state navigation and document roles.
- Migrated the first settled ecosystem architecture from the working roadmap into `ARCHITECTURE.md`.
- Reframed `ROADMAP.md` as a public-facing milestone map for the structural rebuild.
- Aligned the public docs to repo-facing naming and scope.
- Distilled completed pre-documentation history into a public-facing `CHANGELOG.md` backlog.
- Refined `DOCS.md` into a repository-specific documentation specification for the public ecosystem docs set.
- Expanded `README.md` into a fuller ecosystem entry point that explains both the system vision and the current rebuild state.
- Clarified the operative composition model so loaded layers are documented as a single internalized identity rather than as a stack of personas.
- Realigned `ARCHITECTURE.md` and its diagram around abstract templates versus directly usable layer templates, including the current `ALT` positioning. *Commit 44d1263: Documentation Launch*

## 2026-03-26

- Clarified `ARCHITECTURE.md` around protected standalone-layer plumbing, renamed the shared `CORE` spine to `Operative Layer Protocol`, and introduced `OLT` as the directly usable operations-layer template with `ILT`/`OLT`/`CELT` boundaries tightened accordingly.

## 2026-03-27

- Introduced the Operative Kernel as the universal operative baseline and reframed the public architecture around assembled Operative repos built from kernel plus selected upstream layers. *Commit 26b0f92: Kernel*
- Removed `ALT` from the public architecture, introduced target-local `EDITING_<Repo>.md` governance for editable source repos, and realigned the public docs to the kernel-plus-Operative model. *Commit 603e48c: Ready for Implementation*

**0.0.2**

## 2026-04-02

- Clarified `ARCHITECTURE.md` around `PROTOCOL` as the ecosystem-defining protected file, the rest of the kernel file family as required implementation surfaces, and operative files as the canon that defines an Operative. *Commit ce46403: PROTOCOL*
- **operative-kernel**: Reworked `00_PROTOCOL.md` into a compact operative-facing protocol block with a stable assembled-artifact skeleton (`Assembled Identity`, `Operative File Index`). *Commit 383f526: PROTOCOL*

## 2026-04-07

- Reorganized `ARCHITECTURE.md` around the clarified ecosystem architecture, defining the `Templates`/`Layers`/`Operatives` hierarchy, narrowing the kernel to an immutable-by-default baseline, introducing `BOLT` as the maintainer-focused `OLT` line, and clarifying environment layers as host-native embodiment surfaces for platform-agnostic Operatives. *Commit 95feefb: ARCHITECTURE clean-up + BOLT*

## 2026-04-09

- **operative-kernel**: Clarified the kernel protocol and governance baseline so operative-local canon remains maintainable under kernel defaults while included layer repos stay read-only unless a more specific layer-governance source authorizes edits. *Commit a95f64b: assemble vs build*
- Clarified the public architecture around assemble-versus-build terminology, narrowed `BOLT` to upstream layer editing, distinguished live-source versus generated runtime forms, and made explicit that live-source Operatives require a directory-bearing, git-capable environment. *Commit 1f36a99: assemble vs build*
