---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /research
---

## Ongoing Projects:

### Shared Control with Learned Environment Perception during Bilateral Robotic Teleoperation
*University of Sussex*

This work is focused on a teleoperated contact-rich robotic manipulation scenario in an unknown environment. In this research work, a shared control framework is designed for exerting a variable desired force on a surface during a continuous contact task. Utilising the NRP-ILC (see previous work) for autonomous force tracking and a novel online environment estimation method, this framework will mitigate the issues of communication delay by introducing impedance perception as feedback to the human operator. This concept has been successfully implemented in a teleoperation system with a Kinova Gen3 7DOF robot as the follower and a TouchX haptic device as the leader. In this system, implemented using ROS 2, the experiments demonstrated that this proposed method can help human operators to perform continuous force tracking tasks with improved stability and transparency. This work has been submitted to the International Journal of Robotics Research (IJRR) and is currently under review.

## Previous Projects:

### Force-dependent Variable Impedance Control (FVIC) 
*University of Sussex - 2025*

In this work, I developed a position-based variable impedance controller that updates the impedance parameters (stiffness and damping) of a robot based on contact force. When learning unknown environments through contact-rich manipulation, unsafe levels of contact forces are a common problem. The current approaches for this include variable impedance methods with virtual energy tanks to ensure stability. However, such methods compromise the desired contact dynamics. In this novel VIC method, the stiffness and damping are updated as functions of contact force while maintaining stability. The simulations in the MATLAB environment and experiments performed with the Kinova Gen3 robot integrated with two external 6-axis force/torque sensors using the Kinova Kortex API based on C++ show that this method is successful in maintaining safe interactions in unknown environments and ensuring correct position tracking in known environments. 

[This work has been published in IEEE Control System Letters (Special section on: Safety, Robustness, and Effectiveness in Human-Machine Teaming)](/publication/2025_LCSS_FVIC).

<img src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/images/FVIC_simulations.jpg" alt="FVIC Simulations" width="50%"/>
<!-- ![FVIC Simulations](https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/images/FVIC_simulations.jpg "FVIC Simulations") -->


### Non-repetitive-path Iterative Learning Control (NRP-ILC)
*University of Sussex - 2024*

This is a learning and control method stemming from iterative learning control based on the absolute x-y position of a surface. This is an extension of my previous work on MILC. In this work, a collaborative manipulator robot (cobot) is programmed to traverse repetitively through virtual sub-regions of an unknown surface while trying to achieve a desired contact force amidst occasional interruption from the human operator. When the robot visits each sub-region during different iterations, the previous information collected at each sub-region will be used to update the reference position and impedance information of the surface for the next iteration. In the previous work (MILC), the robot needed to visit all the sub-regions during each iteration to ensure proper learning and control. However, in this NRP-ILC, the robot can use any random path while arbitrarily missing some sub-regions, yet still achieving the required control performance. Through this work, I further established the NRP-ILC method as a framework that can be used for achieving multiple control objectives, such as force tracking, orientation adaptation, and impedance learning. I validated this framework via simulations on MATLAB. I also tested it on a Kinova Gen3 robot integrated with two external 6-axis force/torque sensors using the Kinova Kortex API based on C++. This work has been accepted for publication by IEEE Transactions on Robotics.

[This work has been published in IEEE Transactions on Robotics.](/publication/2025_TRO_NRP-ILC)

  <video width="568" height="320" controls loop="" muted="" autoplay="">
  <source src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/videos/NRP-ILC_Demo.mp4">
</video>

### Design of Robotic Manipulators for Nuclear Decommissioning
*University of Sussex, University of Tokyo - 2022-2024*

