# 🌪️ Divergence Operator – Summary Notes

## 📘 Definition

- The **divergence** of a vector field `F = (f₁, f₂)` is defined as:
  
  ```
  ∇·F = ∂f₁/∂x + ∂f₂/∂y
  ```
- It returns a **scalar field** representing net inflow or outflow at a point.

## 🌊 Physical Intuition

- Positive divergence: **sources**, material flows out
- Negative divergence: **sinks**, material flows in
- Zero divergence: **incompressible or rotational flows**, e.g., perfect circular motion

## 🔁 Properties

- The divergence operator is **linear**:
  ```
  ∇·(aF + bG) = a∇·F + b∇·G
  ```
- Superposition of solutions holds — useful for linear PDEs

## 🧪 Examples

### Example 1 – Outward Flow:
  ```
  F(x, y) = (x, y) ⇒ ∇·F = 1 + 1 = 2 (positive)
  ```
  Expanding flow, material is **diverging** outward.

### Example 2 – Inward Flow:
  ```
  F(x, y) = (–x, –y) ⇒ ∇·F = –1 –1 = –2 (negative)
  ```
  Converging flow, material is **compressing**.

### Example 3 – Rotation Only:
  ```
  F(x, y) = (–y, x) ⇒ ∇·F = 0 (divergence-free)
  ```
  Rotational flow, **no net compression/expansion**.

## 🔄 Connection to Other Operators

- Gradient: Converts scalar → vector
- Divergence: Converts vector → scalar
- `∇·(∇f)` = Laplacian `∇²f`, combines both operators

## ⚡ Laplacian Operator

- Defined as:
  ```
  ∇²f = ∂²f/∂x² + ∂²f/∂y²
  ```
- Arises from divergence of the gradient of a scalar
- Central to modeling heat, electrostatics, and fluid flow

## 🧠 Interpretation with Differential Equations

- The vector field defines a system: `dx/dt = F(x, y)`
- Divergence connects to the **rate of expansion/compression** of volume elements
- Used in PDEs like Laplace’s equation: `∇²f = 0`

---

_Next topic: Curl — measuring the rotation of vector fields._