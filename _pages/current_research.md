---
layout: archive
title: "Current Research"
permalink: /current_research/
author_profile: false
sidebar:
  title: "Current Research"
  nav: current_res_sidebar
---
{% include base_path %}
_(This page might take a few seconds to load. Thank you for your patience!)_

# _Introduction_
<hr style="border:2px solid grey">

My current research is focused on designing transfer trajectories between periodic orbits by leveraging quasi-periodic orbits and their manifolds in the cislunar space. 

The trajectory and orbit design in a multi-body gravitational system is a challenging task due to chaotic dynamics and numerical complexities. However, certain assumptions can be made to aid in the description and analysis of the dynamics of a spacecraft for preliminary design, which enables the realization of dynamical structures that can then be utilized to systematically design desired trajectories and orbits. I have used the Circular Restricted Three Body Problem (CR3BP) to model the dynamics of a spacecraft under the influence of the Earth and the Moon. 

CR3BP is a hamiltonian system, so the dynamical systems theory is leveraged to obtain fundamental solutions and their manifolds to characterize the global dynamics. The three types of fundamental solutions are the equilibrium, periodic and quasi-periodic solutions. My focus is on the applications of the quasi-periodic solutions that exist as families of quasi-periodic orbits (QPOs) in CR3BP. The Lagrange points, which are the equilibrium solutions, and periodic orbit families play a crucial role in computing QPOs and realizing their benefits. 
<br>
<br>

# _Lagrange Points and Periodic Orbits_
<hr style="border:2px solid grey">

The Lagrange points are trivial to compute and there exist five of them in any system in the CR3BP model, namely L1, L2, L3, L4, and L5. Periodic and quasi-periodic orbits can be computed around the points to enable space exploration, economy, and surveillance. Periodic Orbits have a key characteristic, as their name suggests, that a spacecraft in orbit returns to its initial state after a finite period. The computation of periodic orbits is challenging due to the chaotic dynamics and lack of a useful analytical solution. Thus, [numerical methods](https://github.com/DhruvJ22/Numerical-Methods) are used to obtain families of orbits and orbits with desired characteristics. A part of my research code can be found [here](https://github.com/DhruvJ22/Astrodynamics_Research), which can be used to compute the Lagrange points and the periodic orbit families. 

NASA [CAPSTONE](https://www.nasa.gov/directorates/spacetech/small_spacecraft/capstone/) and [ARTEMIS 1](https://www.nasa.gov/image-feature/artemis-i-map) mission leveraged a L2 Halo and a DRO orbit in the Earth-Moon system respectively. The _L2 Halo orbit family_(left) and _DRO family_(right), whose members were utilized for the two missions, are plotted below using my publicly available [code](https://github.com/DhruvJ22/Astrodynamics_Research) and the family members are colored by Jacobi Constant. 

<figure class="half">
    <figcaption>These are interactive plots</figcaption>
    <iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://dhruvj22.github.io/Astrodynamics_Research/EM_L2_HaloS_family.html" height="450" width="50%"></iframe>
    <iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://dhruvj22.github.io/Astrodynamics_Research//misc/EM_DRO_family.html" height="450" width="50%"></iframe>
</figure>
The periodic orbits have various applications, as exemplified by the above two NASA missions, and are essential in identifying quasi-periodic orbits. 
<br>
<br>

# _QPOs and their Applications_
<hr style="border:2px solid grey">

Quasi-periodic orbits are a higher dimensional solutions than periodic orbits of the CR3BP. A spacecraft in the orbit is bounded to a surface of quasi-periodic solutions but it does not return to a previously traversed state. The orbits are non-trivial to compute because of the dynamical and numerical complexities. Nonetheless, with the recent improvements in our understanding of the dynamics and computational power, it is feasible to compute the orbit families and leverage them in mission design. The below animation depicts how a spacecraft(red) traverses a QPO (blue surface) and its 2D projections: 

![DJ Animation]({{ site.baseurl }}/files/em_l1_quasilyap_JC_3_01_projections.mp4

The computation of QPO involves using multiple shooting with multiple nodes to target the quasi-periodic behavior and then utilizing a numerical continuation scheme to compute three different families of QPOs. Despite their complexities, they fundamentally expand the solution space, which makes them an attractive choice to host spacecrafts, formation flying, and transfer design. I have worked on recreating some of the applications and I have been able to come up with a novel application that uses their manifolds, which will be described in my upcoming MS thesis. 
<br>

## 1. Host Orbit

[James Webb Space Telescope (JWST)](https://webb.nasa.gov/) is the most recent example of a mission that uses a QPO as a host orbit. The telescope is hosted in a [Sun-Earth L2 Quasi-Halo orbit](https://jwst-docs.stsci.edu/jwst-observatory-characteristics/jwst-orbit). I was able to recreate the orbit(green) and how the trajectory (grey) of the telescope(red point on orbit) evolves using the CR3BP model as shown below

![image-center]({{ site.baseurl }}/files/jwst_10revs.gif){: .align-center}
<br>

## 2. Maneuver Free Transfers

Maneuver free transfers, also known as heteroclinic transfers, between QPOs can be computed by leveraging their manifolds. The same is not guaranteed for periodic orbits because of their lower dimensionality than QPOs. The construction of these types of transfers relies on identifying a good initial guess, which was done by using a Poincare map and k-d tree, and differential correction. The following interactive plot shows 2 maneuver-free trajectories (yellow and green) that can be used to travel from a L2-Quasi Halo orbit (red) to get to a L1 Quasi-Halo Orbit (blue), JC = 3.13.

<figure>
    <figcaption>This is an interactive plot</figcaption>
    <iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://dhruvj22.github.io/Astrodynamics_Research//misc/EM_L2qHalo_L1qHalo_JC_3_13_heteroclinc2tramsfers.html" height="550" width="100%"></iframe>
</figure>

## 3. Transfers between QPOs and Periodic Orbits

The existence and method to compute QPOs have been known since the 20th century and they have been leveraged in a previous [NASA mission](https://solarsystem.nasa.gov/missions/artemis/in-depth/). However, it is only recently that engineers have developed algorithms to compute QPOs and their manfiolds of desired characteristics to enable the use of QPOs directly for mission design. My work builds on these developments and purposes a few improvements to the cutting-edge algorithms to more efficiently compute transfer trajectories between QPOs and periodic orbits. The procedure to compute these types of transfers is similar to that for maneuver-free transfers with the addition of an optimization scheme to obtain locally fuel optimal transfers. The below plot depicts a fuel-efficient transfer trajectory from a L2 Quasi-Halo Orbit to a DRO. 

![image-center2]({{ site.baseurl }}/files/EM_l2qHalo_to_DRO.png){: .align-center}

There are many planned missions that will leverage periodic orbits but it is a constant challenge to compute fuel-efficient transfers between them. Thus, I am working on finding these transfers more efficiently by expanding my work to chain periodic orbit - QPO and QPO - periodic orbit transfer to get a periodic orbit - periodic orbit transfer. You can learn more about them in my upcoming thesis. 

Technologies used: Python(numpy, scipy, pandas, scikit-learn, plotly, matplotlib), MATLAB, C, Git, Command Line Interface, Latex

Concepts learned: Dynamics Modelling, Numerical Methods, Optimization,  Data Analysis, Data Visualization, Technical Communication, Automation, Software Development, Independent and Creative Work