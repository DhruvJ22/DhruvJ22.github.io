---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: false
---

{% include base_path %}

These projects were done as part of courses at Purdue University, or through my passion to learn more about topics related to astrodynamics, numerical methods, and software engineering.
<br>
<br>

# _Poliastro_
<hr style="border:2px solid grey">

**Description** (from the development team): [Poliastro](https://docs.poliastro.space/en/stable/) is an open-source Python library for interactive Astrodynamics and Orbital Mechanics, with a focus on ease of use, speed, and quick visualization. It provides a simple and intuitive API and handles physical quantities with units.

**Contribution**: I had wished to contribute a part of my Master’s research code to the software to expand its use from the two-body problem to the three-body problem. I wrote programs to simulate the Circular Restricted Three Boby Problem and algorithms to compute its equilibrium and periodic solutions. 

**Current Status (9th January 2023)**: The functionalities that I intended to be added to a new release of the software can be found [here](https://github.com/poliastro/poliastro/tree/main/contrib/cr3bp_DhruvJ). A part of the code has been added to the source code ([1](https://github.com/poliastro/poliastro/tree/main/src/poliastro/threebody), [2](https://github.com/poliastro/poliastro/tree/main/src/poliastro/constants), [3](https://github.com/poliastro/poliastro/tree/main/src/poliastro/core/threebody), [4](https://github.com/poliastro/poliastro/tree/main/src/poliastro)). Due to the organizational changes in the core development team, the updates have been delayed.  

**Learnings**: The most important thing I learned was the importance of separating “the science” and data structures to access the functions that describe the science. This also enabled me to build unit tests for the low-level functions, which simulate the science, to validate them against values in the literature or a property. In addition, I gained experience contributing to open-source software, which has helped me realize how to create meaningful pull requests and about various CI/CD tools to maintain the integrity of the code. 

**Technologies used**: Python, Github, Linux, Command Line Interface

**Concepts learned**: Dynamics Modeling and Targeting desired Dynamical Structures, Open Source Software, CI/CD Tools, Unit Tests
<br>
<br>

# _Numerical Methods_
<hr style="border:2px solid grey">

**Description**: The project involved understanding and implementing various Numerical Methods algorithms: root-finding algorithms, linear equation solvers, numerical interpolation, numerical integration, finite differentiation, partial differential equation solvers, and numerical continuation. 

**Learnings**: The project enabled me to learn about algorithms essential in modeling and analyzing dynamical systems, or any behavior that can be described through mathematical equations. 

**Technologies used**: Python (numpy, matplotlib), Jupyter Lab, Github

**Concepts learned**: Numerical Methods, Analysis and Comparison of algorithms

The code and more detailed discussion can be found on [DhruvJ22/Numerical-Methods](https://github.com/DhruvJ22/Numerical-Methods).
<br>
<br>

# _Analysis of Motor Misalignment, Jet-Damping, and Mass variation on a Spinning-Thrusting Cubesat_
<hr style="border:2px solid grey">

**Description**: The evolution of the attitude of a satellite can be understood by making multiple simplifying assumptions but those assumptions are not valid for a CubeSat. This study analyzes the attitude of a Spinning-Thrusting CubeSat with realistic challenges, such as mass variation and motor misalignment. The attitude is simulated using numerical integration of Euler’s equations of motion and an analytical solution. 

**Learnings**: I gained experience with modeling and simulating the attitude of a CubeSat for a more realistic scenario than usually considered in a graduate-level course. In addition, I realized the importance of identifying an analytical solution. Furthermore, I improved my understanding of numerical simulation results and how to compare numerical simulation results and analytical solutions.

**Technologies used**: MATLAB, Latex, Github

**Concepts learned**: Dynamics Modelling, Analysis of Numerical Simulation Results, Attitude Dynamics, Comparison of Numerical Simulation Results and Analytical Solutions

The code and more detailed discussion can be found on [DhruvJ22/ADCS_course_project](https://github.com/DhruvJ22/ADCS_course_project).

<!-- 
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %} 
-->

