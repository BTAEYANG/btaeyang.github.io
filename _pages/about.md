---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a graduate researcher at iMediaLab, Graduate School of Science and Engineering,
**Hosei University**, Tokyo, working with Prof. Jinjia Zhou.

My research is about **making generative and discriminative models cheaper to run without
giving up quality**. My current work is on diffusion models at very small step budgets:
consistency distillation, sampling schedules, and the failure modes that appear when a model
trained for many denoising steps is asked to run in two or four. Before that, I worked on
knowledge distillation — contrastive and correlation-based objectives that transfer what a
large network knows into a smaller one — and on efficient image and video processing,
including inpainting, style transfer and video coding.

Research interests
======
* Few-step diffusion sampling and consistency distillation
* Knowledge distillation and model compression
* Efficient image generation, inpainting and restoration
* Efficient video coding

News
======
* **[09/2026]** Our paper on adaptive sampling for consistency distillation was presented at
  **ICANN 2026** in Padua, Italy. [Poster (PDF)](/files/ICANN2026_poster.pdf)
* **[07/2026]** **Top-KD: Top-scaled contrastive knowledge distillation** was published in
  *Neurocomputing*. [DOI](https://doi.org/10.1016/j.neucom.2026.133636)
* **[02/2026]** Our work on efficient video coding was published in *Sensors*.
  [DOI](https://doi.org/10.3390/s26051522)

Selected publication
======
**Training-Free Adaptive Sampling Scheduler for Discrete-Time Consistency Distillation**
Qi Wang and Jinjia Zhou. *International Conference on Artificial Neural Networks (ICANN)*, 2026.
[DOI](https://doi.org/10.1007/978-3-032-38404-1_33) ·
[Illustrated summary](/icann2026/) ·
[Conference poster (A0, PDF)](/files/ICANN2026_poster.pdf)

Discrete-time distillation methods each ship a sampling schedule welded to their own training
framework, so they degrade as soon as the scheduler or the step count changes at inference.
We show the schedule, not the student, is the bottleneck: an SNR-derived *Importance* measure
says which timesteps carry the structural change, the same step budget is redistributed toward
them, and a matching sampler and colour-balancing pass clean up what classifier-free guidance
compounds. The method needs no retraining and drops into LCM, PCM, TCD and TDD; at 2 sampling
steps FID falls by up to 86%.

See the [full publication list](/publications/) for my earlier work on knowledge distillation,
image inpainting and video coding.

Contact
======
<qi.wang.7c@stu.hosei.ac.jp> · [Google Scholar](https://scholar.google.com/citations?user=4ljiSLsAAAAJ) (39 citations, h-index 4) · [ORCID](https://orcid.org/0009-0007-9056-9522)
