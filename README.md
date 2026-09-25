# -Airflow-analysis-of-Rc-plane-
Airflow analysis of Team Aerohawks which participated in Aerodominator event under Gravitas at Vellore Institute of Technology Vellore from 18th September to 20Th Septemebr,2026.
Analysis was accomplished in Simscale.
# RC Aircraft Aerodynamic Simulation using SimScale

## 1. Project Overview

This project focuses on the aerodynamic analysis of a payload-carrying RC aircraft using **SimScale**, a cloud-based computational fluid dynamics (CFD) simulation platform.

The primary objective is to study the airflow around the aircraft, understand the aerodynamic forces acting on its surfaces, and evaluate its performance under different flight conditions.

The simulation is intended to support the aerodynamic design and optimization of the aircraft before physical fabrication and testing.

## 2. Aircraft Configuration

The aircraft is designed with a high-wing, rectangular-wing configuration for payload-carrying applications.

## 3. Software and Tools

- **SimScale:** Cloud-based CFD simulation and post-processing.
- **Fusion 360:** Aircraft CAD modelling and geometry preparation.
- **AutoCAD**: Engineering drawings and dimensional documentation.

## 4. Simulation Objectives

The main objectives of this simulation are:

1. Visualize airflow around the RC aircraft.
2. Analyze pressure distribution over the wing and fuselage.
3. Study velocity distribution and flow acceleration around the airfoil.
4. Identify regions of flow separation and possible aerodynamic issues.
5. Estimate aerodynamic lift and drag forces.
6. Understand the influence of aircraft geometry on aerodynamic performance.

## 5. Simulation Methodology

### Step 1: CAD Model Preparation

The RC aircraft geometry is created using CAD software and imported into SimScale as STP file.

The model includes the major aerodynamic components, such as:

- Wing with S1223 airfoil profile.
- Fuselage.
- Horizontal and vertical stabilizers.
- Other aerodynamic components included in the final design.

The geometry is checked for surface continuity, unwanted gaps, and intersecting bodies before simulation.

### Step 2: Creation of the Computational Domain

An external flow domain is created around the aircraft to represent the surrounding atmosphere.

The domain is sufficiently large to minimize the influence of the computational boundaries on the airflow around the aircraft.

The aircraft is positioned inside the domain, and the surrounding fluid region is defined as air.

### Step 3: Physics and Boundary Conditions

The simulation is configured using an external aerodynamic flow analysis.

| Parameter | Description |
|---|---|
| Fluid | Air |
| Flow Type | External flow |
| Flow Regime | Incompressible, for low-speed flight conditions |
| Inlet | Uniform incoming airflow |
| Outlet | Pressure outlet |
| Aircraft Surface | No-slip wall |
| Domain Boundaries | Appropriate far-field or slip conditions |

The inlet velocity is selected based on the aircraft's intended flight speed.

For preliminary analysis, a flight velocity of 15 m/s may be considered, subject to the final design requirements.

### Step 4: Mesh Generation

A computational mesh is generated to discretize the fluid domain.

Mesh refinement is applied around the wing, fuselage, leading edge, and trailing edge to capture important flow features.

Additional refinement may be introduced near the aircraft surface to improve the resolution of boundary-layer flow.

A mesh independence study should be performed by comparing results from progressively refined meshes.

### Step 5: Solver Setup

The appropriate steady-state CFD solver is configured in SimScale.

The simulation is run until the solution reaches an acceptable level of convergence.

The residuals, force coefficients, and stability of the monitored quantities are examined to assess convergence.

## 6. Post-Processing and Results

The simulation results are analyzed using SimScale's post-processing tools.

The following outputs are investigated:

| Result | Purpose |
|---|---|
| Velocity Contours | Understand airflow acceleration and deceleration |
| Pressure Contours | Examine pressure distribution over the aircraft |
| Streamlines | Visualize airflow direction and flow patterns |
| Wall Shear Stress | Identify regions of strong surface friction and possible separation |
| Lift Force | Estimate the aerodynamic force perpendicular to the incoming flow |
| Drag Force | Estimate the aerodynamic resistance parallel to the incoming flow |

The results can be used to identify areas for potential aerodynamic improvement and to compare different aircraft configurations.

## 7. Validation and Limitations

CFD results depend on the accuracy of the CAD geometry, boundary conditions, mesh quality, and turbulence modelling.

The simulation represents an approximation of actual flight conditions and does not independently establish the aircraft's flightworthiness.

Further validation can be performed through:

- Mesh independence studies.
- Comparison with theoretical aerodynamic calculations.
- Experimental testing or wind-tunnel measurements.
- Comparison of lift and drag coefficients across different angles of attack.

The effects of propeller slipstream, aircraft control inputs, structural deformation, and unsteady flow may not be captured in the initial simulation.

## 8. Project Workflow

CAD Modelling → Geometry Preparation → Computational Domain → Mesh Generation → CFD Setup → Simulation → Post-Processing → Aerodynamic Evaluation

## 9. Future Work

Future improvements to this project may include:

- Simulating multiple angles of attack.
- Generating lift coefficient versus angle of attack (CL–α) curves.
- Generating drag coefficient versus angle of attack (CD–α) curves.
- Comparing different wing geometries and airfoil configurations.
- Evaluating the aerodynamic effects of payload integration.
- Investigating propeller effects and aircraft stability.

## 10. Acknowledgements

The aerodynamic simulation is carried out using SimScale's cloud-based CFD platform.

This project is undertaken as part of an RC aircraft design and development effort, with the aim of applying aerospace engineering principles to practical aircraft design.

---

**Author:** Ridhviraj Anil Rikke
**Field:** Aerospace Engineering  
**Project:** RC Aircraft Design and Aerodynamic Analysis  
**Simulation Platform:** SimScale
