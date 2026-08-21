# Selected Projects

My work spans robotic modeling, control, hardware experimentation, and learning. I am particularly interested in problems where robots must physically interact with uncertain environments.

---

## Contact-Rich Anchoring for Snake Robots

**Modeling · Optimization · Robot Control · Force/Torque Sensing · Hardware Experiments**

<div style="border: 2px dashed #b8b8b8; border-radius: 8px; padding: 40px 20px; margin: 20px 0; text-align: center; color: #777;">
<strong>MAIN VIDEO / GIF SLOT</strong><br>
Snake robot anchoring experiment<br>
<code>static/assets/img/snake_anchor_demo.gif</code>
</div>

### Overview

My current research focuses on **contact-rich anchoring for snake robots**. The goal is to understand how a snake robot can use multiple environmental contacts to form a stable anchor and resist external loading.

Rather than treating anchoring only as a predefined robot configuration, I am interested in the underlying physical problem: **how robot geometry, joint actuation, contact forces, friction, and external loading jointly determine anchoring performance.**

My work covers the full process from physical problem formulation to analytical modeling, robot control, experimental system development, and data analysis.

### What I Work On

- Develop a simplified rigid-body model of the anchoring configuration.
- Formulate static force and moment equilibrium for multiple environmental contacts.
- Model normal and tangential contact forces under friction constraints.
- Formulate the underdetermined contact-force distribution as an optimization problem.
- Study how robot geometry and commanded joint torque affect contact-force distribution.
- Control a physical ReU snake robot to reproduce anchoring configurations.
- Integrate multiple force/torque sensors for contact-force measurement.
- Develop synchronized acquisition of robot torque and force measurements.
- Design and assemble experimental hardware for controlled external loading.
- Compare analytical predictions with measurements from the physical system.

### From Physical Problem to Experiment

**Anchoring Requirement**

Stable interaction with the environment under external loading.

↓

**Analytical Representation**

Rigid-body geometry, multiple contacts, friction, force equilibrium, and moment equilibrium.

↓

**Optimization**

Estimate feasible contact-force distributions for an underdetermined system.

↓

**Robot Control**

Generate and reproduce physical anchoring configurations using joint actuation.

↓

**Hardware Experiment**

Measure contact forces, joint torque, robot geometry, and external loading.

↓

**Analysis**

Investigate how well the analytical model captures trends observed on the real robot.

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 25px 0;">

<div style="flex: 1; min-width: 280px; border: 2px dashed #b8b8b8; border-radius: 8px; padding: 35px 15px; text-align: center; color: #777;">
<strong>FIGURE SLOT 1</strong><br>
Analytical / contact model<br>
<code>snake_model.png</code>
</div>

<div style="flex: 1; min-width: 280px; border: 2px dashed #b8b8b8; border-radius: 8px; padding: 35px 15px; text-align: center; color: #777;">
<strong>FIGURE SLOT 2</strong><br>
Experimental setup<br>
<code>snake_experiment_setup.jpg</code>
</div>

</div>

### Why This Problem Is Difficult

Snake robot anchoring involves several characteristics that make the problem difficult to model and control:

- **Multiple simultaneous contacts** with the environment.
- **Underdetermined contact forces**, where equilibrium equations alone do not uniquely determine the force distribution.
- **Friction-dependent interaction** at each contact.
- **Changing geometry**, which changes both contact conditions and effective moment arms.
- **Physical uncertainty**, including compliance, sensor noise, contact variation, and differences between an idealized rigid-body model and the real system.

These issues make the project useful not only as an anchoring problem, but also as a platform for studying more general **contact-rich robotic interaction**.

### Experimental System

The physical platform combines:

- a multi-module ReU snake robot,
- multiple force/torque sensors,
- joint torque feedback,
- custom mechanical fixtures,
- an external loading mechanism,
- synchronized force and robot-state data acquisition.

<div style="border: 2px dashed #b8b8b8; border-radius: 8px; padding: 40px 20px; margin: 20px 0; text-align: center; color: #777;">
<strong>VIDEO SLOT</strong><br>
Full experimental trial / external loading test<br>
<code>snake_full_trial.mp4</code>
</div>

### Analysis

A major part of the current work is comparing changes predicted by the analytical model with trends measured on the physical robot.

Quantities of interest include:

