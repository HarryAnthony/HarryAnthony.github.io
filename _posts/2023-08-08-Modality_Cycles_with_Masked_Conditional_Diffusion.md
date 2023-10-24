---
layout: post
title:  "Modality Cycles with Masked Conditional Diffusion for Unsupervised Anomaly Segmentation in MRI"
place: MMMI at MICCAI 2023
authors: Ziyun Liang, *Harry Anthony*, Felix Wagner & Konstantinos Kamnitsas
date:   2023-08-01 11:00:00 +0200
image: /images/masked_modality_cycle.png
categories: out-of-distribution-detection, outlier-detection
paper: https://arxiv.org/abs/2308.16150
arxiv:
code:
poster: 
comments:
year: 2023 
---

![](/images/masked_modality_cycle.png)


## Abstract

Unsupervised anomaly segmentation aims to detect patterns that are distinct from any patterns processed during training, commonly called abnormal or out-of-distribution patterns, without providing any associated manual segmentations. Since anomalies during deployment can lead to model failure, detecting the anomaly can enhance the reliability of models, which is valuable in high-risk domains like medical imaging. This paper introduces Masked Modality Cycles with Conditional Diffusion (MMCCD), a method that enables segmentation of anomalies across diverse patterns in multimodal MRI. The method is based on two fundamental ideas. First, we propose the use of cyclic modality translation as a mechanism for enabling abnormality detection. Image-translation models learn tissue-specific modality mappings, which are characteristic of tissue physiology. Thus, these learned mappings fail to translate tissues or image patterns that have never been encountered during training, and the error enables their segmentation. Furthermore, we combine image translation with a masked conditional diffusion model, which attempts to `imagine' what tissue exists under a masked area, further exposing unknown patterns as the generative model fails to recreate them. We evaluate our method on a proxy task by training on healthy-looking slices of BraTS2021 multi-modality MRIs and testing on slices with tumors. We show that our method compares favorably to previous unsupervised approaches based on image reconstruction and denoising with autoencoders and diffusion models.