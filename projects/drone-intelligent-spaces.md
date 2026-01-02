---
title: Reconfigurable Drones and AI for Autonomous Homes, Spaces, and Environments
---

# Reconfigurable Drones and AI for Autonomous Homes, Spaces, and Environments

{%
  include figure.html
  image="images/project/image-5.png"
%}

The increasing prevalence of smart home hubs, sensors, and actuators is enabling greater convenience and automation within our built environments. Moreover, the advent of large language models (LLM) and foundation models (FM) seem poised to transform our environments even further, due to their human-like capacity in understanding language and sensor data. However, it is difficult to directly connect this digital intelligence to the physical world due to a lack of support in existing built environments. For example, a hungry person may receive food suggestions from their smart speaker but still needs to retrieve the food themselves.

In this line of work, we explore two ideas in this line of work. 1) First, is the concept that our future buildings, homes, and offices can dynamically discover and leverage heterogeneous compute and sensing as devices get added, removed, or moved throughout the environment. 

{%
  include figure.html
  image="images/project/flexifly/teaser.png"
  caption="Drones enables LLMs and FMs to 'zoom in' to any location in the environment, providing the opportunity of fine-grained sensing and actuation anywhere compared to traditional static smart sensors and devices."
%}

2) The second concept is the vision that one of the future devices co-existing with us in our environments will be small reconfigurable drones and robots that can act has hands that LLMs and FMs can control to interface with our environments. For example, a drone can sense any point within the environment, essentially "zooming in" to specific locations (shown above), or bring an item from one point to another due to its mobility.

{%
  include figure.html
  image="images/project/flexifly/drone_system_v2.png"
  caption="Modular drone platform that can reconfigure automatically reconfigure its own sensing and actuation depending on the task at hand."
%}

We create a modular and reconfigurable drone platform, shown above, that allows LLMs and FMs to dynamically choose modalities to sense or perform actuation depending on the task at hand. For example, the LLM agent can attach a compartment filled with snacks that it can then fly to a person requesting something to eat.

## Publications

{% include list.html data="citations" component="citation" style="rich" filter="group == 'homeai_cu'" %}

