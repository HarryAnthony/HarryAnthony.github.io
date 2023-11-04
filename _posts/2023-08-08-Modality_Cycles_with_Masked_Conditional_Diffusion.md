---
layout: post
title:  "Modality cycles with masked conditional diffusion for unsupervised anomaly segmentation in MRI"
place: MMMI at MICCAI 2023
authors: Ziyun Liang, Harry Anthony, Felix Wagner & Konstantinos Kamnitsas
date:   2023-08-01 11:00:00 +0200
image: /images/masked_modality_cycle.png
categories: out-of-distribution-detection
paper: https://arxiv.org/abs/2308.16150
arxiv:
code: https://github.com/ZiyunLiang/MMCCD
poster: /docs/MICCAI_Conference_poster_Ziyun_Liang_2023.jpg
comments:
year: 2023 
---

<style>
@media (max-width: 768px) {
    .container {
        flex-direction: column;
        align-items: left;
    }
</style>


<div class="container" style="display: flex; align-items: center;">
    <div class="image" style="flex: 1; margin-right: 1cm;">
        <img src="/images/masked_modality_cycle.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2>Abstract</h2>
        <p>
Unsupervised anomaly segmentation aims to detect patterns that are distinct from any patterns processed during training, commonly called abnormal or out-of-distribution patterns, without providing any associated manual segmentations. Since anomalies during deployment can lead to model failure, detecting the anomaly can enhance the reliability of models, which is valuable in high-risk domains like medical imaging. This paper introduces Masked Modality Cycles with Conditional Diffusion (MMCCD), a method that enables segmentation of anomalies across diverse patterns in multimodal MRI.</p>
    </div>
</div>


The method is based on two fundamental ideas. First, we propose the use of cyclic modality translation as a mechanism for enabling abnormality detection. Image-translation models learn tissue-specific modality mappings, which are characteristic of tissue physiology. Thus, these learned mappings fail to translate tissues or image patterns that have never been encountered during training, and the error enables their segmentation. Furthermore, we combine image translation with a masked conditional diffusion model, which attempts to `imagine' what tissue exists under a masked area, further exposing unknown patterns as the generative model fails to recreate them. We evaluate our method on a proxy task by training on healthy-looking slices of BraTS2021 multi-modality MRIs and testing on slices with tumors. We show that our method compares favorably to previous unsupervised approaches based on image reconstruction and denoising with autoencoders and diffusion models.

Dive into our research!

<a href="https://arxiv.org/abs/2308.16150">&#x1F4C4; Paper</a> | <a href="/docs/MICCAI_Conference_poster_Ziyun_Liang_2023.jpg">&#x1F4CA; Poster</a> | <a href="https://github.com/ZiyunLiang/MMCCD">`</>` Code</a>