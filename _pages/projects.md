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

# _Senior Spacecraft Design Project, Purdue University_
<hr style="border:2px solid grey">

**Description**: A group of 8 students collaborated to design a space mission to leverage the [Signals of Opportunity](https://ieeexplore.ieee.org/document/8520391) technology to collect the sub-soil moisture data and develop on the success of the [NASA SMAP](https://smap.jpl.nasa.gov/) mission. The project was formulated as a call to a NASA Announcement of Opportunity. The design was focused on the Pre-Phase A development of the mission. The team planned the Science Objectives and Requirements, Science Implementation, Mission Implementation, Cost, and Schedule

**Contribution**: My primary role was to assist the team as a Systems Engineer, so I formulated the Top-Level Requirements, analyzed the Risks, planned Contingencies, mapped the Data and Power flow onboard. In addition, I ideated on Flight Software/Onboard Processing, Development Approach, and Assembly, Integration, Test and Verification. Also, I significantly contributed to planning and budgeting for ADCS, Satellite Constellation Design, and End of Life Disposal. As a Systems Engineer, I also assisted other subsystem teams to be successful by helping them to ideate and keep up with the evolving design. 

**Learnings**: I learned the fundamental principles of Mission Design and the importance of realizing how various satellite subsystems interact with each other. This realization assisted in better supporting the subsystems teams and when to relay the subsystem updates to other teams. Besides the technical knowledge that I gained by working on my specific contributions, I became adept at leading team meetings and collaborating virtually with members of the team spread across 4 different time zones.

**Technologies used**: MATLAB, C, GMAT, Linux, Canva, Slack  
**Concepts learned**: Space Systems Engineering, Mission Formulation, Mission Operations, Satellite Constellation Design, Attitude Determination and Control, Risks and Contengencies

The final report for the project can be found [here]({{site.baseurl }}/files/GAEA_Final_Proposal.pdf).
<br>
<br>

# _Analysis of Motor Misalignment, Jet-Damping, and Mass variation on a Spinning-Thrusting Cubesat_
<hr style="border:2px solid grey">

**Description**: The evolution of the attitude of a satellite can be understood by making multiple simplifying assumptions but those assumptions are not valid for a CubeSat. This study analyzes the attitude of a Spinning-Thrusting CubeSat with realistic challenges, such as mass variation and motor misalignment. The attitude is simulated using numerical integration of Euler’s equations of motion and an analytical solution. 

**Learnings**: I gained experience with modeling and simulating the attitude of a CubeSat for a more realistic scenario than usually considered in a graduate-level course. In addition, I realized the importance of identifying an analytical solution. Furthermore, I improved my understanding of numerical simulation results and how to compare numerical simulation results and analytical solutions.

**Technologies used**: MATLAB, Latex, Github

**Concepts learned**: Dynamics Modelling, Analysis of Numerical Simulation Results, Attitude Dynamics, Comparison of Numerical Simulation Results and Analytical Solutions

The code and more detailed [discussion]({{site.baseurl }}/files/CubeSat_Attitude_Simulator_Report.pdf) can be found on [DhruvJ22/ADCS_course_project](https://github.com/DhruvJ22/ADCS_course_project).
<br>
<br>

# _Purdue Vibrational Instrumental Payload for Educational Research_
<hr style="border:2px solid grey">

**Description**: A team of 5 collaborated for a semester to make progress with the development of a device that is capable of measuring vibrations on a payload of a suborbital rocket flight for educational purposes. 

**Contribution**: I was the lead programmer and I worked with the team to write a program to obtain and process data from an IMU. I had the most experience working with IMUs in the team, so I was chosen to lead the programming effort

**Learning**: I learned the basics of I2P and SPI communication protocol to write a code to read and write data to an IMU and a data logger. In addition, I realized the design decisions made by previous members of the team. I also gained the experience of how to actively participate in a meeting, and lead and collaborate with peers who were much more experienced aerospace students. 

**Technologies used**: Arduino IDE to interface with the embedded systems

**Concepts learned**: I2P and SPI communication protocols, IMU, Data logger

Check out the code and the [project report]({{site.baseurl }}/files/PVIPER_Report_Fall2018.pdf)!

<!-- 
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %} 
-->

