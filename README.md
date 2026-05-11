# RefGround3D

Internet-grounded multi-reference 3D design framework.

Instead of generating 3D assets directly from text prompts,
RefGround3D first retrieves and understands real-world visual references,
then performs structure-aware multi-reference fusion for controllable 3D generation.

---

# Core Idea

Traditional pipelines:

Text → 3D

RefGround3D:

Text
→ Internet References
→ Reference Understanding
→ Multi-reference Fusion
→ 3D Generation
→ CAD-aware Postprocess

The goal is not only generation,
but design understanding.

---

# Why RefGround3D

Current Text-to-3D systems often suffer from:

- weak structural consistency
- lack of engineering semantics
- hallucinated mechanisms
- poor controllability
- no real-world grounding

RefGround3D introduces:

- internet-grounded visual references
- multi-reference decomposition
- structure-aware fusion
- engineering-oriented design semantics

---

# Key Features

## 1. Natural Language Design Intent Parsing

Understand:

- structure
- functionality
- style
- materials
- engineering constraints

Example:

Input:

"A futuristic quadruped robot with exposed metal skeleton and transparent shell."

Parsed Intent:

- quadruped
- mechanical structure
- industrial futuristic style
- transparent outer shell
- metallic materials

---

## 2. Internet-grounded Reference Retrieval

Automatically search references from:

- Google Images
- Bing Images
- Pinterest
- ArtStation
- GrabCAD

The system builds a real-world reference pool instead of generating blindly.

---

## 3. Reference Understanding

References are decomposed into:

- appearance references
- structure references
- material references
- style references
- mechanism references

Powered by:

- CLIP / SigLIP
- GroundingDINO
- SAM

---

## 4. Multi-reference Fusion

Instead of single-image conditioning:

Structure A
+ Appearance B
+ Material C
+ Style D

The system performs semantic-level design fusion.

---

## 5. 3D Generation

Current planned backends:

- TripoSR
- InstantMesh
- Hunyuan3D

Future directions:

- structured generation
- CAD-aware generation
- engineering-aware synthesis

---

# System Architecture

See:

docs/architecture.md

---

# Roadmap

## V0.1
Natural language → Internet image retrieval

## V0.2
CLIP/SigLIP semantic ranking

## V0.3
Reference categorization

## V0.4
Multi-reference selection interface

## V0.5
Image-to-3D integration

## V0.6
Multi-view reconstruction

## V1.0
Complete web prototype

## V2.0
Structure-aware fusion

## V3.0
CAD-aware AI design

---

# Long-term Vision

RefGround3D is not intended to be another Text-to-3D generator.

The long-term goal is:

AI Design Understanding
→ AI Engineering Semantics
→ AI-CAD Co-design

---

# Project Status

Concept-stage research framework.

Early prototype under development.

---

# Keywords

AI Design
Text-to-3D
Multi-reference Fusion
Internet-grounded Generation
AI-CAD
Design Understanding
Engineering-aware AI

---

# License

MIT License
