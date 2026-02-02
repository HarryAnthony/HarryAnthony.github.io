---
layout: post
title: "Specialised or generic? Tokenisation choices for radiology language models"
place: ELAMI at MICCAI 2025
authors: Hermione Warr, Wentian Xu, Harry Anthony, Yasin Ibrahim, Daniel R McGowan & Konstantinos Kamnitsas
date:   2025-09-01 12:00:00 +0200
image: /images/LLM_Tokenisation.png
categories: out-of-distribution-detection
paper: https://link.springer.com/chapter/10.1007/978-3-032-07502-4_8
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
        <img src="/images/LLM_Tokenisation.png" alt="Image" style="max-width:100%; height:auto;">
    </div>
    <div class="content" style="flex: 1;">
        <h2> Tokenisation choice for Language Models </h2>
        <p> The vocabulary used by language models (LM) - defined by the tokenizer - plays a key role in text generation quality. However, its impact remains under-explored in radiology. In this work, we address this gap by systematically comparing general, medical, and domain-specific tokenizers on the task of radiology report summarisation across three imaging modalities. We also investigate scenarios with and without LM pre-training on PubMed abstracts. Our findings demonstrate that medical and domain-specific vocabularies outperformed widely used natural language alternatives when models are trained from scratch.  </p>
    </div>
</div>

Pre-training partially mitigates performance differences between tokenizers, whilst the domain-specific tokenizers achieve the most favourable results. Domain-specific tokenizers also reduce memory requirements due to smaller vocabularies and shorter sequences. These results demonstrate that adapting the vocabulary of LMs to the clinical domain provides practical benefits, including improved performance and reduced computational demands, making such models more accessible and effective for both research and real-world healthcare settings.

Dive into our research!

<a href="https://link.springer.com/chapter/10.1007/978-3-032-07502-4_8">&#x1F4C4; Paper</a> | <a href="https://github.com/hermionewarr/Scribe">`</>` Code</a>