---
title: Drone-based Airflow Sensing without Sensors
---

# Drone-based Airflow Sensing without Sensors

{%
  include figure.html
  image="images/project/teaser_airflow.png"
  caption="Illustration of mapping of 3D airflow fields."
%}

Mapping 3D airflow fields is important for many HVAC, industrial, medical, and home applications. However, current approaches are expensive and time-consuming. We present Anemoi, a sub-$100 drone-based system for autonomously mapping 3D airflow fields in indoor environments. Anemoi leverages the effects of airflow on motor control signals to estimate the magnitude and direction of wind at any given point in space. We introduce an exploration algorithm for selecting optimal waypoints that minimize overall airflow estimation uncertainty.

{%
  include figure.html
  image="images/project/airflow_sensorless_data.png"
  caption="3D visualization of motor control signals and intermediate projections for estimating airflows."
%}

To estimate airflows without directly leveraging any onboard sensors, we take advantage of a drone's stabilization mechanism or control loop. Whenever wind perturbs the drone, the drone needs to change how fast it spins each motor to maintain stability, depending on how the direction and speed of the wind. Using data-driven methods, we learn a model/mapping of motor signals to the wind speed and direction.

{%
  include figure.html
  image="images/project/airflow-architecture-v2-1.png"
  caption="System architecture, including airflow sensing and information-theoretic exploration."
%}

After sampling the airflow at a specific location, the drone uses a novel information-theoretic approach to select the next location to sample. This proposed approach selects the location that has the most uncertainty based on past measurements, while minimizing cost (time and battery required to move to the new location).

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: airflow_cu" %}

