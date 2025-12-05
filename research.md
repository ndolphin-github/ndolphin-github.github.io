---
layout: page
title: Research
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
- 🔗 [GitHub Repository](https://github.com/ndolphin-github/DIGIT_simulation)
- 📄 [Humanoids Conference Paper](/Publications/HongTH_Humanoids_2025.pdf)

--

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
- 🔗 [GitHub Repository](https://github.com/ndolphin-github/Sim2Real_framework_SoftRobot)
- 📄 [AIS Journal Paper](/Publications/HongTH_AIS_2025.pdf)

---


---

### 4. Proprioceptive Origami Actuators (IJRR)
Machine learning approaches for model-based control of pneumatic origami actuators for manipulation tasks.



**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/Topic1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Approaches:**
- Model-based control systems
- Proprioceptive sensing
- Pneumatic manipulation
- Real-time processing algorithms

**Links:**
- 🔗 [GitHub Repository](https://github.com/ndolphin-github/origami-control)
- 📄 [IJRR Paper](/Publications/HongTH_IJRR_2025.pdf)

---

## Selected Publications

### Recent Journal Articles (2025)

**"Bridging High‐Fidelity Simulations and Physics‐Based Learning using a Surrogate Model for Soft Robot Control"**  
*Advances in Intelligent Systems (AIS)*  
[[PDF]](/Publications/HongTH_AIS_2025.pdf) [[Code]](https://github.com/ndolphin-github/Sim2Real_framework_SoftRobot)

**"Model-based control of proprioceptive origami actuators for pneumatic manipulation"**  
*International Journal of Robotics Research (IJRR)*  
[[PDF]](/Publications/HongTH_IJRR_2025.pdf)

**"Design of A Fully-Soft Lift-Assist Wearable Suit Powered by Flat Inflatable Artificial Muscles"**  
*IEEE Robotics and Automation Letters (RAL)*  
[[PDF]](/Publications/HongT_IEEE_RAL_2025.pdf)

### Recent Conference Papers (2025)

**"Bidirectional Mapping Between Physical Contacts and Visual Tactile Images for Physics-Based Simulation"**  
*2025 IEEE-RAS 24th International Conference on Humanoid Robots*  
[[PDF]](/Publications/HongTH_Humanoids_2025.pdf)[[Code]](https://github.com/ndolphin-github/DIGIT_simulation)

---

## Contact & Collaborations

**Email:** [ndolphin93@gmail.com]  
**Lab:** [Soft Robotics and Bionics Lab], Seoul National University  
**Google Scholar:** [Your Profile](https://scholar.google.co.kr/citations?hl=ko&user=kzrORlsAAAAJ&view_op=list_works&sortby=pubdate)

For detailed publications list, please visit my [publications page](/publications/) or download my [CV](/Publications/TaehwaHong_CV.pdf).
