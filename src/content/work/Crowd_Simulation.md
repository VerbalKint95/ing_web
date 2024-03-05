---
title: Crowd Simulation
publishDate: 2023-02-27 00:00:00
img: /assets/evacuation_simulation.gif
img_alt: simulation of a crowd evacuating a room with one exit and one obstacle
description: |
  Implemented a crowd simulation using a granular model for my preparatory project (TIPE). The simulation, developed in Python, replicates crowd behavior during evacuation scenarios.
tags:
  - Simulation
  - Dev
  - Physic
  - Python
---

## Overview

> "Tell me and I forget. Teach me and I remember. Involve me and I learn."

Implemented a crowd simulation project using Python, emphasizing granular physics modeling to simulate crowd behavior during evacuation scenarios. The project delved into the granular approach, modeling individuals as particles subject to various forces, including attraction towards the exit and repulsion from obstacles and other individuals.

### Modeling Forces and Interactions

##### Exit Attraction Force
To model the force pushing individuals towards the exit, iso-time lines were calculated using the Fast Marching Method algorithm. This approach allowed for the determination of the desired direction for each individual.

![room with a lot of obstacle and iso-(time to the exit) lines](/assets/iso-timeToExit_line.png)

##### Social Repulsion Force
For inter-individual interaction forcesI use the Helbing's model. Which is an exponential decay function was utilized, where the force decreases exponentially with distance between individuals.

![equations of Helbing's force](/assets/helbing.png)

### Technologies Used

The project was developed using Python, leveraging the <a href="https://github.com/scikit-fmm/scikit-fmm">scikit-fmm</a> library for the Fast Marching Method implementation. The choice of Python facilitated flexibility and ease of implementation, allowing for comprehensive modeling of crowd dynamics.

### Key Features

- Realistic simulation of crowd behavior during evacuation scenarios.
- Granular physics modeling for detailed analysis of individual movements and interactions.
- Implementation of Fast Marching Method algorithm for computing iso-time lines towards the exit.
- Exponential force interactions between individuals based on distance.

### Acknowledgment of Fluid Dynamics Approach

While the project specifically focused on the granular approach, it acknowledges the alternative fluid dynamics approach. The choice to explore the granular model was driven by its suitability for detailed individual-level analysis. Future developments could potentially explore the fluid dynamics approach for different perspectives on crowd simulation.

### Insights and Learnings

The project provided valuable insights into crowd dynamics and evacuation strategies. By simulating various scenarios, including obstacles and different crowd densities, it facilitated the development of more effective emergency evacuation plans.

#### Future Developments

Future developments may include refining the model to incorporate additional parameters, such as individual characteristics and environmental factors. Additionally, expanding the scope of simulated scenarios to cover a broader range of emergency situations could further enhance the project's utility and impact.

---