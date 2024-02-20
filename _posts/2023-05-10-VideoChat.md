---
title: VideoChat
author: Anonym
date: 2023-05-10 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [VideoChat: Chat-Centric Video Understanding](https://arxiv.org/abs/2305.06355)
- [GitHub Link](https://github.com/OpenGVLab/Ask-Anything)
- Publisher: `Arxiv`
- Author Affiliation: `Shanghai AI Laboratory & Nanjing University & The University of Hong Kong & Chinese Academy of Sciences`
- Functional Division
  + [x] Understanding
  + [ ] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + V+T $\rightarrow$ T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `V: ViT-G`
  + Input Projector
    * `Q-Former w/ Linear Projector`
  + LLM Backbone
    * `Vicuna`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
