# RefGround3D Roadmap

Internet-grounded multi-reference 3D design framework.

---

# Vision

RefGround3D aims to move beyond traditional Text-to-3D pipelines.

Instead of directly generating 3D assets from prompts,
the system first retrieves and understands real-world visual references,
then performs semantic-level multi-reference fusion for controllable 3D generation.

Long-term goal:

AI Design Understanding
→ Structure-aware Synthesis
→ AI-CAD Co-design

---

# Development Stages

---

# Phase 1 — Foundation

## V0.1 — Natural Language Parsing

Goals:

- Parse design intent from prompts
- Extract:
  - structure
  - functionality
  - style
  - materials
  - engineering constraints

Output:

Structured semantic JSON.

---

## V0.2 — Internet-grounded Reference Retrieval

Goals:

- Automatic query expansion
- Internet image retrieval
- Reference caching

Planned sources:

- Google Images
- Bing Images
- Pinterest
- ArtStation
- GrabCAD

---

## V0.3 — Semantic Ranking

Goals:

- CLIP/SigLIP semantic similarity
- Prompt-image ranking
- Reference scoring

---

## V0.4 — Reference Categorization

Goals:

Separate references into:

- appearance
- structure
- materials
- style
- mechanisms

---

# Phase 2 — Interactive Design Pipeline

## V0.5 — Multi-reference Selection UI

Goals:

Users can select:

- appearance reference
- structure reference
- material reference
- style reference

---

## V0.6 — Image-to-3D Integration

Planned backends:

- TripoSR
- InstantMesh
- Hunyuan3D

Goals:

Generate:

- GLB
- OBJ
- STL

---

## V0.7 — Multi-view Generation

Goals:

- improve geometry consistency
- reduce hallucinated structures
- support better mesh reconstruction

---

# Phase 3 — Structure-aware Design

## V1.0 — Semantic Fusion

Goals:

- semantic-level reference fusion
- structure-aware conditioning
- part-aware generation

Instead of:

single latent conditioning

Use:

Structure A
+ Appearance B
+ Material C
+ Style D

---

## V1.5 — Structural Relationship Graphs

Goals:

Represent:

- joints
- supports
- mechanisms
- motion relationships

Future directions:

Scene graphs
+ Part-aware latent fusion

---

# Phase 4 — Engineering-aware AI

## V2.0 — CAD-aware Generation

Goals:

Move beyond mesh generation.

Future outputs:

- parametric structures
- CAD feature trees
- manufacturable geometry

---

## V2.5 — Structural Validation

Goals:

- manufacturability
- motion validation
- structural consistency
- collision checking

---

## V3.0 — AI Design Copilot

Long-term vision:

Prompt
→ Design Understanding
→ Engineering Semantics
→ AI-CAD Co-design

RefGround3D evolves into an AI engineering and design copilot system.

---

# Current Status

Concept-stage research framework.

Early prototype under development.