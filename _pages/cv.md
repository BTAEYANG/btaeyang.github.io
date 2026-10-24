---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education and research
======
* Graduate researcher, iMediaLab, Graduate School of Science and Engineering, Hosei University, Tokyo, Japan
  * Advisor: Prof. Jinjia Zhou
  * Research: efficient diffusion sampling, consistency distillation, knowledge distillation

Research interests
======
* Few-step diffusion sampling and consistency distillation
* Knowledge distillation and model compression
* Efficient image generation, inpainting and restoration
* Efficient video coding

Skills
======
* Generative models: diffusion models, consistency models, few-step sampling
* Model efficiency: knowledge distillation, contrastive objectives, sampling-schedule design
* Image and video: inpainting, style transfer, learned video coding
* Evaluation: FID, CLIP Score, Inception Score

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Talks and presentations
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>

Profiles
======
* [Google Scholar](https://scholar.google.com/citations?user=4ljiSLsAAAAJ) — 39 citations, h-index 4, i10-index 1
* [ORCID](https://orcid.org/0009-0007-9056-9522)
* [GitHub](https://github.com/BTAEYANG)
