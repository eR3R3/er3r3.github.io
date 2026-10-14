---
layout: page
title: IronPulse Robot
description: Subsystem state-machine code for FRC 6941 IronPulse's REEFSCAPE 2025 robot. Programming leader; team qualified for the FIRST Championship in Houston.
img: assets/img/projects/ironpulse_robot_cover.png
importance: 5
category: computer-science
---

- **Role:** Programming Leader (sole lead over 20+ programmers)
- **Season:** REEFSCAPE 2025 — team qualified for the **FIRST Championship in Houston**
- **Team:** FRC 6941 IronPulse
- **Robot:** Specter
- **Channel:** [@ironpulse6941 on YouTube](https://www.youtube.com/@ironpulse6941)

### The robot — Specter (2025 REEFSCAPE reveal)

<div style="aspect-ratio: 16/9; width: 100%; margin: 1.5rem 0;">
  <iframe src="https://www.youtube.com/embed/BarYC6-Ouvs" title="2025 Reefscape Season Reveal — Specter" style="width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### 2025 REEFSCAPE season

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    <div style="aspect-ratio: 16/9; width: 100%;">
      <iframe src="https://www.youtube.com/embed/M2BQYoAS8Uo" title="2025 REEFSCAPE Regional Recap" style="width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
    <div class="caption">2025 REEFSCAPE Regional Recap — how the season played out.</div>
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    <div style="aspect-ratio: 16/9; width: 100%;">
      <iframe src="https://www.youtube.com/embed/R2uDv7KkPEE" title="Chasing Dreams — Impact Award Video 2025" style="width: 100%; height: 100%; border: 0;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
    <div class="caption">Chasing Dreams — IronPulse's Impact Award video, 2025.</div>
  </div>
</div>

### Building the robot

Behind-the-scenes footage and photos from the shop — assembly, iteration, testing.

<div style="aspect-ratio: 16/9; width: 100%; margin: 1.5rem 0;">
  <video src="{{ 'assets/video/ironpulse_robot_build.mp4' | relative_url }}" controls style="width: 100%; height: 100%; object-fit: contain; background: black;"></video>
</div>

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_robot_cover.jpg" title="In the shop" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_robot_build.jpg" title="Build session" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>

### My contributions

State-machine code for the robot's subsystems — intake, arm, elevator, scoring mechanism. In a competition robot, each subsystem has to transition between well-defined states quickly and predictably — *intake running*, *intake stowed*, *arm scoring*, *arm resetting* — because the drive team is making decisions on a 15-second time budget.

State machines are the right abstraction for this because:
- The behavior is **legible** to both software and the drivers. The drive team can learn the robot by learning the state names.
- Transitions are **explicit**. Illegal moves (e.g. extending the arm while stowed) are physically impossible rather than relying on code discipline.
- Debugging under competition pressure is **tractable**. You can see which state the subsystem thinks it's in and reason about why.

### Cross-project connections

Robotics made spatial understanding feel like a *concrete* problem rather than an academic one. The robot needs on-field 3D localization, and that overlapped directly with the computer-vision research (CaRF, GeoCGA) I was doing. Working across the robot code and the scouting software made me think about how each technical decision would eventually affect what the drive team could do on the field.

### Also

For the matching web platform that captures and surfaces this match data, see **[IronPulse Scouting](/projects/4_project/)**.
