---
title: ModaVerse
author: Anonym
date: 2024-01-12 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [ModaVerse: Efficiently Transforming Modalities with LLMs](https://arxiv.org/abs/2401.06395)
- GitHub Link: `None`
- Publisher: `Arxiv`
- Author Affiliation: `University of Adelaide`
- Functional Division
  + [ ] Understanding
  + [x] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I+V+A+T $\rightarrow$ I+V+A+T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `ImageBind`
  + Input Projector
    * `Linear Projector`
  + LLM Backbone
    * `LLaMA-2`
  + Output Projector
    * `MLP`
  + Modality Generator
    * `I: Stable Diffusion`
    * `V: Videofusion`
    * `A: AudioLDM`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
