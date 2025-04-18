# Micro Small Intelligent Jumping Robot

Project details can be found in [notion link](https://cherry-room-163.notion.site/?pvs=4)

## Project Overview

This project, developed at the University of Electronic Science and Technology of China (UESTC), focuses on creating a micro-sized intelligent jumping robot. Unlike many biomimetic designs, this robot utilizes engineering principles and a carbon fiber structure to achieve significantly higher jump heights, potentially exceeding 5 meters. The goal is to develop a robot capable of navigating complex terrains with potential applications in reconnaissance and defense.

## Key Features & Components

*   **High-Performance Jumping:** Employs carbon fiber legs for efficient energy storage and release, enabling high jumps.
*   **Engineering-Based Design:** Focuses on mechanical principles rather than direct biological imitation for maximizing jump height.
*   **Motor-Driven Actuation:** Uses a [`GA12-N20`](assets/GA12-N20.SLDPRT) DC geared motor (6V, 50r/min, 298:1 ratio) to wind a rope, compressing the carbon fiber legs for energy storage.
*   **Mechanical Latch Release:** A custom [`latch`](assets/latch.SLDPRT) and release arm system ([`releasing arm2.SLDPRT`](assets/releasing arm2.SLDPRT), [`releasing arm3.SLDPRT`](assets/releasing arm3.SLDPRT)) triggered by a [`楔形.SLDPRT`](assets/楔形.SLDPRT) (wedge) on the rope provides a rapid release mechanism.
*   **Power Source:** Utilizes a compact 7.4V, 180mAh LiPo [`电池.SLDPRT`](assets/电池.SLDPRT) (battery).
*   **Lightweight Construction:** Incorporates carbon fiber and other lightweight materials. CAD models for components are available in the [`assets/`](assets/) directory, including the main [`组装体.SLDASM`](assets/组装体.SLDASM) (assembly).

## Jumping Mechanism

1.  The motor rotates, winding a rope attached to the carbon fiber legs via a [`拉绳板.SLDPRT`](assets/拉绳板.SLDPRT) (rope plate).
2.  The legs bend, storing elastic potential energy.
3.  A wedge fixed to the rope moves upwards as it's wound.
4.  The wedge contacts and pushes open the latch mechanism.
5.  The release arm, no longer supported by the latch, swings down due to rope tension.
6.  The rope rapidly unwinds from the motor shaft, releasing the tension on the legs.
7.  The carbon fiber legs snap back to their original shape, converting stored potential energy into kinetic energy, launching the robot upwards.
8.  Elastic bands reset the release arm for the next jump cycle.

## Current Status

*   A physical prototype has been constructed and tested.
*   Achieved an estimated jump height of approximately 5 meters.
*   The time interval between jumps is around 10 seconds.
*   Demonstrated partial capability for repetitive jumping.

## Future Work & Planned Improvements

*   Develop and implement control systems for jump direction and aerial attitude stabilization (potentially using IMU, GPS).
*   Enhance the reliability and reduce potential jamming of the release mechanism.
*   Address potential delamination issues with the carbon fiber legs after repeated stress cycles.
*   Integrate control components (microcontroller, sensors, wireless communication like Bluetooth).
*   Implement obstacle avoidance capabilities.
*   Refine the overall mechanical structure and component interactions.

## Team & Advisor

*   **Team Members:** Gou Xuning, Cao Zhihan, Cui Chenguang, Tan Peijie
*   **Advisor:** Wei Dunwen
*   **Institution:** University of Electronic Science and Technology of China (UESTC)

## Assets

The [`assets/`](assets/) directory contains SolidWorks CAD files (`.SLDPRT` for parts, `.SLDASM` for assembly) detailing the robot's mechanical design.