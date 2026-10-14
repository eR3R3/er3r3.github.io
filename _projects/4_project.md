---
layout: page
title: IronPulse Scouting
description: Web-based scouting & analytics platform for FRC 6941 IronPulse Robotics. TypeScript / NestJS / Next.js / PostgreSQL. Used by our drive team to argue strategy from data.
img: assets/img/projects/ironpulse_2_home.png
importance: 3
category: computer-science
---

- **Role:** Programming Leader (sole lead over 20+ programmers)
- **Season:** REEFSCAPE 2025 — team qualified for the **FIRST Championship in Houston**
- **Stack:** TypeScript · NestJS · Next.js · PostgreSQL

### Overview

A web-based scouting platform that captures match data and surfaces analytics for strategic decisions. Scouts enter per-match and pit observations through a mobile-first UI; the dashboard aggregates performance across teams so our strategy meetings can argue from data rather than impressions.

#### Authentication & home

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_1_signin.png" title="Sign-in page" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Sign-in — team-scoped auth.</div>
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_2_home.png" title="Home" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Home — entry point to match / pit scouting and analytics.</div>
  </div>
</div>

#### Scouting entry

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_3_pitscouting.png" title="Pit scouting form" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Pit scouting — mobile-first form filled before matches.</div>
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_5_match_record.png" title="Match record" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Match record — per-match scouting entries.</div>
  </div>
</div>

#### Analytics dashboard

<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_4_team_comparison.png" title="Team performance comparison" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Team performance comparison — strategy meeting view.</div>
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_6_match_stats.png" title="Match statistics" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Match statistics — aggregated performance metrics.</div>
  </div>
</div>
<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_7_match_details.png" title="Match details" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Match details — drill into a single match.</div>
  </div>
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_8_match_view_stats.png" title="Match detail — stats view" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Match detail — stats view.</div>
  </div>
</div>
<div class="row mt-3">
  <div class="col-md-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/ironpulse_9_pit_viewer.png" title="Pit scout viewer" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Pit-scout viewer — browse pre-match team notes.</div>
  </div>
</div>

### Team impact

A scouting pipeline that converts the chaos of a competition day into something a strategy meeting can actually reason over. Instead of relying on who-remembers-what, our drive team walks into alliance selection with ranked candidates, drill-down match detail, and side-by-side team comparisons.
