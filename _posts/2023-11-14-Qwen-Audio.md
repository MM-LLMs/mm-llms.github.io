---
title: Qwen-Audio
author: Anonym
date: 2023-11-14 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [Qwen-Audio: Advancing Universal Audio Understanding via Unified Large-Scale Audio-Language Models](https://arxiv.org/abs/2311.07919)
- [GitHub Link](https://github.com/QwenLM/Qwen-Audio)
- Publisher: `Arxiv`
- Author Affiliation: `Alibaba Group`
- Functional Division
  + [x] Understanding
  + [ ] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + A+T $\rightarrow$ T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `A: Whisper-L-v2`
  + Input Projector
    * `Linear Projector`
  + LLM Backbone
    * `Qwen-7B`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
