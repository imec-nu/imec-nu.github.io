---
title: Building Energy Footprinting
---

# Building Energy Footprinting

While buildings are becoming smarter with increasing number of energy monitoring endpoints, the real-time effect of an occupant’s personal actions on the overall energy consumption of the building is still unclear. We are exploring a number of avenues towards increasing awareness of personal energy consumption at the building and city scale.

The first part of this project is personal energy footprinting in commercial buildings. By building on top of existing indoor localization and building energy monitoring techniques, we propose a system that tracks each individual’s energy usage in a shared environment, and provides visibility into his or her real-time energy footprint.

Our most recent work attempts to extend personal energy footprinting to the city scale. We utilize open source city-wide datasets provided by the city of New York to estimate the energy consumption and population of buildings in the city. Using this information, we are able to estimate the personal energy footprint for a citizen in any location in Manhattan.

{% include section.html %}

## ePrints: Personal Energy Footprinting

In this first part of the project, we propose a system that enables accountability of energy usage in commercial buildings, and provides actionable feedback, as well as historical insights for both occupants and building managers, so that they can act accordingly in a timely manner. The system goes beyond traditional disaggregation or monitoring solutions by providing real-time footprint of the users which helps them understand the energy impact of their actions. As per our knowledge, we are the first to develop and implement such a system that is capable of providing actionable feedback in terms of real-time usage footprints for every user under a energy network across different levels of disaggregation – types of loads, location, person, time.

### Project Website and Media

{% include button.html type="website" text="ePrints Project Website" link="http://icsl.ee.columbia.edu/buildingEnergy/" %}

{% include button.html type="app" text="iOS" link="https://itunes.apple.com/us/app/icsl-energy/id1209898397?mt=8" %} {% include button.html type="app" text="Android" link="https://play.google.com/store/apps/details?id=edu.columbia.icsl.androidmobile&hl=en" %}

### Implementation

{%
  include figure.html
  image="images/project/systemArchitecture_eprints.png"
  caption="System and implementation architecture."
%}

We implemented the system as 5 coupled subsystems each of which designed to take care of specific actions. The Energy Reporting subsystem involves controlling and managing all deployed sensors, plug monitors and smart devices to retrieve all energy actions efficiently, and polling data from the building’s internal building management system (BMS) through the BACNET interface. The Query subsystem takes care of all database and data-structure functions which includes storing data and retriving it for various visualization platforms. The occupant tracking system localizes each occupant based on Wi-Fi fingerprinting and Bluetooth Beacon based localization methods. The energy usage of a user is aggregated based on his location (which room he is at and what are the various devices he is using within the room/building). The database system is an implementation of a custom tripartite graph data structure to handle all related operations with an optimized trade-off between performance and storage space.  The foot printing service is the central service which takes care of coupling all other subsystems and managing the interactions between them.

Another major contribution of our implementation is the development of an Interoperability Adaptor which we call the Interoperability Standardization Adaptor which abstracts all complexity associated with the disparate technology and brands of sensors and commercially available smart devices and monitors. This allows the system to interface with a wide variety of existing smart devices or monitors with limited applications without sacrificing on functionalities.

The implementation was done using Microsoft Azure, Python scripts and various other APIs. We also developed custom sensing nodes on Particle Photon and used existing smart technologies such as Samsung Smart Hub, Aeon Labs Plug load meters, Keen Home smart vents, Cree smart bulbs and other commercially available solutions.

A test system was deployed in our laboratory building and successfully evaluated. We also built web-based visualization platforms in Javascript, and mobile device applications for iOS and Android.

{% include section.html %}

## CityEnergy: City-Scale Energy Footprinting

{%
  include figure.html
  image="images/project/titleFigure2-1.png"
  caption="Example of a personal energy footprint in NYC."
%}

In urban cities such as New York City, buildings are responsible for up to 75% of total greenhouse gas emissions, and over 90% of total benchmarked energy consumption. A significant portion of the energy consumed directly services humans in retail, commercial, and residential buildings. As sustainability increasingly becomes an important factor in modern society, energy consumption in the built environment is one area where reduction can have a major impact.

However, many areas of the built environment do not have the capabilities to measure personal energy consumption, much less notify people of their personal energy responsibility. Most notably, there is a lack of energy and population data with high temporal and spatial granularity. Without sensors to measure this data, or models to estimate this data, energy footprinting is not possible.

CityEnergy is a scalable, real-time system for computing personal energy footprint estimates. As shown in the figure, CityEnergy estimates the energy consumption and population for each building in real-time; these estimates are used to calculate the per capita energy footprint at the building level. CityEnergy is able to provide personal energy footprints to people who provide their location data through a mobile application.

{% include button.html type="website" text="CityEnergy Project Website" link="http://icsl.ee.columbia.edu/cityEnergy/" %}

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: energyfootprint_cu" %}

