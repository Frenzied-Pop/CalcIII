# 🔁 The Continuity Equation – Mass Conservation in Fluid Flow

## 📘 Core Concept
The **Continuity Equation** is a Partial Differential Equation (PDE) expressing **mass conservation** in a fluid:
```math
\frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{u}) = 0
```
- `ρ(x, t)`: density (scalar)
- $$\vec{u}(x, t)$$: velocity field (vector)
- This equation ensures that **mass is not created or destroyed** in the flow.

---

## 📦 Derivation via Gauss's Divergence Theorem
From Gauss’s theorem:
```math
\iint_S \rho \vec{u} \cdot \hat{n} \, dS = \iiint_V \nabla \cdot (\rho \vec{u}) \, dV
```
- Total **outflow of mass** across the surface = **divergence of mass flux** within the volume.
- Taking the time derivative of total mass in a control volume and equating it with the flux gives:
```math
\frac{d}{dt} \iiint_V \rho \, dV = - \iiint_V \nabla \cdot (\rho \vec{u}) \, dV
```
By merging terms and assuming this holds for **all control volumes**:
```math
\frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{u}) = 0
```

---

## 🌊 Incompressible Flow Case
If the fluid has **constant density** (e.g. water):
- $$\( \nabla \rho = 0 \)$$
- $$\( \frac{\partial \rho}{\partial t} = 0 \)$$
Then the continuity equation simplifies:
```math
\nabla \cdot \vec{u} = 0
```
✅ The flow is said to be **divergence-free**.

---

## ⚠️ Source Terms and Limitations
If **mass is created or destroyed** (e.g. nuclear reactions):
```math
\frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{u}) = Q
```
- `Q(x, t)`: source term (positive: creation, negative: destruction)

If fields are **discontinuous** (shock waves, supersonic jets):
- The derivative terms may break down.
- We fall back to **control volume integrals** and **numerical approximations**.

---

## 🔍 Physical Interpretation
- **ρ ∇·u**: Local compression/expansion
- **u · ∇ρ**: Advection of density (movement of varying density)
- Total change = local + advected changes

---

## 🔧 Chain Rule Expansion (for compressible flow)
Using product rule:
```math
\nabla \cdot (\rho \vec{u}) = \rho \nabla \cdot \vec{u} + \vec{u} \cdot \nabla \rho
```
Full equation:
```math
\frac{\partial \rho}{\partial t} + \rho \nabla \cdot \vec{u} + \vec{u} \cdot \nabla \rho = 0
```

---

## 🔁 Related Conservation Laws
- **Momentum conservation** → Navier–Stokes equations
- **Energy conservation** → Energy equations for thermodynamics

✅ These follow similar derivations using Gauss’s theorem and physical assumptions.

---

## 🧠 Summary Table

| Assumption         | Resulting Form                        |
|--------------------|----------------------------------------|
| General fluid      | $$\( \frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{u}) = 0 \)$$ |
| Incompressible     | $$\( \nabla \cdot \vec{u} = 0 \)$$          |
| With source/sink   | $$\( \frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{u}) = Q \)$$|

---

_This equation is the bedrock of fluid dynamics, enabling derivation of more advanced models for momentum and energy transport._
