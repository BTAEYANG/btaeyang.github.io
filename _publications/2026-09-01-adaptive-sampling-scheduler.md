---
title: "Training-Free Adaptive Sampling Scheduler for Discrete-Time Consistency Distillation"
collection: publications
category: conferences
permalink: /publication/2026-09-01-adaptive-sampling-scheduler
excerpt: 'Few-step consistency models fail not because the student is weak but because the sampling schedule is rigid. We score every timestep by an SNR-derived Importance measure, spend the same step budget where the trajectory actually moves, and add a matching sampler and colour-balancing pass. No retraining is required, and the method drops into LCM, PCM, TCD and TDD. At 2 sampling steps FID falls by up to 86%.'
date: 2026-09-01
venue: 'International Conference on Artificial Neural Networks (ICANN)'
citation: 'Qi Wang and Jinjia Zhou. (2026). &quot;Training-Free Adaptive Sampling Scheduler for Discrete-Time Consistency Distillation.&quot; <i>International Conference on Artificial Neural Networks (ICANN)</i>.'
---

Discrete-time consistency distillation methods each ship a timestep schedule welded to their own
training framework and step budget, so they degrade as soon as the scheduler or the step count changes
at inference time. We show that the schedule, not the student, is the bottleneck.

**Method.** An SNR-derived *Importance* measure scores each timestep by the normalised inverse rate of
change of log-SNR; it peaks in the middle of the trajectory, where structure actually forms. Candidates
above a threshold replace uniform-grid steps, so the step count never changes — only its spacing. A
$$\gamma$$-I sampler scales noise re-injection by the local Importance instead of a constant, and a
tanh soft clamp with channel and global mean re-centring removes the colour drift that classifier-free
guidance compounds at low step counts.

**Results.** Across LCM, PCM, TCD and TDD on both SDXL (1024×1024) and SD v1.5 (512×512), every
baseline improves on FID, CLIP Score and Inception Score at 2, 4 and 8 sampling steps. The gains
concentrate where few-step sampling is weakest: at 2 steps FID falls 82–86% for PCM and TCD. The method
is training-free, adds no parameters, and costs negligible runtime.

[**Read the full illustrated summary**](/icann2026/) — equations, the complete results table and every
figure, formatted for reading on a phone.

[**Download the conference poster (A0, PDF)**](/files/ICANN2026_poster.pdf)

*Supported by JSPS KAKENHI JP25K15165 and the Kayamori Foundation of Informational Science Advancement.*
