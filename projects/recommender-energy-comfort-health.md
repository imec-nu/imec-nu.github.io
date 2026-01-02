---
title: Recommender Systems for Optimizing Energy, Comfort, and Health
---

# Recommender Systems for Optimizing Energy, Comfort, and Health

Recent research efforts have made significant progress in reducing commercial building energy consumption through a variety of methods, including optimizing building heating, ventilation, and air conditioning (HVAC), lighting, and personal electric devices. However, these works focus on reducing energy consuming resources while treating occupants as immovable objects separate from the building energy optimization problem. Moreover, energy is not the only important objective in commercial buildings; maintaining occupant comfort and health is also crucial to improving wellness and productivity.

{% include section.html %}

## RecEnergy: An Energy Saving Recommender System

{%
  include figure.html
  image="images/project/recEnergyWatch_IoTJ-1024x1024.png"
  caption="A user receives a recommendation to move to a different lab space to reduce energy."
%}

First, we developed recEnergy, a recommender system for reducing energy consumption in commercial buildings with human-in-the-loop. We formulate the building energy optimization problem as a Markov Decision Process, show how deep reinforcement learning can be used to learn energy saving recommendations, and effectively engage occupants in energy-saving actions. Example actions, include shifting your schedule to be more in line with others so that the building can reduce HVAC service during off-peak hours, or nudging people to share spaces so that the building can reduce HVAC service to more rooms.

{% include section.html %}

## RECA: A Multi-Task Deep Reinforcement Learning-Based Recommender System for Co-Optimizing Energy, Comfort and Air Quality in Commercial Buildings

{%
  include figure.html
  image="images/project/RECA_DeepQNetworkSetpoint.png"
  caption="Multi-task deep Q-network architecture for generating human-in-the-loop recommendations to co-optimize energy, comfort, and health."
%}

Next, we develop RECA, a recommender system that expands the capabilities of recEnergy to co-optimize air quality and occupant comfort in addition to energy consumption. RECA leverages multi-task deep reinforcement learning to efficiently optimize these objectives, while giving building managers flexibility to configure the system (e.g., setting the system to prioritize occupant health over energy savings). For example, recommending occupants to share a space may allow the building to reduce service to other rooms, thus saving energy; however, a single space may not be able to accommodate the thermal preferences of multiple people, which reduces overall occupant comfort.

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: energyrec_cu" %}

