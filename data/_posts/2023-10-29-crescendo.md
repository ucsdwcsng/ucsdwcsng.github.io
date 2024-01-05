---
layout: publication
title: "Crescendo: Towards Wideband, Real-Time,
High-Fidelity Spectrum Sensing Systems"
short_title: "Crescendo"
tags: Spectrum-Sensing Communications
cover: /assets/images/pubpic/crescendo.png
authors: "Raghav Subbaraman, Kevin Mills, Aaron Schulman, Dinesh Bharadia"
conference: "MobiCom 2023"
paper: https://dl.acm.org/doi/abs/10.1145/3570361.3613294
github: https://github.com/ucsdwcsng/crescendo
slides: https://sigmobile.org/mobicom/2023/media/presentations/SubbaramanCrescendo.pdf
osd: "The artifact provides data and code to analyze the case-study evaluations in the paper"
---

Spectrum sensing systems provide real-time feedback essential for spectrum sharing. However, the growth of spectrum sharing is limited by the capabilities of these spectrum sensors. Sharing a new frequency band is only possible if sensors
can detect activity in that band with sufficient time granularity and signal fidelity to meet spectrum sharing policy
requirements. In this work, we introduce Crescendo, a system design that shows we can achieve wideband, real-time,
high-fidelity spectrum sensing using sweeping spectrum sensors. We first provide an analysis that demonstrates there are
operating points of sweeping sensors that can sense multiple
popular protocols. Then we demonstrate these sensors can
be built in practice with an adaptive gain superheterodyne
RF frontend with high-fidelity LO generation, and evaluate a
prototype built with COTS components. In our benchmarks,
Crescendo outperforms prior wideband spectrum sensors,
achieving a 30 dB increase in dynamic range and 10 dB in-
crease in SNR.
