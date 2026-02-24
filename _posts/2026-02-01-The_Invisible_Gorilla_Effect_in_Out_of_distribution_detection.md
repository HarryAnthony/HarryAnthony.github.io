---
layout: post
title: "The Invisible Gorilla Effect in Out-of-distribution Detection"
place: CVPR 2026
authors: Harry Anthony, Ziyun Liang, Hermione Warr & Konstantinos Kamnitsas
date:   2026-02-01 12:00:00 +0200
image: /images/Invisible_gorilla.png
categories: out-of-distribution-detection
paper: https://arxiv.org/pdf/2602.20068v1
arxiv:
code: 
poster:
presentation:
comments:
year: 2026
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
        <img src="/images/Invisible_Gorilla.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2> Abstract </h2>
        <p> Deep Neural Networks achieve high performance in vision tasks by learning features from regions of interest (ROI) within images, but their performance degrades when deployed on out-of-distribution (OOD) data that differs from training data. This challenge has led to OOD detection methods that aim to identify and reject unreliable predictions. Although prior work shows that OOD detection performance varies by artefact type, the underlying causes remain underexplored. To this end, we identify a previously unreported bias in OOD detection: for hard-to-detect artefacts (near-OOD), detection performance typically improves when the artefact shares visual similarity (e.g. colour) with the model's ROI and drops when it does not - a phenomenon we term the Invisible Gorilla Effect.  </p>
    </div>
</div>

For example, in a skin lesion classifier with red lesion ROI, we show the method Mahalanobis Score achieves a 31.5% higher AUROC when detecting OOD red ink (similar to ROI) compared to black ink (dissimilar) annotations. We annotated artefacts by colour in 11,355 images from three public datasets (e.g. ISIC) and generated colour-swapped counterfactuals to rule out dataset bias. We then evaluated 40 OOD methods across 7 benchmarks and found significant performance drops for most methods when artefacts differed from the ROI. Our findings highlight an overlooked failure mode in OOD detection and provide guidance for more robust detectors.
