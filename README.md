# Two-Load Crane System Control using LQR and LQG
(This the final projet from the control systems course)

## Overview  
This project focuses on modeling, analyzing, and controlling a **two-load crane system** using **Linear Quadratic Regulator (LQR)** and **Linear Quadratic Gaussian (LQG) controllers**. The study involves deriving the system's **equations of motion**, performing **state-space representation**, and designing optimal controllers for stability and disturbance rejection.  

## Project Objectives  
- Derive the **nonlinear equations of motion** for the crane system.  
- Linearize the system around an equilibrium point.  
- Analyze **controllability** and **observability** conditions.  
- Design and tune an **LQR controller** for optimal stability.  
- Develop a **Luenberger observer** and an **LQG controller** for state estimation and control.  
- Validate performance through simulations on **both linearized and nonlinear models**.  

## System Description  
The system consists of:  
- A **frictionless cart (crane)** moving along a 1D track actuated by an external force.  
- **Two suspended loads** with different cable lengths.  
- Control inputs include applied force on the crane, while outputs may include cart position and load angles.  

## Implementation Details  
### Mathematical Modeling  
- Derived **nonlinear equations of motion**.  
- Linearized around equilibrium conditions (*x = 0, θ₁ = 0, θ₂ = 0*).  

### Controller Design  
- **LQR**: Designed to minimize a quadratic cost function and stabilize the system.  
- **LQG**: Combines the LQR controller with a **Kalman filter** for state estimation.  

### Simulation  
Validated controller performance using:  
- **Linearized system**  
- **Original nonlinear system**  

## Dependencies & Setup  
Ensure you have the following installed:  
```bash
pip install numpy scipy matplotlib control

