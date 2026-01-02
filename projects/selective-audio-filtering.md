---
title: Selective and Adaptive Audio Filtering for Mobile, Embedded, and Cyber-Physical Systems
---

# Selective and Adaptive Audio Filtering for Mobile, Embedded, and Cyber-Physical Systems

There are many acoustic applications that would benefit from a platform that allows users and developers to select which sounds to keep and enhance and sounds/noises to remove and filter out. Such a platform is difficult to realize because of the large number of different sounds, models, and signal representations that developers may use in their applications. For example, an audio safety platform that utilizes audio to detect and localize vehicles may benefit from an architecture that filters out urban noises (e.g., construction or speech) and improves the detection of vehicles. Another example is a mobile sleep monitoring system that detects and analyzes breathing sounds. However, when the microphone is on, it can easily detect and record privacy sensitive speech. An application in audio privacy would ideally remove speech while preserving the breathing sounds.

{% include section.html %}

## AvA System Architecture

{%
  include figure.html
  image="images/project/system_architecture.png"
  caption="System architecture."
%}

We introduce, AvA, an acoustic selective filtering architecture that intelligently integrates the physics of sound waves with a wide range of data-driven models in an adaptive feedback architecture to filter and enhance sounds depending on the application.

{% include section.html %}

## Content-Informed Beamforming (CIBF) Process Flow

{%
  include figure.html
  image="images/project/cibf_adaptation.png"
  caption="CIBF architecture and data flow."
%}

AvA allows developers to select sounds they want to enhance or filter out using a novel filter algorithm called content-informed beamforming (CIBF), which combines multi-channel (spatial) filtering methods with data-driven machine learning models that developers may themselves have developed for their applications. CIBF uses a novel three-step process that allows AvA to incorporate almost any type of sound model or machine learning detector to use during the optimization process to learn optimal weights to enhance or filter out specified sounds.

{% include section.html %}

## Applications

{%
  include figure.html
  image="images/project/ava_applications.png"
  caption="Applications of AvA including safety, privacy, cities, health."
%}

We incorporate AvA into a wide range of real systems and applications in health, safety, and privacy to demonstrate its utility.

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: ava_cu" %}

