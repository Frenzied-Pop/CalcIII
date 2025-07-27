# [Div, Grad, and Curl — Vector Calculus Building Blocks for PDEs](https://youtu.be/lKXW7DRyyro?si=Q1bWk3__r-PwuGMu)

## Introduction

This lecture introduces the three fundamental operators of vector calculus: **Gradient**, **Divergence**, and **Curl**. These are the building blocks for understanding and deriving **partial differential equations (PDEs)** that describe physical laws like fluid flow, temperature change, and electromagnetism.

---

## The Nabla (Del) Operator `∇`

- Also called "nabla" or "del", it represents a **vector of partial derivatives**.
- Written as:  
  ```
  ∇ = (∂/∂x, ∂/∂y, ∂/∂z)
  ```
- Can be **dotted** (·) or **crossed** (×) with vectors to form divergence and curl.
- Functions similarly to a vector with unit directions **i**, **j**, and **k**.

---

## Gradient Operator `∇f`

- **Input**: Scalar field `f(x, y, z)`  
- **Output**: Vector field  
- Computes the **direction and rate** of greatest increase of `f`.

```
∇f = (∂f/∂x, ∂f/∂y, ∂f/∂z)
```

- Example: Gradient of temperature points in the direction of **fastest heating**.

---

## Divergence Operator `∇·F`

- **Input**: Vector field `F = (F₁, F₂, F₃)`  
- **Output**: Scalar field  
- Measures **net outflow** (expansion) or **inflow** (compression) from a point.

```
∇·F = ∂F₁/∂x + ∂F₂/∂y + ∂F₃/∂z
```

- If divergence is:
  - `> 0`: Field is **expanding** (source).
  - `< 0`: Field is **contracting** (sink).
  - `= 0`: Field is **incompressible**.

---

## Curl Operator `∇×F`

- **Input**: Vector field `F = (F₁, F₂, F₃)`  
- **Output**: Vector field  
- Measures **circulation** or local rotation of a field.

```
∇×F = (
  ∂F₃/∂y - ∂F₂/∂z,
  ∂F₁/∂z - ∂F₃/∂x,
  ∂F₂/∂x - ∂F₁/∂y
)
```

- Positive curl = local **rotation** or "swirl" around a point.

---

## Summary and Big Picture

- These operators form the **alphabet of vector calculus**.
- Used to express **conservation laws** and derive **PDEs**.
- Help us measure **change in space and time**, which is the essence of calculus.
- These tools enable translation from **physical systems** into **math**.

---
