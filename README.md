# AI Operative System Documentation

This repository is the documentation home for the AI Operative ecosystem. It defines the core architectural principles, shared concepts, and organizational structure that guide the design and development of all operative layers, templates, and instances.

## Current System Shape

The ecosystem currently organizes around these layers of structure:

1. Class Templates
   - `ILT`: What is the essence of an Identity Layer?
   - `ALT`: What governance must be considered when allowing an Operative to modify itself?
   - `ELT`: What must be considered when integrating an Operative into a particular platform?

2. Instance Templates
   - `PILT` / `TILT`: What minimum defaults define a Personal / Team Identity Layer?
   - `CELT`: What does an Operative need to integrate seamlessly into GitHub Copilot?

3. Layer Repositories
   - Personal Identity Layer: Who is this specific personal identity layer and what does it always know?
   - Team Identity Layer: Who is this specific team identity layer and what does it always know?
   - Environment Layer: What platform-specific tooling does this individual or team provide for their Operatives?
   - Autonomy Layer: What boundaries does this individual or team impose around self-editing?

4. Operatives
   - Runtime compositions of layer repositories within a specific platform context and the embodied instance of that composition in a host platform.

## Template Tree

```mermaid
flowchart TD
   subgraph ClassTemplates[Class Templates]
      ILT["<b>Identity Layer Template</b><br>(ILT)<br>Identity-layer essence and inheritance rules"]
      ALT["<b>Autonomy Layer Template</b><br>(ALT)<br>Self-edit governance, authority, safety"]
      ELT["<b>Environment Layer Template</b><br>(ELT)<br>Abstract environment integration model"]
   end

   subgraph InstanceTemplates[Instance Templates]
      PILT["<b>Personal Identity Layer Template</b><br>(PILT)<br>Minimal structure and defaults for a personal identity layer"]
      TILT["<b>Team Identity Layer Template</b><br>(TILT)<br>Minimal structure and defaults for a team identity layer"]
      CELT["<b>Copilot Environment Layer Template</b><br>(CELT)<br>GitHub Copilot integration utilities and minimal defaults"]
   end

   subgraph LayerRepos[Layer Repositories]
      PIL["<b>Personal Identity Layer</b><br>Identity and knowledge for one person's operative"]
      TIL["<b>Team Identity Layer</b><br>Identity and knowledge for a team's operative"]
      ELR["<b>Environment Layer</b><br>Specific platform tooling and integration surfaces"]
      ALR["<b>Autonomy Layer</b><br>Concrete self-edit boundaries"]
   end

   subgraph OperativeLayer[Operative]
      OP["<b>Operative</b><br>Runtime composition of one or more layers"]
   end

   ILT -->|inherits into| PILT
   ILT -->|inherits into| TILT
   ALT -->|instantiates into| ALR
   ELT -->|inherits into| CELT

   PILT -->|instantiates into| PIL
   TILT -->|instantiates into| TIL
   CELT -->|instantiates into| ELR

   PIL -->|may compose into| OP
   TIL -->|may compose into| OP
   ELR -->|may compose into| OP
   ALR -->|may compose into| OP
```

`ALT` currently routes directly into concrete autonomy layers because no useful autonomy instance-template split has been identified yet. `ELT` remains abstract for now, with `CELT` as its first concrete environment-template line.

## Core Architectural Principles

- The repository is the master. Live instances are disposable projections of repo-owned truth.
- Operative layers are portable, repo-sovereign, instance-symmetric identity modules.
- Persistent behavior belongs in git, even when it is platform-specific.
- Generated artifacts are projections of canon, not silent replacements for canon.
