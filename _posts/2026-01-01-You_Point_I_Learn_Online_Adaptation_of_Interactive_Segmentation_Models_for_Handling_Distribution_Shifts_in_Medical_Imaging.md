---
layout: post
title: "You Point, I Learn: Online Adaptation of Interactive Segmentation Models for Handling Distribution Shifts in Medical Imaging"
place: ICLR 2026
authors: Wentian Xu, Ziyun Liang, Harry Anthony, Yasin Ibrahim, Felix Cohen, Guang Yang & Konstantinos Kamnitsas
date:   2026-01-01 12:00:00 +0200
image: /images/Interactive_segmentation.png
categories: out-of-distribution-detection
paper:
arxiv:
code: 
poster:
presentation:
comments:
year: 2025
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
        <img src="/images/Interactive_segmentation.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2> Interactive Segmentation Pipeline </h2>
        <p> Interactive segmentation uses real-time user inputs, such as mouse clicks, to iteratively refine model predictions. Although not originally designed to address distribution shifts, this paradigm naturally lends itself to such challenges. In medical imaging, where distribution shifts are common, interactive methods can use user inputs to guide models towards improved predictions. Moreover, once a model is deployed, user corrections can be used to adapt the network parameters to the new data distribution, mitigating distribution shift. Based on these insights, we aim to develop a practical, effective method for improving the adaptive capabilities of interactive segmentation models to new data distributions in medical imaging.  </p>
    </div>
</div>

Firstly, we found that strengthening the model's responsiveness to clicks is important for the initial training process. Moreover, we show that by treating the post-interaction user-refined model output as pseudo-ground-truth, we can design a lean, practical online adaptation method that enables a model to learn effectively across sequential test images. The framework includes two components: (i) a Post-Interaction adaptation process, updating the model after the user has completed interactive refinement of an image, and (ii) a Mid-Interaction adaptation process, updating incrementally after each click. Both processes include a Click-Centered Gaussian loss that strengthens the model's reaction to clicks and enhances focus on user-guided, clinically relevant regions. Experiments on 5 fundus and 4 brain‑MRI databases show that our approach consistently outperforms existing methods under diverse distribution shifts, including unseen imaging modalities and pathologies. 
