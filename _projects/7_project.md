---
layout: page
title: Sashimiyo
description: Lane-based sushi tower defense in Unity. Made at CMU National High School Game Academy, summer 2026.
img: assets/img/projects/sashimyo_1.png
importance: 7
category: computer-science
---

- **Engine:** Unity
- **Made at:** Carnegie Mellon University, National High School Game Academy, summer 2026
- **My role:** Gameplay programmer; later producer

### Overview

Sashimiyo is a lane-based tower-defense game where the enemies are anthropomorphic sushi marching toward you. The theme is light; the design work isn't. Lane pacing, enemy variety, upgrade economy, and the shape of the difficulty curve were the parts that took the real iteration.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_1.png" title="Sashimiyo gameplay" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_2.png" title="Sashimiyo level" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_3.png" title="Sashimiyo tower placement" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_4.png" title="Sashimiyo enemies" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_5.png" title="Sashimiyo wave" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/sashimyo_6.png" title="Sashimiyo UI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">Screens from the sushi tower-defense build. Made at CMU National High School Game Academy, summer 2026.</div>

### My contributions

- Core gameplay loop in C# — unit spawning, pathing, tower placement, projectile systems.
- Design iteration on the economy: how fast players earn resources, how expensive late-game towers should be, how to make upgrade decisions interesting rather than obvious.
- Collaboration with the art team on readability — enemies had to be distinguishable at a glance even at a distance from the tower rows.
