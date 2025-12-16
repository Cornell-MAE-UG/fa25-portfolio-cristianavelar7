---
layout: project
title: Small Wind Turbine Blade Design
description: Aerodynamic Design, Structural Analysis, and Experimental Testing
technologies: [MATLAB, Autodesk Fusion 360, Wind Tunnel Testing]
image: /assets/images/wind-turbine-blade.jpg
---
## Project Overview
As part of **MAE 4272: Fluids and Heat Transfer Laboratory**, our team was tasked with designing, fabricating, and testing a small-scale wind turbine blade capable of maximizing power output under fixed wind-tunnel operating conditions. The project emphasized the integration of aerodynamic theory, structural safety, and experimental validation, mirroring the type of multidisciplinary design process commonly encountered in industry.

The primary goal was to optimize blade geometry to increase power generation while ensuring structural integrity under free-spin (overspeed) conditions. The design was constrained by a 6-inch blade length, 1-inch hub radius, maximum rotational speed of 2000 RPM, a 55 MPa material strength limit, and a torque-brake system with limited resolution. These constraints required careful balancing of aerodynamic efficiency and mechanical reliability.

---

## Design Process

Our design process began with the development of a MATLAB-based blade element and bending-stress model. The blade was discretized into radial elements, and local aerodynamic forces were computed using quasi-steady lift and drag formulations. These forces were integrated to predict both aerodynamic torque and root bending stress, which is the critical failure location for rotating blades.

Key design iterations focused on modifying the chord and twist distributions, particularly in the outer 40% of the blade span, where aerodynamic loading and bending stresses increase significantly with radius. The model solved for the free-spin overspeed condition by finding the rotational speed at which net aerodynamic torque was zero, allowing us to evaluate worst-case structural loading.

Once a geometry was identified that satisfied both performance and stress limits, the optimized blade profile was translated into Autodesk Fusion 360. MATLAB-generated chord and twist data were imported, airfoil sections (NACA 4412) were scaled and aligned using a quarter-chord reference, and smooth guide rails were used to generate a manufacturable solid blade model suitable for 3D printing.

---

## Testing Summary

The fabricated blades were tested in a closed-loop wind tunnel across four wind-tunnel frequencies (8–11 Hz), corresponding to wind speeds of approximately 4.6–6.3 m/s. For each frequency, torque brake voltage was incrementally increased until stall, while RPM, torque, and electrical power output were recorded.

Performance was evaluated by generating power vs. RPM curves for each test condition. The blades consistently produced power across all frequencies, achieving a peak experimental power of 1.33 W at 1664 RPM at the highest test frequency. Across all tests, the average peak power was 0.712 W at approximately 1557 RPM, showing good agreement with theoretical trends predicted by the MATLAB model.

Testing also revealed important system-level limitations. At higher wind speeds, the turbine exhibited rapid acceleration and torque spikes, highlighting the effects of torque-brake resolution and RPM safety limits—factors not fully captured in the simplified aerodynamic model.

---

## My Contribution

I focused primarily on the development and refinement of the MATLAB blade-element and structural model, working to link aerodynamic loading, rotational speed, and root bending stress. I contributed to iterative geometry tuning, overspeed stress evaluation, and comparison of theoretical predictions with experimental power data. I also assisted with experimental testing and data analysis, helping assess discrepancies between modeled and measured performance.

---

## Figures

- **Figure 1:** Baseline vs. tuned free-spin root bending stress as a function of wind speed  
/assets/images/Figure1.blade.design

- **Figure 2:** Optimized chord and twist distributions along the blade radius  
/assets/images/Figure2.blade.design

- **Figure 3:** Final CAD model and blade dimensions  
/assets/images/Figure3.blade.design

- **Figure 4:** Superimposed experimental power curves for 8–11 Hz wind-tunnel tests  
/assets/images/Figure4.blade.design

---
## Conclusion

This project strengthened my understanding of how aerodynamic design decisions, structural limits, and test-system constraints interact to determine real-world performance. It reinforced the importance of designing not only for ideal theoretical conditions, but for the practical limitations imposed by manufacturing, materials, and testing hardware.