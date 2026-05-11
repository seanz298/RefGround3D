# RefGround3D Architecture

Internet-grounded multi-reference 3D design framework.

---

# Core Philosophy

Traditional Text-to-3D systems:

Text → 3D

RefGround3D:

Text
→ Internet References
→ Reference Understanding
→ Multi-reference Fusion
→ 3D Generation
→ CAD-aware Future Pipeline

The goal is not only generation,
but design understanding.

---

# Overall Pipeline

```text
User Prompt
    ↓
Intent Parsing
    ↓
Query Expansion
    ↓
Internet Image Retrieval
    ↓
CLIP/SigLIP Ranking
    ↓
Reference Pool Construction
    ↓
Reference Decomposition
    ↓
Multi-reference Fusion
    ↓
Image / Multi-view Generation
    ↓
3D Reconstruction
    ↓
Mesh Postprocess
    ↓
CAD-aware Future Pipeline

System Layers
Layer 1 — Design Intent Understanding

Purpose:

Understand what the user actually wants.

Input:

Natural language prompt.

Example:

"A futuristic quadruped robot with exposed metallic skeleton."

Output:

Structured semantic representation.

Example:

{
  "structure": [
    "quadruped",
    "mechanical skeleton"
  ],
  "style": [
    "futuristic",
    "industrial"
  ],
  "materials": [
    "metal"
  ]
}

Key idea:

Design understanding instead of blind generation.

Layer 2 — Internet-grounded Reference Retrieval

Purpose:

Ground generation in real-world visual references.

Instead of generating directly from prompts,
the system retrieves:

product designs
industrial concepts
mechanical structures
material references

Planned retrieval sources:

Google Images
Bing Images
Pinterest
ArtStation
GrabCAD
Layer 3 — Reference Understanding

Purpose:

Understand what each reference contributes.

References are decomposed into:

appearance references
structure references
mechanism references
material references
style references

Planned models:

CLIP
SigLIP
GroundingDINO
SAM
Layer 4 — Multi-reference Fusion

Core idea:

Semantic-level fusion.

Instead of:

single-image conditioning

Use:

Structure A

Appearance B
Material C
Style D

Potential future directions:

scene graphs
part-aware latent fusion
structural relationship graphs
Layer 5 — 3D Generation

Purpose:

Generate controllable conceptual 3D assets.

Planned backends:

TripoSR
InstantMesh
Hunyuan3D

Current output formats:

GLB
OBJ
STL

Future directions:

structured generation
parametric generation
CAD-aware generation
Layer 6 — Engineering Semantics (Future)

Long-term vision:

The system should understand:

structural validity
manufacturability
motion relationships
engineering constraints

Future goals:

AI Design Understanding
→ Engineering-aware AI
→ AI-CAD Co-design

Long-term Direction

RefGround3D is not intended to become another generic Text-to-3D generator.

The long-term goal is:

AI Design Copilot
for engineering-aware conceptual design.
