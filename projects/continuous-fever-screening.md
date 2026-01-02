---
title: Robust, Continuous, and Multi-Person Fever Screening
---

# Robust, Continuous, and Multi-Person Fever Screening

{%
  include figure.html
  image="images/project/sifter_columbiadoctors.png"
  caption="SIFTER deployment at ColumbiaDoctors."
%}

With the recent societal impact of COVID-19, companies and government agencies alike have turned to thermal camera based skin temperature sensing technology to help screen for fever. However, the cost and deployment restrictions limit the wide use of these thermal sensing technologies. In this work, we present SIFTER, a low-cost system based on a RGB-thermal camera for continuous fever screening of multiple people. This system detects and tracks heads in the RGB and thermal domains and constructs thermal heat map models for each tracked person, and classifies people as having or not having fever.

This is a challenging problem because temperature measurements should be robust to conditions that are not in the system’s control. First, skin temperature is largely dependent on the ambient environment. For people who have not yet been acclimated to the indoor environment, temperature measurements will not be consistent. Second, distance from thermal camera can can cause differences in thermal measurements. Third, measurements of a single person may change in the presence of multiple people. Although these conditions can sometimes be controlled through protocols, improving measurement robustness to these conditions brings advantages to the screening efficiency and enforcement of protocol. Fourth, the system needs to select accurate temperature features. There are variations in skin temperature for different regions of the face, meaning that aggregate statistics will change depending on which regions of the face are visible to the thermal camera.

{%
  include figure.html
  image="images/project/3DMapping-1024x644.png"
  caption="3D temperature mapping onto a model of each person’s head."
%}

Rather than rely on aggregate statistics to estimate temperature, we model thermal features by mapping temperatures onto a 3D head model. This enables two important ideas: first, detected thermal features are robust to changes in facial perspective, and second, facial temperature features can be selected directly from the 3D head model, without needing to train a network to specifically target regions of the face.

Additionally, we present a variant gradient boosting method using asymmetric loss functions to target high temperature measurements in this fever screening application to account for low temperature measurements commonly observed from people further away from the camera.

{%
  include figure.html
  image="images/project/SystemArchitecture_sifter.png"
  caption="System architecture."
%}

We designed the system to be low cost, easily deployable, and usable in both low and high throughput settings. SIFTER uses the 399 USD FLIR One Pro with a Jetson Nano, to keep the hardware cost less than 500 USD per unit.

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: fever_cu" %}

