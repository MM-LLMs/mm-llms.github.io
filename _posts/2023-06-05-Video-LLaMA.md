---
title: Video-LLaMA
author: Anonym
date: 2023-06-05 00:00:00 +0800
categories: [EMNLP 2023]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding](https://arxiv.org/abs/2306.02858)
- [GitHub Link](https://github.com/DAMO-NLP-SG/Video-LLaMA)
- Publisher: `EMNLP 2023`
- Author Affiliation: `Alibaba Group`
- Functional Division
  + [x] Understanding
  + [ ] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text)
  + I+V+A+T $\rightarrow$ T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `I/V: Eva-CLIP ViT-G/14`
    * `A: ImageBind`
  + Input Projector
    * `Q-Former w/ Linear Projector`
  + LLM Backbone
    * `Vicuna/LLaMA`
  + Output Projector
    * `None`
  + Modality Generator
    * `None`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
