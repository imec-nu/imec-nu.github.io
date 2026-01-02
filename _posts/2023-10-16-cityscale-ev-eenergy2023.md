---
title: '"A Data-Driven and Human-Centric EV Charging Recommendation System at City-Scale" Accepted and Presented at ACM e-Energy 2023'
author: imec
group: recent
image: images/news/eenergy2023_presentation.jpeg
---

{%
  include figure.html
  image="images/news/eenergy2023_presentation.jpeg"
%}

["A Data-Driven and Human-Centric EV Charging Recommendation System at City-Scale"](https://dl.acm.org/doi/abs/10.1145/3575813.3597350) was accepted and presented at the 14th ACM International Conference on Future Energy Systems ([e-Energy 2023](https://energy.acm.org/conferences/eenergy/2023/)), co-located with [FCRC 2023](https://fcrc.acm.org/). Congrats team!

In this paper, we present a practical, data-driven, and human-centric EV charging recommendation system at the city-scale based on deep reinforcement learning (DRL). The system co-optimizes the welfare of both the EV drivers and the grid. We augmented and aggregated data from various sources, including public data, location-based data companies, and government authorities, with different formats and time granularities. The data includes EV charger information, grid capacity, EV driving behavior information, and city-scale mobility. We created a 30-day per-minute unified EV charger information dataset with charging prices and grid capacity, as well as an EV driving behavior dataset with location and State of Charge (SoC) information. Our evaluation of the recommendation system shows that it is able to provide recommendations that reduce the average driver-to-charger distance and minimize the number of times chargers switch to a different driver.

We constructed an EV driving-charging-dataset containing 61,392 valid trips in Nov. 2022 and [open-sourced the dataset](https://github.com/Columbia-ICSL/Data-Driven-Human-Centric-EV-Charging) to facilitate the research in this area.
