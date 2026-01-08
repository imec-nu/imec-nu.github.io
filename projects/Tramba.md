---
title: 'TRAMBA: Practical Bone-Conduction / IMU Speech Enhancement'
---

# TRAMBA: Practical Bone-Conduction / IMU Speech Enhancement

{%
  include figure.html
  image="images/project/tramba_fig1_overview.png"
  caption="TRAMBA enhances vibration-based speech (BCM/ACCEL), which is naturally robust to ambient noise but lacks high-frequency components."
%}

TRAMBA is a hybrid Transformer + Mamba model for acoustic and bone-conduction speech super-resolution and enhancement on mobile/wearable platforms. It is designed to be practical: small memory footprint, fast inference, and quick user-specific fine-tuning.

{%
  include figure.html
  image="images/project/tramba_fig2_tradeoff.png"
  caption="Performance vs. efficiency trade-offs compared with state-of-the-art U-Net and GAN baselines (model size, inference time, and fine-tuning time)."
%}

{% include section.html %}

## Architecture

{%
  include figure.html
  image="images/project/tramba_fig4_arch.png"
  caption="TRAMBA architecture: modified U-Net with self-attention in down/up blocks and a Mamba bottleneck for efficient long-range modeling."
%}

Key ideas:
- Hybrid Transformer + Mamba: attention helps generate complex formants; Mamba reduces memory and improves speed.
- Pre-train on widely available OTA audio, then fine-tune with a small amount of paired vibration data.

{% include section.html %}

## System & Prototype

{%
  include figure.html
  image="images/project/tramba_fig7_system.png"
  caption="Data collection locations, environments, and our mobile-TRAMBA prototype."
%}

We integrate TRAMBA into an end-to-end wearable/mobile pipeline to enable real-time enhancement in noisy environments and reduce sensing + transmission costs by allowing lower sampling rates.

{% include section.html %}

## Key Results

{%
  include figure.html
  image="images/project/tramba_fig6_sampling_rate.png"
  caption="Effect of sampling rate on super-resolution quality: TRAMBA remains competitive even at low sampling rates."
%}

{% include section.html %}

## Code and Media

{% include button.html type="paper" text="Paper (IMWUT 2024)" link="https://dl.acm.org/doi/pdf/10.1145/3699757" %}
{% include button.html type="source" text="Code" link="https://github.com/IMEC-Northwestern/TRAMBA" %}
{% include button.html type="demonstration" text="Demo Page" link="https://imec-northwestern.github.io/TRAMBAPage/" %}

{% include section.html %}

## Publications

- **TRAMBA: A Hybrid Transformer and Mamba Architecture for Practical Audio and Bone Conduction Speech Super Resolution and Enhancement on Mobile and Wearable Platforms.**
  *IMWUT 2024.*  
  https://dl.acm.org/doi/10.1145/3699757

