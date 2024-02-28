---
title: SkyEyeGPT
author: Anonym
date: 2024-01-18 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [SkyEyeGPT: Unifying Remote Sensing Vision-Language Tasks via Instruction Tuning with Large Language Model](https://arxiv.org/pdf/2401.09712.pdf)
- [GitHub Link](https://github.com/ZhanYang-nwpu/SkyEyeGPT)
- Publisher: `Arxiv`
- Author Affiliation: `Northwestern Polytechnical University`
- Functional Division
  + [ ] Understanding
  + [x] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I/V+T $\rightarrow$ I<sub>B</sub>+T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `I/V: EVA-CLIP`
  + Input Projector
    * `Linear Projector`
  + LLM Backbone
    * `LLaMA2-chat`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