- normal contact forces,
- tangential / shear forces,
- commanded and measured joint torque,
- robot configuration,
- contact geometry,
- external loading,
- anchoring stability.

<div style="border: 2px dashed #b8b8b8; border-radius: 8px; padding: 40px 20px; margin: 20px 0; text-align: center; color: #777;">
<strong>RESULT PLOT SLOT</strong><br>
Predicted vs. measured force trends<br>
<code>snake_force_results.png</code>
</div>

### Current Limitation & Next Direction

The current analytical formulation relies on simplified rigid-body and contact assumptions. This makes the model useful for understanding the mechanics of anchoring, but limits its ability to generalize across more complex geometries and uncertain contact conditions.

This limitation motivates my broader interest in **combining analytical structure with learning-based approaches for contact-rich robotics**.

I am particularly interested in how model-based knowledge, physical constraints, and experimental data can be used together to develop robotic systems that adapt more effectively to changing environments.

---

## Lower-Limb Exoskeleton

**Mechanical Design · Embedded Control · Actuator Integration · System Integration**

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 20px 0;">

<div style="flex: 1; min-width: 280px; border: 2px dashed #b8b8b8; border-radius: 8px; padding: 35px 15px; text-align: center; color: #777;">
<strong>IMAGE SLOT</strong><br>
Exoskeleton prototype / assembly<br>
<code>exoskeleton_system.jpg</code>
</div>

<div style="flex: 1; min-width: 280px; border: 2px dashed #b8b8b8; border-radius: 8px; padding: 35px 15px; text-align: center; color: #777;">
<strong>IMAGE / GIF SLOT</strong><br>
Actuator or motor-control demonstration<br>
<code>exoskeleton_actuator.gif</code>
</div>

</div>

### Overview

During a robotics internship, I worked on the development and integration of an exoskeleton system. My work covered several layers of the robotic system, from mechanical structure and actuator assembly to embedded motor-level control.

This experience gave me practical exposure to the challenges that appear when mechanical design, electronics, actuation, and control must operate together on a physical robot.

### My Work

- Redesigned and assembled mechanical structures for a lower-limb exoskeleton.
- Integrated and debugged actuator modules.
- Implemented motor-level control using an STM32 platform.
- Participated in control-related implementation and system testing.
- Worked on prototype integration and practical mechatronic debugging.
- Contributed to mechanical design for an upper-limb exoskeleton.

### What I Learned

This project strengthened my understanding of robotics as a complete physical system:

**Mechanical Structure → Actuation → Embedded Control → Robot Behavior**

It also gave me experience debugging problems that cannot be isolated to a single software or mechanical component, which continues to influence how I approach robotic system development.

---

## Cross-Platform Human Activity Recognition

**Machine Learning · Dataset Development · Generalization · Evaluation**

<div style="border: 2px dashed #b8b8b8; border-radius: 8px; padding: 40px 20px; margin: 20px 0; text-align: center; color: #777;">
<strong>RESULT / PIPELINE FIGURE SLOT</strong><br>
Model pipeline, dataset, or evaluation results<br>
<code>har_results.png</code>
</div>

### Overview

This team project studied the **generalization of human activity recognition models across different sensing platforms**, such as smartphones and smartwatches.

The project provided experience with a more data-driven workflow and complements my work on physical robotic systems.

### My Work

- Evaluated open-source human activity recognition models.
- Designed experiments to compare model generalization across sensing platforms.
- Collected and prepared data for training and evaluation.
- Trained and validated the selected model.
- Analyzed model performance across different experimental conditions.
- Explored potential approaches for improving generalization.

### Project Focus

The main question was not only whether a model could achieve good performance on one dataset, but whether its learned representation could remain useful when the sensing platform changed.

This project helped me develop experience with:

**Dataset → Training → Evaluation → Generalization Analysis**

[View Project on GitHub](https://github.com/Wilheimbeta/CMU-24696-WearableHealthTechnology-Programming)

---

## What Connects These Projects?

Although these projects use different robotic and computational systems, they reflect the same way I like to approach engineering problems:

**Understand the physical problem → build a useful representation → develop a solution → test it on real data or hardware → identify where the current method fails → improve the next iteration.**

My current goal is to continue developing this approach toward **robot control and learning for contact-rich physical interaction**.
