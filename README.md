# AI Operative System Documentation

The AI Operative ecosystem is a system for building durable AI operatives from reusable sources. Instead of treating prompts, instructions, and environment-specific integration as disposable runtime fragments, it defines them as maintained sources with clear roles and update paths.

An Operative begins from the shared kernel, composes selected identity and operations layers into one coherent operative canon, and can then be embodied in specific host environments. This repository documents that model and tracks the work of building it out.

## What the Ecosystem Is

At a high level, the ecosystem separates three kinds of concerns:

1. Operative Baseline
   The kernel defines the shared baseline and protected contract every Operative begins from.
2. Layer Families
   Identity, operations, and environment layers contribute distinct kinds of canon to the system.
3. Operative Composition And Embodiment
   Operatives compose selected layer canon into one durable system and may then be embodied across specific host environments.

This architecture makes Operatives composable, governable, and maintainable across repositories instead of collapsing everything into one monolithic prompt surface.

## Current State

The public architecture is established. The implementation work now underway is building the shared kernel, template lines, and environment surfaces that realize it as a working ecosystem.

Today, that means the ecosystem has a stable architectural model and an active buildout focused on turning `OK`, `OLT`, `BOLT`, `ILT`, `CELT`, `TILT`, and `PILT` into concrete templates and maintained source repositories.

## Documents

- `README.md`: current state and navigation surface
- `ARCHITECTURE.md`: the end-state model for the ecosystem, its layers, and their relationships
- `ROADMAP.md`: the live public milestone map for the rebuild
- `CHANGELOG.md`: major completed documentation and architecture changes
- `DOCS.md`: maintainer-facing rules for how this public docs set is managed
