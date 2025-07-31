# 🔄 The Curl of a Vector Field – Summary Notes

## 📘 Definition
- The **curl** measures the **rotation** or "swirl" of a vector field.
- In 3D, curl is defined as:
  ```math
  \nabla \times \vec{F} = \begin{vmatrix}
  \hat{i} & \hat{j} & \hat{k} \\
  \partial/\partial x & \partial/\partial y & \partial/\partial z \\
  f_1 & f_2 & f_3
  \end{vmatrix}
  ```
- Result: A **vector field** (unlike divergence, which gives a scalar).

## 🌪 Physical Intuition
- Curl detects local **rotation** or **circulation**.
- Examples:
  - Radial vector field → **zero curl** (irrotational)
  - Circular vector field → **non-zero curl** (rotational)

## 🔁 Key Properties
- **Curl of a gradient** is always zero:
  ```math
  \nabla \times (\nabla f) = 0
  ```
- **Divergence of a curl** is always zero:
  ```math
  \nabla \cdot (\nabla \times \vec{F}) = 0
  ```

## 🧮 2D Curl Simplification
For 2D vector field `F = (f₁(x, y), f₂(x, y))`:
```math
\text{curl}_z = \frac{\partial f_2}{\partial x} - \frac{\partial f_1}{\partial y}
```
- The result points **perpendicular to the plane** (in the 𝑘 or z-direction).

## 🧪 Examples
- **Outward radial flow** (divergent but irrotational): curl = 0
- **Rotational flow** (divergence = 0): curl = 2
- **Solid body rotation**: Constant non-zero curl aligned with rotation axis

## 🛰 Solid Body Rotation Interpretation
- Angular velocity vector: `\vec{\omega}`
- Position vector from origin: `\vec{r}`
- Velocity at a point: 
  ```math
  \vec{v} = \vec{\omega} \times \vec{r}
  ```
- Curl of the velocity field for solid body rotation:
  ```math
  \nabla \times \vec{v} = 2\vec{\omega}
  ```

## 🔄 Operator Summary Table

| Operator     | Input   | Output  | Example Use |
|--------------|---------|---------|--------------|
| Gradient     | Scalar  | Vector  | `∇f`         |
| Divergence   | Vector  | Scalar  | `∇·F`        |
| Curl         | Vector  | Vector  | `∇×F`        |
| Laplacian    | Scalar  | Scalar  | `∇²f = ∇·∇f` |

---

_Next step: apply these tools to conservation laws and PDEs!_