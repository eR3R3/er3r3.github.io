---
layout: page
title: Sustainable Mega-Event Hosting
description: Life-cycle GHG footprint of the Super Bowl + a city-level sustainability index to pick the 2029 host and reshape the World Cup. HiMCM 2025 Problem B.
img: assets/img/projects/himcm_2025_cover.png
importance: 4
category: math
---

- **Contest:** HiMCM 2025, Problem B
- **Team:** 17252

### The question

Mega sports events — Super Bowl, Olympics, World Cup — generate concentrated environmental impact in a very short window: travel, lodging, stadium energy, water, waste. But host-city selection almost never treats environmental performance as the *primary* criterion. What would change if it did?

### Our three-layer model

- **Model 1 — Life-cycle event footprint.** Using Super Bowl LIX in New Orleans as a baseline, we decomposed emissions into long-distance travel, local transport, stadium energy, hotels, food, water, and waste. Published emission factors were combined with event-specific data to compute total and per-spectator GHG emissions.
- **Model 2 — City-level sustainability score \\(S_c\\).** We normalized five indicators per candidate city — per-spectator GHG emissions, electricity carbon intensity, regional water stress, waste-diversion performance, and a travel metric combining transit access and distance from the U.S. fan base — then combined them into a weighted linear index (lower = more sustainable).
- **Model 3 — Tournament format optimization.** We extended the framework beyond a single-site event to a *distributed-tournament* design that could lower the carbon footprint of a World Cup.

### Outcomes

- A ranking of candidate U.S. cities for **Super Bowl 2029** based on environmental cost alone.
- A reusable framework for other sport mega-events — the same \\(S_c\\) can be recomputed with different event-specific inputs.
- A concrete demonstration that re-weighting a single criterion (environmental impact → dominant) shifts host selection enough to matter.

### Takeaways

Modeling environmental decisions means being honest about where your numbers come from — published emission factors are not the same as measured ones, and you have to argue for your inputs as hard as you argue for your model. That discipline carries over into every applied-ML project where benchmark numbers can look authoritative without being so.

### The paper

<iframe src="{{ '/assets/pdf/2025HiMCM17252.pdf' | relative_url }}"
        width="100%" height="1100px"
        style="border: 1px solid #ccc; border-radius: 4px; margin: 1.5rem 0;">
</iframe>

[Download PDF]({{ '/assets/pdf/2025HiMCM17252.pdf' | relative_url }})