This was a part of the EPSRC project *[A Nuclear Decommissioning Manipulator with Novel Variable Impedance Actuator](https://ukerc.rl.ac.uk/cgi-bin/ercri5.pl?GChoose=gregsum&GRN=EP/W016168/1&GrantRegion=7&GrantOrg=250&HTC=50101D2C&SHTC=1B84A95;)* (EP/W016168/1), a collaboration between the University of Sussex and the University of Tokyo. Two robotic manipulators were designed for use-case scenarios at Sellafield and Fukushima nuclear power plants, respectively. These manipulators were designed to be integrated with a novel continuously variable transmission system (CVT). The addition of CVT increased the strength requirement of the manipulator, which required a thorough compromise between the weight and strength of components. I carried out initial CAD-based designs of the Fukushima manipulator and detailed designs of the Sellafield manipulator. The design and optimisation of structural components through FEA, bearing selection, bolt calculations, gear calculations, shaft design, keyway design, and coupling selection were among the design tasks that I did. I further developed extensive design drawings that considered the design for manufacture and assembly requirements. Additionally, I was responsible for procuring standard components and commissioning component manufacturing.

<video width="568" height="320" controls loop="" muted="" autoplay="">
  <source src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/videos/Manipulators.mp4">
</video>

Additionally, we have conducted a CVT characterisation on a test bench to evaluate the collision-safe capabilities of this project. We carried out initial tests using a combination of an Arduino Portenta board and Maxon motor controllers as DAQs and Controllers to assess the variation in speed transmission ratio. The test-bench controllers currently incorporate the input data from motor encoders, a torque sensor, and magnetic encoders to record output shaft velocity. Output signals include motor output, brake control signals, and pneumatic pressure regulators.


### Mesh Iterative Learning Control (MILC)
*University of Sussex - 2023*

This is a learning and control method stemming from iterative learning control based on the absolute x-y position of a surface. In this method, a collaborative manipulator robot (cobot) is programmed to repetitively traverse through virtual sub-regions of an unknown surface while trying to achieve a desired contact force. When the robot visits each sub-region during different iterations, the previous information collected at each sub-region will be used to update the reference position and impedance information of the surface for the next iteration. This method differs from the traditional iterative learning control methods, as it does not require the robot to repeat the same path with the same process time. I simulated this controller in the MATLAB environment. Experiments were performed on the Sawyer robot arm to validate the method. 

[This work was presented in the 2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS).](/publication/2023_IROS_MILC)


  <video width="568" height="320" controls loop="" muted="" autoplay="">
  <source src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/videos/MILC_demo.mp4">
</video>

### Literature Review on Wearable Devices for Load-Handling Activities
*University of Moratuwa, University of Sussex - 2023*

A scoping review on load-handling wearable devices (i.e., exoskeletons) focusing on the devices published from 2010 onwards. I, in collaboration with a few other researchers from the University of Moratuwa (Sri Lanka), performed this extensive review by analysing the classification of wearable devices based on application, targeted joint, mechanical design, etc. This also features a PRISMA analysis along with a bibliometric analysis of all the related literature during the duration considered. I further researched and discussed biomechanics related to load-handling activities in this article. 

[This review was published in IEEE Access.](/publication/2023_Access_ExoReview)

### Multi-Objective Optimization-based Assist-as-Needed Controller for Improved Quality of Assistance in Rehabilitation Robotics
*University of Sussex - 2023*

*This project was a part of the interdisciplinary project “5G-enabled robotic teleoperation system for remote physical therapy: a post-COVID recovery approach in health care” by researchers from the University of Sussex; funded by Higher Education Innovation Funding - HEIF*

A reference-free control method was developed for an upper-limb rehabilitation robotic device from HumanRobotiX (HRX-1) concerning wrist flexion/extension. In this control method, the control signal was optimised based on the state of the patient’s hand while ensuring the motions were carried out within pre-defined constraints. This system incorporates position, velocity, and tremor constraints to allow the patient to engage in remote physiotherapy within their capabilities. I simulated this controller in the MATLAB environment for validation. This project included a PPIE (public and patient involvement and engagement) element where the user requirements were identified through discussions and engagements with a stroke survivor, a family carer, an NHS physician, and a physiotherapist. 

