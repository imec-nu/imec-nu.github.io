---
title: Modular and Reconfigurable Sensing Platforms
---

# Modular and Reconfigurable Sensing Platforms

{%
  include figure.html
  image="images/project/teaser_legosense-1.png"
  caption="Overview of strengths and features of LegoSENSE compared to existing platforms."
%}

Domain-specific sensor deployments are critical to enabling various IoT applications. Existing solutions for quickly deploying sensing systems require significant amount of work and time, even for experienced engineers. We propose LegoSENSE, a low-cost open-source and modular platform, built on top of the widely popular Raspberry Pi single-board computer, that makes it simple for anyone, regardless of technical background, to rapidly set up and deploy a customized sensing solution for application specific IoT deployments. We [open-source all designs](https://github.com/Columbia-ICSL/LegoSENSE) to allow developers to easily incorporate new sensors and modules into the ecosystem.

{%
  include figure.html
  image="images/project/hw_overview_v3-legosense.png"
  caption="Hardware architecture."
%}

LegoSENSE can accommodate up to four different modules comes equipped with a standard hardware interface that abstracts out the need for users to understand how to wire and connect sensors; all slots can support common communication protocols, such as analog, GPIO, I2C, and SPI.

{%
  include figure.html
  image="images/project/sw_arch-legosense.png"
  caption="Software architecture."
%}

LegoSENSE leverages software drivers to detect and communicate with sensors on-the-fly. Users can easily configure the sensor (e.g., sampling rate) through an interface that does not require any coding. Additionally, developers can easily add drivers to enable LegoSENSE to support new sensors.

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: legosense_cu" %}

