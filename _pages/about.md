---
permalink: /
title: "Qi Wang"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a graduate researcher at iMediaLab, Graduate School of Science and Engineering,
**Hosei University**, Tokyo, working with Prof. Jinjia Zhou.

My research is on **making diffusion models usable at very small step budgets** — consistency
distillation, sampling schedules, and the failure modes that appear when a model trained for many
denoising steps is asked to run in two or four.

Current work
======
**Training-Free Adaptive Sampling Scheduler for Discrete-Time Consistency Distillation** —
*ICANN 2026*

Discrete-time distillation methods each ship a sampling schedule welded to their own training framework,
so they degrade as soon as the scheduler or the step count changes at inference. We show the schedule,
not the student, is the bottleneck: an SNR-derived *Importance* measure says which timesteps carry the
structural change, the same step budget is redistributed toward them, and a matching sampler and
colour-balancing pass clean up what classifier-free guidance compounds. The method needs no retraining
and drops into LCM, PCM, TCD and TDD; at 2 sampling steps FID falls by up to 86%.

- [Illustrated summary](/icann2026/) — equations, full results table and every figure, readable on a phone
- [Conference poster (A0, PDF)](/files/ICANN2026_poster.pdf)

Contact
======
<qi.wang.7c@stu.hosei.ac.jp>
