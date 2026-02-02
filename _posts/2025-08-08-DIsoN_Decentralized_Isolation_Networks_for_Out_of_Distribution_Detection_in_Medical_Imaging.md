---
layout: post
title: "DIsoN: Decentralized Isolation Networks for Out-of-Distribution Detection in Medical Imaging"
place: NeurIPS 2025
authors: Felix Wagner, Harry Anthony, Pramit Saha, J Alison Noble, & Konstantinos Kamnitsas
date:   2025-08-01 12:00:00 +0200
image: /images/DISON.png
categories: out-of-distribution-detection
paper: https://neurips.cc/virtual/2025/loc/san-diego/poster/115312
arxiv:
code: https://github.com/FelixWag/DIsoN/tree/main
poster: /docs/Neurips_2025_poster.png
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
        <img src="/images/DISON.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2> Out-of-distribution detection <br> and Federated Learning </h2>
        <p> Safe deployment of machine learning (ML) models in safety-critical domains such as medical imaging requires detecting inputs with characteristics not seen during training, known as out-of-distribution (OOD) detection, to prevent unreliable predictions. Effective OOD detection after deployment could benefit from access to the training data, enabling direct comparison between test samples and the training data distribution to identify differences. State-of-the-art OOD detection methods, however, either discard the training data after deployment or assume that test samples and training data are centrally stored together, an assumption that rarely holds in real-world settings. This is because shipping the training data with the deployed model is usually impossible due to the size of training databases, as well as proprietary or privacy constraints.  </p>
    </div>
</div>

We introduce the Isolation Network, an OOD detection framework that quantifies the difficulty of separating a target test sample from the training data by solving a binary classification task. We then propose Decentralized Isolation Networks (DIsoN), which enables the comparison of training and test data when data-sharing is impossible, by exchanging only model parameters between the remote computational nodes of training and deployment. We further extend DIsoN with class-conditioning, comparing a target sample solely with training data of its predicted class. We evaluate DIsoN on four medical imaging datasets (dermatology, chest X-ray, breast ultrasound, histopathology) across 12 OOD detection tasks. DIsoN performs favorably against existing methods while respecting data-privacy. This decentralized OOD detection framework opens the way for a new type of service that ML developers could provide along with their models: providing remote, secure utilization of their training data for OOD detection services.

Dive into our research!

<img src="/images/Critical_analysis_OOD/Paper_summary.gif" alt="" />

<a href="https://neurips.cc/virtual/2025/loc/san-diego/poster/115312
">&#x1F4C4; Paper</a> | <a href="/docs/Neurips_2025_poster.pdf">&#x1F4CA; Poster</a> | <a href="https://github.com/FelixWag/DIsoN/tree/main">`</>` Code</a>