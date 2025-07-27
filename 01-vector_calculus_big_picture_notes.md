# Vector Calculus & PDEs – Big Picture Overview

## Introduction
Vector calculus is used to derive and solve partial differential equations (PDEs), especially those that express conservation laws like mass, momentum, and energy.

## Vector Calculus and Conservation Laws
- PDEs describe conservation laws in physics.
- Vector calculus operations like **gradient**, **divergence**, and **curl** are the language of these laws.
- These concepts were often taught independently but are deeply connected.

## Fluid Flow and Vector Fields
- Example: Fluid flow in the Gulf of Mexico.
- Velocity field `\vec{u}(x, y, t) = (u(x, y, t), v(x, y, t))`
- This vector field is a solution to PDEs like the Navier-Stokes equations.

## Deriving PDEs (Navier-Stokes and Heat Equation)
- Heat Equation: `∂T/∂t = α²(∂²T/∂x² + ∂²T/∂y²)`
- This uses the **Laplacian** operator: `∇²T`
- These equations are derived from physical principles using vector calculus.

## Dynamics of Particles in Vector Fields
- A vector field (like fluid flow) induces a **dynamical system**.
- You can drop a particle in the field and solve for its trajectory using:
  - `dx/dt = u(x, t)`
- Useful in modeling oil spills, rescue operations, etc.

## Vector Calculus Operations (Div, Grad, Curl)
- **Divergence** measures how much a field spreads out from a point (source/sink).
- **Curl** measures rotational motion in the field (e.g., cyclones).
- **Gradient** turns a scalar field (like temperature) into a vector field.
  - Points in the direction of fastest increase.
- Crucial in physics and machine learning (e.g., gradient descent).

## Applications and Broader Impact
- PDEs help model real systems:
  - Heat flow, fluid dynamics, aerodynamic lift.
- Simulations predict behavior like oil drift, heat distribution, and particle motion.

## What's Next
- Next videos will dive into:
  - Gauss’s Divergence Theorem
  - Stokes’s Theorem
  - Derivations of key PDEs from conservation laws
