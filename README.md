# Vehicle Suspension Robust Control

A repository containing the master’s thesis on robust control strategies for an 8 Degrees of Freedom (DOF) active vehicle suspension system, focusing on ride quality, road handling, and robustness against uncertainties, delays, and faults.

## Overview

Vehicle suspension systems are critical for ensuring ride comfort, road handling, and vehicle longevity. Poor suspension performance can degrade ride quality and compromise vehicle health. Active suspension systems, equipped with actuators to add or dissipate energy, offer superior ride quality and handling compared to passive systems. This thesis proposes an 8 DOF full-car model that incorporates driver seat dynamics to maximize ride comfort. Based on this model, robust H∞ control strategies are developed to address:

- **Road Disturbance Attenuation**: Minimizing the impact of road irregularities on the driver’s seat.
- **Parametric Uncertainty**: Handling variations in vehicle mass due to passengers or cargo.
- **Input Delay**: Mitigating the effects of delayed control inputs caused by electromechanical actuators and processing times.
- **Actuator Fault Tolerance**: Ensuring system performance despite wear and tear or actuator faults.

The thesis introduces a Center of Gravity (COG) representation to simplify the complex mathematics of polytopic system controller design, enhancing computational efficiency.

## Thesis Objectives

- Develop an 8 DOF active suspension full-car model, including driver seat dynamics.
- Design robust H∞ controllers to address:
  - Disturbance rejection for improved ride quality.
  - Robustness against uncertain vehicle mass.
  - Stability and performance under delayed control inputs.
  - Fault tolerance for actuator degradation.
- Simplify polytopic system control design using COG representation.
- Validate controller performance through simulations.

## Methodology

1. **Modeling**:
   - An 8 DOF full-car model is formulated, capturing vehicle body, wheel, and driver seat dynamics.
   - Vehicle mass is treated as an uncertain parameter to reflect real-world variability.

2. **Controller Design**:
   - **Robust H∞ Control**: Designed to minimize the H∞ norm for disturbance attenuation, uncertainty robustness, delay robustness, and fault tolerance.
   - **COG Representation**: Introduced to reduce the computational complexity of polytopic system control design.
   - Controllers account for:
     - Road disturbances affecting ride quality.
     - Uncertain vehicle mass due to passengers or cargo.
     - Input delays from actuator and processor latencies.
     - Actuator faults due to wear and tear.

3. **Simulation**:
   - MATLAB/Simulink simulations evaluate controller performance under various conditions (road profiles, mass variations, delays, and faults).
   - Performance metrics include ride comfort (seat acceleration), road handling, and actuator effort.

## Results

Simulation results demonstrate the effectiveness of the proposed robust H∞ controllers:
- **Disturbance Rejection**: Significant reduction in seat acceleration, enhancing ride comfort.
- **Parametric Uncertainty**: Stable performance across a range of vehicle masses.
- **Input Delay**: Maintained control efficacy despite actuator and processing delays.
- **Fault Tolerance**: Robust performance under simulated actuator faults.
- The COG representation reduced computational complexity without compromising control quality.

Detailed results, including plots and numerical data, are provided in the thesis document.
