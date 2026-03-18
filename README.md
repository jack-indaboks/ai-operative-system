# AI Operative System Documentation

The AI Operative ecosystem is a framework for building reusable AI identities, governance layers, and platform integrations as repository-owned components rather than one-off prompt fragments. Its central idea is simple: layers define Operatives, and an Operative can be composed from one or more layers without turning those layers into disposable runtime state.

This repository is the documentation for that system. It explains what the ecosystem is, where it is headed, and how the current rebuild is organized.

## What the Ecosystem Is

At a high level, the ecosystem separates three kinds of concerns:

1. Identity & Governance
   Personal and team identity layers define voice, values, context, and enduring working style.
2. Self-Maintenance
   Autonomy layers define whether and how an Operative is allowed to modify its own operative files.
3. Environment Integration
   Environment layers define how an Operative is embodied in a specific platform such as GitHub Copilot.

Those concerns are being formalized into a layered template system so Operatives can be composed deliberately, maintained in version control, and deployed across multiple runtimes without collapsing everything into one giant prompt.

## Current State

The ecosystem is in an active structural rebuild. The public documentation set is in place, the high-level architecture is defined, and the next major work is focused on building the shared template and environment lines that will make the system practical to use and maintain.

The active public repository surfaces in ecosystem scope are:

1. Documentation
   `ai-operative-system`
2. Layer Templates
   `ALT`
   `TILT`
   `PILT`
   `CELT`
3. Abstract Templates (not for direct use)
   `ILT`
   `ELT` (planned)

In current terms, this means the ecosystem already has a durable public architecture and roadmap, but the implementation work to realize that architecture is still underway.

## Documents

- `README.md`: current state and navigation surface
- `ARCHITECTURE.md`: the end-state model for the ecosystem, its layers, and their relationships
- `ROADMAP.md`: the live public milestone map for the rebuild
- `CHANGELOG.md`: major completed documentation and architecture changes
- `DOCS.md`: maintainer-facing rules for how this public docs set is managed
