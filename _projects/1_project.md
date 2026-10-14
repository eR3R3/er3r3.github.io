---
layout: page
title: CaRF
description: Camera-aware cross-view alignment for referring 3D Gaussian Splatting segmentation. ICME 2026 Oral (Top 5%) · Team China ISEF 2026 (Shanghai delegation) · sole first author.
img: assets/img/projects/carf_quadchart.png
importance: 1
category: computer-science
related_publications: true
after_references_image: assets/img/projects/carf_challenge_13.png
after_references_caption: ICME 2026 Oral (Bangkok) presentation. Closing slide.
---

{% include figure.liquid path="assets/img/projects/carf_title_banner.png" title="CaRF: Camera Aware Referring Field (ISEF 2026, TECA020)" class="img-fluid rounded z-depth-1" zoomable=true %}

- **Full title:** *CaRF: Camera-Aware Cross-View Alignment for Referring 3D Gaussian Splatting Segmentation*
- **Highlights:**
  - IEEE ICME 2026, oral presentation (top 5%)
  - Shanghai representative on **Team China** at the ***2026 Regeneron ISEF***, project **TECA020** (Technology Enhances the Arts)
  - **Outstanding Student Award**, Science Talent Program (Yingcai), Shanghai cohort
- **Role:** Sole first author
- **Mentors:** Xin Tan and Yuan Xie (ECNU)
- **Second-draft reviewer:** Kanglei Zhou (Tsinghua)
- **Program:** **Science Talent Program (Yingcai), Shanghai**. 2025 cohort (admission rate 62/1033), jointly organized by the **Ministry of Education of China** and the **China Association for Science and Technology (CAST)**.
- **Links:** [arXiv:2511.03992](https://arxiv.org/abs/2511.03992) · [GitHub (eR3R3/CaRF)](https://github.com/eR3R3/CaRF) · [ISEF project page](https://isef.net/project/teca020-carf-camera-aware-referring-field) · [ISEF presentation (YouTube)](https://www.youtube.com/watch?v=kEip8v9I2Q8)

### ISEF quad chart

{% include figure.liquid path="assets/img/projects/carf_quadchart.png" title="CaRF ISEF 2026 quad chart: research question, methodology, results, and conclusion." class="img-fluid rounded z-depth-1" zoomable=true %}

### Full research poster

The complete 4608×4608 poster covering motivation, methodology, ablations, iterations, and results. Click to zoom in, or [open at full resolution]({{ 'assets/img/projects/carf_full_poster.png' | relative_url }}) in a new tab.

{% include figure.liquid path="assets/img/projects/carf_full_poster.png" title="CaRF full research poster: 9 sections including Introduction, Methodology, Ablation Study, Iterations, Limitations, and Conclusion." class="img-fluid rounded z-depth-1" zoomable=true %}

<div style="aspect-ratio: 16/9; width: 100%; margin: 1.5rem 0;">
  <iframe src="https://www.youtube.com/embed/kEip8v9I2Q8" title="2026 ISEF Finalist Project CaRF" style="width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### The task (R3DGS)

- **Referring 3D Gaussian Splatting Segmentation** was introduced in the ICML 2025 oral paper *ReferSplat*.
- Unlike earlier 3D segmentation work that just **selects** an object, R3DGS asks the model to **generate an actual 2D mask**.
- The text query includes adjectives and spatial relationships (e.g. *"the small bottle to the left of the apple."*).

### Limitations of the prior SOTA

- *ReferSplat*'s cross-modal alignment captures spatial semantics effectively.
- Reproduction reveals **substantial mask-quality degradation under novel views**.
- A given object may be partially segmented or contaminated by neighbors under pose variation.

### CaRF contributions

- **CaRF** (Camera-Aware Referring Field): a differentiable framework enforcing **multi-view consistency at training time**.
- **ITPVS (In-Training Paired-View Supervision).** Jointly supervises Gaussians under **two overlapping views per iteration**, exposing the model to inter-view discrepancies directly.
- **GFCE (Gaussian Field Camera Encoding).** Injects **encoded camera features** into text-to-Gaussian alignment, providing geometric priors for the view variation induced by ITPVS.

### Results

- Surpasses all state-of-the-art methods in mIoU on three standard benchmarks (**Ref-LERF, LERF-OVS, 3D-OVS**).
- Largest gain on **Ref-LERF**: 25.0 → 29.2 average mIoU (**+16.8% relative** over ReferSplat).

### Significance

- Robustness under viewpoint change is a prerequisite for deployment in **embodied AI and AR/VR** systems.
- Camera pose is unconstrained in these settings; cross-view consistency is a necessary condition, not an optimization.

### My contributions

- Surveyed prior R3DGS literature and identified cross-view inconsistency as the dominant failure mode.
- Designed both proposed modules (ITPVS and GFCE).
- Implemented the full training and evaluation pipeline; conducted cross-scene and cross-view analyses.
- Authored the initial manuscript.
- Iterated on the method through weekly reviews with mentors.

### Code

{% include repository/repo.liquid repository="eR3R3/CaRF" %}

<div style="margin-top: 3rem;"></div>

### Supplementary materials

Slides from the talk I gave at the ICME 2026 Oral session in Bangkok. Click any slide to zoom.

<div class="row mt-3">
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_01.png" title="ICME 2026 Oral slide 1" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_02.png" title="ICME 2026 Oral slide 2" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_03.png" title="ICME 2026 Oral slide 3" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="row mt-3">
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_04.png" title="ICME 2026 Oral slide 4" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_05.png" title="ICME 2026 Oral slide 5" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_06.png" title="ICME 2026 Oral slide 6" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="row mt-3">
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_07.png" title="ICME 2026 Oral slide 7" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_08.png" title="ICME 2026 Oral slide 8" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_09.png" title="ICME 2026 Oral slide 9" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="row mt-3">
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_10.png" title="ICME 2026 Oral slide 10" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_11.png" title="ICME 2026 Oral slide 11" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_challenge_12.png" title="ICME 2026 Oral slide 12" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>

<div style="margin-top: 2rem;"></div>

#### Team China at Regeneron ISEF 2026, Phoenix

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_isef_team_china.jpg" title="Team China (Shanghai delegation) at Regeneron ISEF 2026, Phoenix." class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/carf_isef_team_photo.jpg" title="Team China group photo at the Regeneron ISEF 2026 backdrop." class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
