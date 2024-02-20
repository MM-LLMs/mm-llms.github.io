---
title: MM-Interleaved
author: Anonym
date: 2024-01-18 00:00:00 +0800
categories: [Arxiv]
tags: [MM-LLMs]
math: true
pin: false
---

- Paper: [MM-Interleaved: Interleaved Image-Text Generative Modeling via Multi-modal Feature Synchronizer](https://browse.arxiv.org/abs/2401.10208)
- [GitHub Link](https://github.com/OpenGVLab/MM-Interleaved)
- Publisher: `Arxiv`
- Author Affiliation: `Shanghai AI Laboratory`
- Functional Division
  + [ ] Understanding
  + [x] Generation
- Design Division
  + [ ] Tool-using
  + [x] End-to-end
- Input Modalities $\rightarrow$ Output Modalities <br />(I: Image, V: Video, A: Audio, 3D: Point Cloud, T: Text, I<sub>D</sub>: Document understanding, I<sub>B</sub>: Output bounding box, I<sub>M</sub>: Output segmentation mask, I<sub>R</sub>: Output retrieved images)
  + I+T $\rightarrow$ I+T
- Model Architecture <br />(Input $\rightarrow$ Modality Encoder $\rightarrow$ Input Projector $\rightarrow$ LLM Backbone $\rightarrow$ Output Projector $\rightarrow$ Modality Generator $\rightarrow$ Output)
  + Modality Encoder
    * `I: CLIP ViT-L/14`
  + Input Projector
    * `Cross-attention`
  + LLM Backbone
    * `Vicuna-13B`
  + Output Projector
    * `Tiny Transformer`
  + Modality Generator
    * `I: Stable Diffusion-2.1`
- Datasets Scale
  + Pre-training Stage
    * `Not report`
  + Instruction-tuning Stage
    * `Not report`
