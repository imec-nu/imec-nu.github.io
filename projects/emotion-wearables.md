---
title: Wearables for Emotion Sensing
---

# Wearables for Emotion Sensing

{%
  include figure.html
  image="images/project/spiders_and_manikin.png"
  caption="Left: SPIDERS glasses platform (red: hardware sensors; blue: PCB boards; green optional attachments). Right: SPIDERS glasses on a mannequin."
%}

Monitoring the emotional well-being of a person is important in many domains, such as health monitoring, elderly care, depression treatment, entertainment, so on and so forth. We present SPIDERS which is a low-cost, wireless, glasses-based platform for continuous in-situ monitoring of user’s facial expressions and real emotions. SPIDERS costs less than $20 to assemble and can continuously run for up to 9 hours before recharging.

{%
  include figure.html
  image="images/project/Architecture_spiders.png"
  caption="Four-layer system architecture block diagram."
%}


SPIDERS has a four-layer system architecture. Each layer in the architecture directly enables the applications or functionalities in the layer directly above. We present algorithms to provide four core functions (eye shape and eyebrow movements, pupillometry, zygomaticus muscle movements, and head movements). The algorithms use the bio-signals acquired from three non-contact sensors (infrared camera, proximity sensor, an inertial measuring unit). SPIDERS can be also extended to include functionalities provided by contact-based sensors, such as heart rate sensors and 8-channel EEG sensors.

{% include section.html %}

## Core Function Library

We present novel and robust vision-based techniques to perform pupillometry as well as eye & eyebrow shape detection using IR-band gray-scale images, from an IR camera positioned at a low angle from the eye as to not block the field of view of the user. A proximity sensor is used to detect the movements of zygomaticus muscle (smile muscle), which aims at adding another dimension of knowledge to the facial expression.

{% include section.html %}

## Advanced Functionalities

{%
  include figure.html
  image="images/project/Picture3_spiders.png"
  caption="Eye images of seven common facial expressions. The constraints from the gray-scale image captured by a wearable eye tracker make it difficult to distinguish subtle differences among different emotions (eg. happy and disgusted)."
%}

{%
  include figure.html
  image="images/project/FlowChartLogic_spiders.png"
  caption="The pipeline of eye-image-based facial expression (apparent emotion) detection."
%}

SPIDERS distinguishes between different classes of facial expression and real emotion states based on these four bio-signals. We prototype advanced functionalities, including facial expression detection and real emotion classification. Specifically, we deploy a novel facial expression detector based on landmarks and optical flow that leverages changes in a user’s eyebrows and eye shapes to achieve an accuracy that outperforming the state-of-the-art approach. We also implement a pupillometry-based real emotion classifier with higher accuracy than other low-cost wearable platforms that use sensors requiring skin contact.


{% include section.html %}

## Code and Media

{% include button.html type="presentation" text="IoTDI 2020 Presentation" link="https://youtu.be/NzPlKYPWuKI" %} {% include button.html type="demonstration" text="IPSN 2020 Demo" link="https://www.youtube.com/watch?v=SOX7UIqaQGQ" %}

{% include button.html type="source" text="Code" link="https://github.com/Columbia-ICSL/SPIDERS" %}

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: spiders_cu" %}