[This work was presented at the 2023 International Conference on Rehabilitation Robotics (ICORR) held in Singapore.](/publication/2023_ICORR_MOO)

[Link to poster](https://www.researchgate.net/publication/374413308_Multi-Objective_Optimization-based_Assist-as-needed_Controller_for_Improved_Quality_of_Assistance_in_Rehabilitation_Robotics)

### Literature Review on Circular External Fixators 
*University of Moratuwa, Imperial College London, QMUL - 2022*

A review on the circular external fixators, an orthopaedic device that is mainly used to stabilise complex bone structures, based on a PRISMA analysis performed on all the available research on the topic. As most reviews are focused on the clinical aspects of these devices, I focused this review on the engineering design aspects of available devices. This work also features an extensive discussion of the history and the evolution of the device, along with a bibliometric analysis.

[The review was published in Injury (an Elsevier journal).](/publication/2023_Injury_CEF)

### Design of a Low-Cost Wire Clamp for Ilizarov Ring Fixators
*University of Moratuwa, Imperial College London, QMUL - 2021*

*A part of collaborative research by the University of Moratuwa and Imperial College London: Funded by [NIHR PrOTeCT Grant](https://www.imperial.ac.uk/trauma-bioengineering/nihr-protect-grant/)*

We designed and optimised a low-cost wire clamp for Ilizarov Ring Fixators (an orthopaedic device that is mainly used for stabilising complex fractures). We collaborated with an orthopaedic surgeon to understand and address the user requirements. We visited the operating theatre of a national hospital in Sri Lanka during an orthopaedic surgery to understand the fixator application process in action. Design for manufacturability was specifically considered when designing the clamp with the intention of cost reduction. I used Ansys Workbench to perform static structural analysis on the proposed clamp. I identified and optimised several geometric parameters using the response surface optimisation method, focusing on ‘avoiding wire slippage in the clamp’, ‘reduction of clamp mass’, and ‘ensuring no failure under the applied forces’. The finite element analysis showed that the final design can avoid wire slippage while maintaining a mass of 125.73 g without failure. 

This was presented as a poster at the Blast Injury Conference 2021. Furthermore, [a research feature](/publication/2022_Bolgoda_CEF) is published on this work in the Bolgoda Plains research magazine, published by the University of Moratuwa. We have also applied for a patent for this wire clamp.

[Link to poster](https://www.researchgate.net/publication/353046589_Design_of_a_Low-cost_Wire_Clamp_for_Ilizarov_Ring_Fixators)

### TRoPHy: Transtibial Robotic Prosthesis with Hybrid Powering Mechanism
*University of Moratuwa - 2019*

*This was my undergraduate final year project (group of 3)*

A lightweight ankle robotic prosthesis that uses both passive and active actuation to generate ankle motion was developed. The power requirement of the prosthesis was reduced by recovering energy using a spring system. As the team leader, I studied anatomy and biomechanics related to the ankle-foot complex and derived the design parameters. In addition to that, I designed the control system of the device. An event-triggered control system was used to feed pre-defined time-varying speed patterns to the motor. Event detection was done by Force Sensitive Resistors with a defined threshold. Published data plots from the literature were digitised using “Web Plot Digitizer” software and then acquired respective polynomials using MATLAB Curve-Fitting to develop the speed variation pattern. MATLAB Simulink was used to simulate the models, and then they were used in developing an Arduino control model for the system. 

[This work was presented at the Moratuwa Engineering Research Conference (MERCon).](/publication/2019_MERCon_TRoPHy)

  <video width="320" height="240" controls loop="" muted="" autoplay="">
  <source src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/videos/TRoPHy.mp4">
</video>
  <video width="320" height="240" controls loop="yes" muted="" autoplay="yes">
  <source src="https://github.com/KithmiNDWidanage/KithmiNDWidanage.github.io/raw/refs/heads/master/videos/TRoPHy_sim.mp4">
</video>
