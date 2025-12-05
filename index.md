---
layout: default
title: Home
---

## About Me

My research focuses on bridging the reality gap in contact-rich physical interactions by proposing
a unified data-driven abstraction framework. This approach decouples high-fidelity ground truth generation from runtime execution to resolve the fidelity-tractability trade-off.

**Research Interests:**
- Physics-based Simulation
- Soft Robotics & Deformable Body Simulation
- Tactile Sensing 
- Contact Rich Manipulation


## Research Projects

### 1.  Geometry-Aware Neural Physics Engine for Vision Tactile Sensor
This research focuses on enabling real-time, high-fidelity simulation of contact mechanics for robotic manipulation. Standard rigid-body simulators use simplified contact models that fail to capture the complex deformation of soft sensors, while numerical solvers are too slow for online interaction.

will be submittedd
**Main Takeaway Video:**
<video width="100%" controls>
  <source src="/Videos/Topic4NPE.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Methods:**
A Neural Physics Engine is developed using a geometry-aware Graph Neural Network. This network is trained on the high-fidelity dataset generated in the previous topic to predict full-field nodal deformations based on sparse contact primitives provided by a rigid-body simulator. The model acts as a fast proxy solver that injects soft-body physics into a rigid simulation loop.

**Main Takeaway**
Takeaway The Neural Physics Engine achieves sub-millimeter accuracy in predicting deformation and runs significantly faster than traditional finite element solvers, enabling real-time simulation of contact-rich tasks. This capability allows for the zero-shot transfer of manipulation policies, such as peg-in-hole insertion, from simulation to the real world.

**Links:**
- 🔗 [Code](https://github.com/ndolphin-github/VisionTactileSim_Mujoco)
- 📄 [Paper] Expected Submission: Dec 2025

---

### 2. DIGIT Sensor & Tactile Simulation 
This work addresses the data scarcity issue in vision-based tactile sensing, where high-resolution visual data exists but lacks corresponding physical ground truth such as force and deformation fields. Existing simulators often prioritize visual realism over mechanical accuracy, limiting their utility for physically grounded learning.

**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/topic3.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Methods**
A bidirectional data pipeline is established using a finite element model of a sensor that is rigorously calibrated to real-world indentation data. Two neural networks are trained on paired datasets: a perception network that infers dense physical states from real tactile images, and a rendering network that synthesizes photorealistic images from simulated physical states.

**Main Takeaway**
The framework creates a closed loop between the visual and physical domains, enabling the automatic annotation of real-world tactile images with physical data and the generation of large-scale, physically grounded synthetic datasets. This resolves the labeling bottleneck for tactile perception tasks.


**Links:**
- 🔗 [Code](https://github.com/ndolphin-github/DIGIT_simulation)
- 📄 [Paper](/Publications/HongTH_Humanoids_2025.pdf)

---

### 3. Surrogate Model for Soft Robot Dynamics 
This research aims to resolve the trade-off between physical fidelity and computational speed in simulating soft robots for reinforcement learning. High-fidelity finite element method simulations are accurate but too slow for learning, while rigid-body simulators are fast but lack physical realism regarding deformation.

**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/topic2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/Topic2_result.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


**Methods**
The framework employs a data-driven surrogate modeling approach. A high-fidelity simulation is first calibrated to the real robot and then compressed using model order reduction to generate a training dataset. A transformer-based physics-informed neural network is trained to learn the forward dynamics from this data. This learned model is then mapped to a simplified virtual kinematic chain (surrogate) within a fast physics engine, enabling rapid policy training.

**Main Takeaway**
The surrogate model successfully bridges the reality gap, allowing reinforcement learning policies trained in a fast simulation to transfer zero-shot to a physical soft manipulator for trajectory tracking and force control tasks. This method provides a scalable pipeline for training soft robots by decoupling accurate physics generation from runtime execution.

**Links:**
- 🔗 [Code](https://github.com/ndolphin-github/Sim2Real_framework_SoftRobot)
- 📄 [Paper](/Publications/HongTH_AIS_2025.pdf)


---

### 4. Proprioceptive Origami Actuators (IJRR)
This research addresses the challenge of controlling soft manipulators constructed from origami cylinder modules, specifically those utilizing the Yoshimura pattern. While these structures offer lightweight and collapsible properties, their non-linear folding mechanics make traditional modeling computationally expensive and unsuitable for real-time control.


**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/Topic1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Method**
The study derives a simplified kinematic model based on first principles, treating the actuator as a conservative energy system. The method decouples the deformation into axial and bending components, using geometric constraints and potential energy minimization to predict force and moment outputs. To enable real-time execution, these complex analytical relationships are precomputed into lookup tables, allowing the controller to rapidly infer strain and bending angles from pressure inputs and external loads.

**Main Takeaway**
The proposed analytical model facilitates real-time, closed-loop position and force control of a soft manipulator using only embedded proprioceptive sensors, eliminating the need for computationally heavy finite element analysis during operation. However, the reliance on specific geometric patterns limits the generalizability of this approach to arbitrary soft body morphologies.

**Links:**
- 📄 [Paper](/Publications/HongTH_IJRR_2025.pdf)

---

## Contact & Collaborations

**Email:** ndolphin93@gmail.com  
**Lab:** Soft Robotics and Bionics Lab, Seoul National University  
**Google Scholar:** [Your Profile](https://scholar.google.co.kr/citations?hl=ko&user=kzrORlsAAAAJ&view_op=list_works&sortby=pubdate)

For detailed publications list, please visit my [publications page](/publications/) or download my [CV](/Publications/Taehwa%20Hong%20CV.pdf).