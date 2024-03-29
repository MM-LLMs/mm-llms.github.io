---
title: InstructBLIP
author: Anonym
date: 2023-05-11 00:00:00 +0800
categories: [NeurIPS 2023]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [InstructBLIP: Towards General-purpose Vision-Language Models with Instruction Tuning](https://arxiv.org/abs/2305.06500)
- [GitHub Link](https://github.com/salesforce/LAVIS/tree/main/projects/instructblip)
- Publisher: `NeurIPS 2023`
- Author Affiliation: `Salesforce Research`
- Functional Division
  + [x] Understanding
  + [ ] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I+V+T $\rightarrow$ T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `I/V: ViT-G/14@224`
  + Input Projector
    * `Q-Former w/ Linear Projector`
  + LLM Backbone
    * `Flan-T5/Vicuna`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `129M`
  + Instruction-tuning Stage
    * `1.2M`
