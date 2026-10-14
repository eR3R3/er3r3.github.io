---
layout: page
title: GeoCGA
description: Geometry-aware cross-modal graph alignment for referring segmentation in 3D Gaussian Splatting. CVPR 2026 Poster · sole first author.
img: assets/img/projects/geocga_paper.png
importance: 2
category: computer-science
---

- **Full title:** *Geometry-Aware Cross-Modal Graph Alignment for Referring Segmentation in 3D Gaussian Splatting*
- **Highlights:**
  - ***CVPR 2026***, Poster session (Saturday June 6, 2026, 11:45 AM – 1:45 PM MDT, Vancouver)
- **Role:** Sole first author
- **Co-authors:** Kanglei Zhou (Tsinghua), Chang Li, Liyuan Wang
- **Links:** [CVPR virtual site (poster 38204)](https://cvpr.thecvf.com/virtual/2026/poster/38204) · [Paper walkthrough (YouTube)](https://www.youtube.com/watch?v=jtZWzR-rODs) · [Paper PDF]({{ 'assets/pdf/CVPR_26___8490___GeoCGA.pdf' | relative_url }})

### CVPR 2026 paper preview

The full 4800×2411 CVPR 2026 poster-paper covering motivation, method, and results. Click to zoom in, or [open the PDF]({{ 'assets/pdf/CVPR_26___8490___GeoCGA.pdf' | relative_url }}) for the vector version.

{% include figure.liquid path="assets/img/projects/geocga_paper.png" title="GeoCGA: CVPR 2026 poster-paper (4800×2411)." class="img-fluid rounded z-depth-1" zoomable=true %}

<div style="aspect-ratio: 16/9; width: 100%; margin: 1.5rem 0;">
  <iframe src="https://www.youtube.com/embed/jtZWzR-rODs" title="GeoCGA paper walkthrough" style="width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### The task (R3DGS)

- **Referring 3D Gaussian Splatting Segmentation** requires generating a 2D mask for a specific object given a natural-language description.
- Queries typically rely on **spatial relationships** rather than appearance (e.g. *"the bottle between the apple and the banana"*).
- The core challenge: resolving references when multiple objects share appearance but differ in position.

### Limitations of the prior SOTA

- Existing methods rely primarily on **appearance-based cross-modal matching**.
- Visually indistinguishable objects (e.g. identical bottles) collapse under appearance alone.
- Spatial relations in the text query are not grounded in the underlying 3D geometry.

### GeoCGA contributions

- **GeoCGA** (Geometry-Aware Cross-Modal Graph Alignment): a dual-graph framework for referring segmentation on 3D Gaussian Splatting scenes.
- **Scene graph.** Constructs an **object-level geometric graph** directly from the 3DGS field: nodes are object instances, edges encode spatial relations.
- **Text graph.** Parses the query into a **semantic–spatial graph** mirroring the structure of the scene graph.
- **Cross-modal alignment.** Matches the two graphs across modalities, grounding the referring expression in 3D geometry rather than appearance.

### Results

- mIoU gains over prior SOTA on three standard benchmarks:
  - **+28.8%** on Ref-LERF
  - **+2.6%** on LERF-OVS
  - **+3.1%** on 3D-OVS

### Significance

- A concrete step toward **physical AI**: aligning what a system sees in 3D with what a person actually means.
- The same alignment signal is directly usable by downstream **robot grasping and manipulation** pipelines.

### My contributions

- Designed both the geometric graph construction and the cross-modal alignment modules.
- Implemented the full training and evaluation pipeline across the three benchmarks.
- Authored the initial manuscript.
- Iterated on method and framing through weekly discussions with Dr. Zhou and co-authors.
