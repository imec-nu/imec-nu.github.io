---
title: '"Unsupervised Deep Clustering for Human Behavior Understanding" Accepted and Presented at ACM HumanSys 2025'
author: imec
group: recent
image: images/project/c-pter_t-sne-1.png
---

{%
  include figure.html
  image="images/project/c-pter_overview-1.png"
%}

Our paper, ["Unsupervised Deep Clustering for Human Behavior Understanding"](https://dl.acm.org/doi/abs/10.1145/3722570.3726885) has been accepted for publication in [ACM HumanSys 2025](https://humansys-workshop.github.io/WS/2025/index.html), co-located with [CPS-IoT Week 2025](https://cps-iot-week2025.ics.uci.edu/)!

In this work, we propose Compressed-Pseudo-Temporal Enhanced Representation Learning (C-PTER), a novel unsupervised clustering framework for human-centered behavior analysis (architecture shown above). With the growing prevalence of wearables, smartphones, and IoT devices, vast amounts of human activity data are collected in real-world settings, yet traditional supervised learning approaches require extensive manual labeling, making them impractical for large-scale deployment. Existing deep clustering methods, such as autoencoder-based approaches, often fail to capture temporal dependencies and struggle with noisy sensor readings, leading to suboptimal clustering performance.

{%
  include figure.html
  image="images/project/c-pter_t-sne-1.png"
%}

C-PTER proposes a pseudo-temporal feature extractor with a parallel CNN-LSTM autoencoder to enable robust spatial-temporal representation learning. We demonstrate up to 30% improvement in normalized mutual information and 21% improvement in downstream task performance on a variety of human activity datasets, compared with existing state-of-art clustering methods.

Congratulations to Weisi Yang and the rest of the team!

