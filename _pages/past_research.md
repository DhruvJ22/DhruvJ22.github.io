---
layout: archive
title: "Past Research"
permalink: /past_research/
author_profile: false
---

{% include base_path %}

These are the research projects that I pursued as an independent study with a faculty member. 
<br>
<br>

# _Space Object Taxonomy_
_May 2018 - Feburary 2020_, __Prof. Carolin Frueh, Purdue University__


**Description**: The multi-semester-long research was geared towards identifying patterns in the Geosynchronous Orbit (GEO) space objects. The patterns enabled in designing a program to autonomously classify new space objects into a taxonomy based on the 8 groups defined in the ESA [GEO Classification Report](http://www.astronomer.ru/data/0128/ESA_GEO_Classification_Report_issue_19.pdf).

**Learnings**: I learned the fundamentals of Astrodynamics to understand the orbits that the space objects were in. I used TLE data and the SGP4 model to simulate the orbits, and created functions to compute orbital elements and longitude. I developed an intuition of the orbital characteristics of the GEO objects and insights into the challenges of the space debris problem.

**Technologies used**: Python, MATLAB, Latex, CelsTrak database

**Concept learned**: Space Object Characterization, TLE, SGP4 

A report detailing part of the work can be found [here]({{site.baseurl }}/files/paper1.pdf). 

<hr style="border:2px solid grey">
<hr style="border:1px solid grey">
# _Aerodynamics Deorbit Experiement_
************************************
_January 2019 - May 2019_, __Prof. David Spencer, Purdue University__


**Description**: A CubeSat was being developed to characterize the use of a deployable drag sail as a passive deorbit mechanism through a multi-university partnership. More information about the project can be found [here](https://engineering.purdue.edu/CubeSat/missions/ade)

**Contribution**: I was tasked with orbit modeling the CubeSat to estimate the deorbit time and ground station contact time using Freeflyer, STK, and MATLAB. I performed a Monte-Carlo analysis to account for a range of initial RAAN and launch Epochs. In addition, the coefficient of drag and solar radiation pressure area were modeled as time-variant for a range of values. Furthermore, I assisted in the development of a function in C to interface flight software with an IMU using Raspberry Pi and Linux. 

**Learnings**: I learned about the intricacies of orbit modeling with multiple variables and the development of a complicated mission. I gained experience with identifying the level of fidelity needed to model the orbit and CubeSat, and how to defend design choices. In addition, I realized on a very high level how the flight software was designed for the mission and how to remotely collaborate with partner universities. 

**Technologies used**: Freeflyer, STK, MATLAB, C, Linux, Raspberry Pi

**Concepts learned**: Orbit Modeling, Monte-Carlo Analysis, Contact Analysis,Technical Communication

A rerport summarizing the mission, and various design analysis and decisions can be found [here]({{site.baseurl }}/files/paper1.pdf). 


<!-- 
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %} 
-->

