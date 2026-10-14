---
layout: page
title: Silent Speak
description: Portable lip-language-to-text system — a vision module + AR glasses that displays the converted text on the lens. For tracheostomy patients and high-noise industrial workers. Silver Prize at AdventureX 2025 (Even Reality Track).
img: assets/img/projects/silentspeak_product.png
importance: 4
category: computer-science
---

- **Venue:** AdventureX 2025 (Hangzhou), Even Reality Track
- **Award:** Silver Prize
- **Collaborators:** 3 co-leaders from PHCS
- **Project page:** [AdventureX gallery](https://gallery.adventure-x.cn/projects/2500d2b4-87f2-43a3-89fa-a14aa05e9ea9)

### Product

{% include figure.liquid path="assets/img/projects/silentspeak_product.png" title="Silent Speak — product definition: Lip Link Cam + Even G1 AR glasses." class="img-fluid rounded z-depth-1" zoomable=true %}

Silent Speak is a **portable lip-language-to-text conversion solution** made of two parts:

- **Lip Link Cam** — a vision hardware module with onboard computing. It captures lip movement and runs the lip-reading pipeline.
- **Even G1** — commercial AR glasses (made by Even Realities, our track sponsor). Converted text appears **directly on the lens**, in-view, no second screen required.

### Target users

- **Tracheostomy patients** who have lost normal voicing but retain mouth movement — they get a wearable interface for speaking that doesn't require typing on a phone.
- **Industrial workers** in environments too loud for speech recognition to work — the lip signal is independent of the audio noise floor.

### System overview

A **fine-tuned Vision Transformer** backbone does the lip-reading. The Lip Link Cam captures frames and performs on-device inference; results stream to the Even G1 over Bluetooth and are rendered as text on the lens. The whole pipeline runs quietly enough to be a continuous wearable rather than a one-shot tool.

### My contributions

- Led **Bluetooth communication development** between the Lip Link Cam and the Even G1 glasses.
- Led **AI model fine-tuning** of the Vision Transformer lip-reading backbone.
- Co-led system integration across the camera module, the glasses, and the host.

### Motivation

Lip-reading is a problem where the input signal is deliberately uncoupled from audio, which makes it a clean place to practice end-to-end multimodal perception. It also had the quality I look for in a project: a specific person who would actually use the result.
