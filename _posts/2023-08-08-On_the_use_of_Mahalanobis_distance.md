---
layout: post
title:  "On the use of Mahalanobis distance for out-of-distribution detection with neural networks for medical imaging"
place: UNSURE at MICCAI, Springer, 2023
authors: Harry Anthony & Konstantinos Kamnitsas
date:   2023-08-01 12:00:00 +0200
image: /images/On_the_use_of_Mahalanobis.png
categories: out-of-distribution-detection, outlier-detection
paper: https://arxiv.org/abs/2309.01488
arxiv:
code: https://github.com/HarryAnthony/Mahalanobis-OOD-detection
---

![](/images/On_the_use_of_Mahalanobis.png)


## Abstract

Implementing neural networks for clinical use in medical applications necessitates the ability for the network to detect when input data differs significantly from the training data, with the aim of preventing unreliable predictions. The community has developed several methods for out-of-distribution (OOD) detection, within which distance-based approaches - such as Mahalanobis distance - have shown potential. This paper challenges the prevailing community understanding that there is an optimal layer, or combination of layers, of a neural network for applying Mahalanobis distance for detection of any OOD pattern. Using synthetic artefacts to emulate OOD patterns, this paper shows the optimum layer to apply Mahalanobis distance changes with the type of OOD pattern, showing there is no one-fits-all solution. This paper also shows that separating this OOD detector into multiple detectors at different depths of the network can enhance the robustness for detecting different OOD patterns. These insights were validated on real-world OOD tasks, training models on CheXpert chest X-rays with no support devices, then using scans with unseen pacemakers (we manually labelled 50% of CheXpert for this research) and unseen sex as OOD cases. The results inform best-practices for the use of Mahalanobis distance for OOD detection.