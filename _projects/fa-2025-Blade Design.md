---
layout: project
title: Small Wind Turbine Blade Design
description: Aerodynamic Design, Structural Analysis, and Experimental Testing
technologies: [MATLAB, Autodesk Fusion 360, Wind Tunnel Testing]
image: /assets/images/wind-turbine-blade.jpeg
---


As part of MAE 4272: Fluids and Heat Transfer Laboratory at Cornell University, our team designed, fabricated, and experimentally tested a small-scale wind turbine blade. The objective was to maximize power output under fixed wind-tunnel operating conditions while ensuring structural safety under overspeed (free-spin) scenarios. This project mirrors real-world engineering challenges where aerodynamic performance must be balanced against material limits and system constraints.

The blade design was governed by strict constraints, including a 6-inch blade length, 1-inch hub radius**, maximum allowable speed of 2000 RPM, 55 MPa material strength limit, and limitations imposed by the torque-brake testing system. These constraints required careful iteration to achieve reliable and safe performance.

---

## Design Process

We developed a MATLAB-based blade element and structural stress model to guide the design. The blade was discretized into radial elements, and local aerodynamic forces were computed using quasi-steady lift and drag formulations. These forces were integrated to calculate aerodynamic torque** and **root bending stress, the most critical failure location for rotating blades.

Design iterations focused on modifying the chord and twist distributions, particularly in the outer 40% of the blade span where aerodynamic loading and bending stresses are most significant. The model solved for the free-spin overspeed condition by finding the rotational speed at which net aerodynamic torque equals zero, allowing us to evaluate worst-case structural loading.

Once a geometry satisfied both aerodynamic performance and structural safety requirements, the optimized design was translated into Autodesk Fusion 360. MATLAB-generated chord and twist data were imported, NACA 4412 airfoil sections were scaled and aligned using a quarter-chord reference, and smooth guide rails were used to generate a manufacturable solid blade suitable for 3D printing.

---

## Testing Summary

The blades were tested in a closed-loop wind tunnel across four operating frequencies (8–11 Hz), corresponding to wind speeds of approximately 4.6–6.3 m/s**. For each condition, torque-brake voltage was increased incrementally until stall while recording RPM, torque, and electrical power output.

Performance was evaluated using power vs. RPM curves**. The blade consistently produced power across all test conditions, achieving a peak experimental output of 1.33 W at 1664 RPM at the highest wind speed. Across all tests, the average peak power was 0.712 W at approximately 1557 RPM, demonstrating strong agreement with theoretical trends.

Testing also revealed important system-level limitations, including torque-brake resolution and RPM safety constraints, which influenced achievable performance at higher wind speeds.

---

## My Contribution

I focused on the development and refinement of the MATLAB blade element and structural stress model, contributing to geometry iteration, overspeed stress evaluation, and comparison of theoretical predictions with experimental results. I also assisted with wind-tunnel testing and post-processing of experimental data.

---

## Figures

<div class="figure-block">

![Root Bending Stress vs. Wind Speed]({{ "/assets/images/Figure1.blade.design.png" | relative_url }})

<p class="figure-caption">
<strong>Figure 1.</strong> Root bending stress versus wind speed comparing baseline and optimized blade designs.
</p>

</div>

<div class="figure-block">

![Chord and Twist Distributions]({{ "/assets/images/Figure2.blade.design.png" | relative_url }})

<p class="figure-caption">
<strong>Figure 2.</strong> Tuned chord and twist distributions along the blade radius.
</p>

</div>

<div class="figure-block">

![Final CAD Model]({{ "/assets/images/Figure3.blade.design.png" | relative_url }})

<p class="figure-caption">
<strong>Figure 3.</strong> Final manufacturable blade geometry generated in Autodesk Fusion 360.
</p>

</div>

<div class="figure-block">

![Experimental Power Curves]({{ "/assets/images/Figure4.blade.design.png" | relative_url }})

<p class="figure-caption">
<strong>Figure 4.</strong> Experimental power output across 8–11 Hz operating conditions.
</p>

</div>


---

This project reinforced the importance of integrating aerodynamic modeling, structural analysis, and experimental validation while accounting for real-world testing limitations—an approach directly applicable to quality, test, and mechanical engineering roles.
