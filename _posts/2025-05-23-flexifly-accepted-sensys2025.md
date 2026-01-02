---
title: '"FlexiFly: Interfacing the Physical World with Foundation Models Empowered by Reconfigurable Drone Systems" Accepted and Presented at ACM SenSys 2025'
author: imec
group: recent
image: images/news/05-23-2025/PXL_20250509_211714574-scaled.webp
---

{%
  include figure.html
  image="images/news/05-23-2025/PXL_20250509_211714574-scaled.webp"
%}

Our work, ["FlexiFly: Interfacing the Physical World with Foundation Models Empowered by Reconfigurable Drone Systems"](https://dl.acm.org/doi/10.1145/3715014.3722081), was accepted and presented at [SenSys 2025](https://sensys.acm.org/2025/) during [CPS-IoT Week 2025](https://cps-iot-week2025.ics.uci.edu/). This research was developed through a collaborative effort between Northwestern University and Columbia University, with contributions from Minghui (Scott) Zhao, Junxi Xia, Kaiyuan Hou, Yanchen Liu, and Professor Stephen Xia, Professor Xiaofan (Fred) Jiang.

{%
  include figure.html
  image="images/news/05-23-2025/flexifly_pipeline.webp"
  caption="FlexiFly's operation pipeline"
%}

In this work, we addressed a fundamental challenge in enabling foundation models to interact meaningfully with physical environments. While foundation models excel at digital tasks, they struggle when required to understand localized events in large physical spaces or perform real-world actions. Our contributions are summarized as follows:

**(1) Novel Foundation Model Orchestration Framework:** We introduce a comprehensive framework that integrates multiple large language models, vision-language models, and an open-set object detection model for dynamic, task-driven sensor/actuator selection.

**(2) Advanced Image Segmentation Approach:** We propose a new segmentation method that reliably pinpoints task-relevant areas even in large, cluttered environments, overcoming limitations of existing approaches.

**(3) Custom Reconfigurable Drone Platform:** We present a purpose-built drone system capable of autonomously adapting its sensors and actuators in response to commands from the FM orchestration framework, enabling seamless physical interaction and significantly improving task success rates in real-world deployments compared to static sensor approaches.

FlexiFly enables foundation models to "zoom in" on areas of interest using reconfigurable drones that can automatically swap between different sensing and actuation modules. Through extensive real-world evaluations, our system demonstrated up to 85% improvement in task success rates across diverse applications including object identification, environmental monitoring, surveillance, and physical item delivery.


