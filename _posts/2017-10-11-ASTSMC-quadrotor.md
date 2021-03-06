---
layout: post
title: Adaptive Super Twisting Sliding Mode Control for a Quadrotor
date: 2017-10-11 00:00:00 +0300
description: A non-linear control methods (sliding mode control) for a quadrotor.
img:  bandicam-2017-10-10-01-58-3.gif # Add image post (optional)
tags: [Control] # add tag
type: project
---

### [Description]
Sliding mode control is a powerful tool to make system more robust. 
This project gives preliminary results applying super twisting sliding mode control to a quadrotor. 
Comparisons between traditional linear PD control and several sliding mode control methods are provided. 
Simulations show that adaptive super twisting sliding mode control achieves good tracking performance and reduces chattering effectively.

---
### [Simulaiton results]

We applied sliding mode (SM) control for a quadrotor, which improve its robustness against disturbances. 
The following figure shows the velocity-vs-time plot of helix trajectory tracking under disturbances in mass and inertia. 
Both SM controllers out-perform PD controller under such uncertainty.

![](https://shaoanlu.files.wordpress.com/2017/10/vel_compare.png)

Futhermore, we introduced an adaptive gain for [super-twisting sliding mode control (STSMC)](http://www.sciencedirect.com/science/article/pii/S2405896316300672), known as [adaptive super-twisting sliding model control (ASTSMC)](https://ieeexplore.ieee.org/document/7487462), to achieve faster convergence and eliminate notorious chattering effect.
The following figure illustrates the control input signals (1 thrust control and 3 moment controls) of helix trajectory tracking under external force disturbances, in which the adaptive method presents less high frequency components and thus better performance.

![](https://shaoanlu.files.wordpress.com/2017/10/compare_inpall_helix_uncert2.png)

---
### [Animation]

**Helix trajectory**

![](https://shaoanlu.files.wordpress.com/2017/10/bandicam-2017-10-09-22-33-2.gif)

**Four points trajectory**

![](https://shaoanlu.files.wordpress.com/2017/10/bandicam-2017-10-10-01-58-3.gif)

**Helix trajectory (ill-tuned controller)**

![](https://shaoanlu.files.wordpress.com/2017/10/ezgif-2-6a8dbc3e03.gif)

##### This project is related to a coursera course titled Aerial Robotics from University of Pennsylvania.
