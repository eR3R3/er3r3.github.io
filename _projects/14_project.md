---
layout: page
title: Evaluating Olympic Sports
description: Two-stage AHP + TOPSIS decision model for which sports should enter future Olympics. HiMCM 2024 Problem A · Meritorious Award (Top 13%).
img: assets/img/projects/himcm_2024_cover.png
importance: 3
category: math
---

- **Contest:** HiMCM 2024, Problem A
- **Team:** 15621
- **Result:** Meritorious Award (top 13%)

### The question

If the International Olympic Committee had to decide which sports, disciplines, or events (SDEs) to add to a future Olympic Games using a reproducible evaluation framework rather than a one-off political decision, what should that framework look like?

### Our approach

We built a two-stage model.

- **Stage 1 — Analytic Hierarchy Process (AHP).** We identified six IOC criteria (popularity and accessibility, gender equity, sustainability, infrastructure demand, athlete welfare, youth appeal) and ten underlying factors, then used pairwise comparisons to produce a logical weighting across them.
- **Stage 2 — TOPSIS.** We scored each candidate sport by how closely it matched an "ideal" sport profile, weighted by the AHP output. TOPSIS gave us a clean, interpretable ranking rather than a black-box score.

### Performance

On historical IOC decisions, our ranking recovered them with **73.91% accuracy, 83.02% precision, 83.02% recall** — strong enough to argue the framework is capturing real IOC preferences rather than noise.

### Takeaways

Modeling contests teach you that "building a model" is less about picking fancy methods and more about picking methods whose assumptions you can defend to a reader. AHP + TOPSIS is a cliché combination for a reason: the weights are explicit, the ranking is explicit, and you can argue with every step of it.

### The paper

<iframe src="{{ '/assets/pdf/2024HiMCM15621.pdf' | relative_url }}"
        width="100%" height="1100px"
        style="border: 1px solid #ccc; border-radius: 4px; margin: 1.5rem 0;">
</iframe>

[Download PDF]({{ '/assets/pdf/2024HiMCM15621.pdf' | relative_url }})
