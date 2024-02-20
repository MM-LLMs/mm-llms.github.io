---
title: LLaVA-Plus
author: Anonym
date: 2023-11-09 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [LLaVA-Plus: Learning to Use Tools for Creating Multimodal Agents](https://arxiv.org/abs/2311.05437)
- [GitHub Link](https://llava-vl.github.io/llava-plus/)
- Publisher: `Arxiv`
- Author Affiliation: `Tsinghua University`
- Functional Division
  + [ ] Understanding
  + [x] Generation
- Design Division
  + [x] Tool-using
  + [ ] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I+T $\rightarrow$ I+I<sub>M</sub>+I<sub>B</sub>+T
