# AI Operative System Documentation

The AI Operative ecosystem is a framework for building reusable AI identities, procedural layers, and platform integrations as repository-owned components rather than one-off prompt fragments. Its central idea is simple: an Operative begins as an instance of the shared kernel, grows through selected layers, and remains grounded in durable source repositories rather than disposable runtime state.

This repository is the documentation for that system. It explains what the ecosystem is, where it is headed, and how the current rebuild is organized.

## What the Ecosystem Is

At a high level, the ecosystem separates three kinds of concerns:

1. Operative Baseline & Assembly
   The kernel defines the universal operative baseline, and assembly workflows extend that baseline with selected upstream layers into one durable Operative repo.
2. Identity & Procedure
   Identity layers define voice, values, context, and enduring working style, while operations layers provide reusable procedures that are not inseparable from identity.
3. Environment Integration
   Environment layers define how an Operative is embodied in a specific platform such as GitHub Copilot.

Those concerns are being formalized into a layered template system so Operatives can be composed deliberately, maintained in version control, and deployed across multiple runtimes without collapsing everything into one giant prompt.

## Current State

The ecosystem is in an active structural rebuild. The public documentation set is in place, the high-level architecture is defined, and the next major work is focused on building the shared kernel, template, and environment lines that make that architecture practical to use and maintain.

In current terms, this means the ecosystem already has a durable public architecture centered on the Operative Kernel, assembled Operative repos, and preserved upstream layer sources, while the implementation work to realize `OK`, `OLT`, `ILT`, `CELT`, `TILT`, and `PILT` is still underway.

## Documents

- `README.md`: current state and navigation surface
- `ARCHITECTURE.md`: the end-state model for the ecosystem, its layers, and their relationships
- `ROADMAP.md`: the live public milestone map for the rebuild
- `CHANGELOG.md`: major completed documentation and architecture changes
- `DOCS.md`: maintainer-facing rules for how this public docs set is managed
