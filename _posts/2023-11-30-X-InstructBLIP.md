---
title: X-InstructBLIP
author: Anonym
date: 2023-11-30 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [X-InstructBLIP: A Framework for aligning X-Modal instruction-aware representations to LLMs and Emergent Cross-modal Reasoning](https://arxiv.org/abs/2311.18799)
- [GitHub Link](https://github.com/artemisp/LAVIS-XInstructBLIP)
- Publisher: `Arxiv`
- Author Affiliation: `University of Pennsylvania`
- Functional Division
  + [x] Understanding
  + [ ] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I+A+V+3D+T $\rightarrow$ T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `I/V: Eva-CLIP ViT-G/14`
    * `A: BEATs`
    * `3D: ULIP-2`
  + Input Projector
    * `Q-Former w/ Linear Projector`
  + LLM Backbone
    * `Vicuna-v1.1-7B/13B`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
