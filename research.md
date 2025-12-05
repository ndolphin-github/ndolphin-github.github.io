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

### 1.  (NPE - Most Recent)
This research focuses on enabling real-time, high-fidelity simulation of contact mechanics for robotic manipulation. Standard rigid-body simulators use simplified contact models that fail to capture the complex deformation of soft sensors, while numerical solvers are too slow for online interaction.

will be submittedd
**Main Takeaway Video:**
<video width="100%" controls>
  <source src="/Videos/Topic4NPE.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Methods:**
A Neural Physics Engine is developed using a geometry-aware Graph Neural Network. This network is trained on the high-fidelity dataset generated in the previous topic to predict full-field nodal deformations based on sparse contact primitives provided by a rigid-body simulator. The model acts as a fast proxy solver that injects soft-body physics into a rigid simulation loop.

**Results**
Takeaway The Neural Physics Engine achieves sub-millimeter accuracy in predicting deformation and runs significantly faster than traditional finite element solvers, enabling real-time simulation of contact-rich tasks. This capability allows for the zero-shot transfer of manipulation policies, such as peg-in-hole insertion, from simulation to the real world.

**Links:**
- [Code](https://github.com/ndolphin-github/VisionTactileSim_Mujoco)
- [Paper] Expected Submission: Dec 2025

---

### 2. Soft Robot Control & Simulation Framework (AIS Journal)
Implementation of high-fidelity simulation and surrogate models for soft robot control using physics-based learning.

**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/Topic2_result.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


**Technologies:**
- SOFA Framework
- FEM simulation
- Neural network integration
- Sim2Real transfer learning

**Links:**
- 🔗 [GitHub Repository](https://github.com/ndolphin-github/Sim2Real_framework_SoftRobot)
- 📄 [AIS Journal Paper](/Publications/HongTH_AIS_2025.pdf)

---

### 3. DIGIT Sensor & Tactile Simulation (Humanoids Conference)
Development of advanced tactile sensors using DIGIT technology for enhanced robotic manipulation and object recognition.

**Demo Video:**
<video width="100%" controls>
  <source src="/Videos/topic2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Key Features:**
- High-resolution tactile imaging
- Real-time contact detection
- Integration with robotic systems
- Physics-based simulation framework

**Links:**
- 🔗 [GitHub Repository](https://github.com/ndolphin-github/tactile-simulation)
- 📄 [Humanoids Conference Paper](/Publications/HongTH_Humanoids_2025.pdf)

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
