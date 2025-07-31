# 💧 Laplace’s Equation and Potential Flow – Summary Notes

## 📘 What is Potential Flow?
A **potential flow** is a vector field that is:
- ✅ **Steady**: No change in time (`∂v/∂t = 0`)
- ✅ **Incompressible**: Divergence-free (`∇ · v = 0`)
- ✅ **Irrotational**: Curl-free (`∇ × v = 0`)

These properties define a simplified model used in:
- Gravitational and electric potentials
- Steady-state heat conduction
- Fluid flow (especially early aircraft design)

---

## 🧠 Core Idea
Any vector field of the form:
```math
\vec{v} = \nabla \phi
```
where `φ(x, y)` is a **real-valued scalar potential**, is automatically:
- ✅ Irrotational (since `∇ × ∇φ = 0`)
- ✅ Steady (if φ doesn't change with time)

But for the flow to also be **incompressible**, we require:
```math
\nabla \cdot \vec{v} = \nabla \cdot \nabla \phi = \nabla^2 \phi = 0
```

Thus, `φ` must satisfy **Laplace's equation**:
```math
\nabla^2 \phi = 0
```

---

## 🔁 Laplace’s Equation
This is a second-order linear PDE:
```math
\nabla^2 \phi = \frac{\partial^2 \phi}{\partial x^2} + \frac{\partial^2 \phi}{\partial y^2} = 0
```

It arises naturally in systems where the field is:
- Smooth
- Steady-state
- No internal sources or sinks

---

## 🔍 Complex Potential and Analytic Functions

Let `z = x + i y`. Then define:
```math
\Phi(z) = \phi(x, y) + i \psi(x, y)
```

- `Φ(z)` is called the **complex potential**
- `φ(x, y)` is the **velocity potential**
- `ψ(x, y)` is the **stream function**

If `Φ(z)` is **analytic** (e.g., `z²`, `e^z`, `sin(z)`), then both:
```math
\nabla^2 \phi = 0 \quad \text{and} \quad \nabla^2 \psi = 0
```
are satisfied.

✅ This gives a direct way to construct valid potential flows from complex analysis.

---

## 🧪 Example Task
Try `Φ(z) = z^2`:
- Expand and isolate real part `φ(x, y)`
- Compute its gradient to get `v = ∇φ`
- Check:
  - `∇ × v = 0`
  - `∇ · v = 0`

---

## 🧠 Summary Table

| Property            | Math Condition               | Implication                        |
|---------------------|------------------------------|-------------------------------------|
| Steady              | `∂v/∂t = 0`                   | No change over time                |
| Incompressible      | `∇ · v = 0`                   | No volume change (density constant)|
| Irrotational        | `∇ × v = 0`                   | No rotation                        |
| Potential Flow      | `v = ∇φ`, `∇²φ = 0`           | All of the above                   |

---

## 🔄 Applications
- Idealized fluid flow
- Electrostatics
- Gravitational fields
- Steady-state heat conduction
- Airfoil and wing design (early aircraft)

---

By combining vector calculus (grad, div, curl) with complex analysis, we build powerful models for real-world systems using Laplace’s equation.