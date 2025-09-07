# Calc III – Week 1: 3D Geometry Formula Sheet

*(Copy/paste friendly markdown with LaTeX.)*

---

## 1) Points & Vectors
- Point: $P=(x,y,z)$
- Vector: $\vec v=\langle a,b,c\rangle$, magnitude $\,|\vec v|=\sqrt{a^2+b^2+c^2}$
- Unit vector: $\hat v = \vec v/|\vec v|$
- Standard basis: $\mathbf{i}=\langle1,0,0\rangle,\;\mathbf{j}=\langle0,1,0\rangle,\;\mathbf{k}=\langle0,0,1\rangle$

## 2) Dot, Angle, Projections
- Dot: $\vec a\cdot\vec b = a_1b_1+a_2b_2+a_3b_3$
- Angle: $\;\vec a\cdot\vec b = |\vec a||\vec b|\cos\theta\;\Rightarrow\;\cos\theta=\dfrac{\vec a\cdot\vec b}{|\vec a||\vec b|}$
- Orthogonal $\Leftrightarrow\;\vec a\cdot\vec b=0$
- Scalar projection of $\vec a$ on $\vec b$: $\;\operatorname{comp}_{\vec b}(\vec a)=\dfrac{\vec a\cdot\vec b}{|\vec b|}$
- Vector projection: $\;\operatorname{proj}_{\vec b}(\vec a)=\dfrac{\vec a\cdot\vec b}{\vec b\cdot\vec b}\,\vec b$

## 3) Cross Product & Areas
- Cross: $\;\vec a\times\vec b=\det\begin{vmatrix}\mathbf{i}&\mathbf{j}&\mathbf{k}\\ a_1&a_2&a_3\\ b_1&b_2&b_3\end{vmatrix}$
- Magnitude & angle: $|\vec a\times\vec b|=|\vec a||\vec b|\sin\theta$; direction by right‑hand rule
- Parallelogram area: $|\vec a\times\vec b|$; triangle area: $\tfrac12|\vec a\times\vec b|$

## 4) Lines in $\mathbb R^3$
- Through $P_0=(x_0,y_0,z_0)$ with direction $\vec v=\langle a,b,c\rangle$:
  - **Vector/param:** $\mathbf r(t)=P_0+t\vec v$ \; i.e., $x=x_0+at,\;y=y_0+bt,\;z=z_0+ct$
  - **Symmetric:** $\dfrac{x-x_0}{a}=\dfrac{y-y_0}{b}=\dfrac{z-z_0}{c}$ (assume nonzero denominators)
- Through two points $P_1,P_2$: direction $\vec v=\overrightarrow{P_1P_2}=P_2-P_1$

## 5) Planes in $\mathbb R^3$
- With normal $\vec n=\langle A,B,C\rangle$ through $P_0$:
  - **Point–normal:** $\vec n\cdot(\mathbf r-P_0)=0$
  - **Scalar:** $Ax+By+Cz=D$ with $D=Ax_0+By_0+Cz_0$
- Through three noncollinear points $P_1,P_2,P_3$:
  - $\vec n=(P_2-P_1)\times(P_3-P_1)$; then use point–normal form

## 6) Distances
- Point–point: $\;\,|P_2-P_1|$
- Point–plane (plane $Ax+By+Cz+D=0$): $\;\dfrac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}$
- Point–line (line $\mathbf r= P_0+t\vec v$): $\;\dfrac{|(P-P_0)\times\vec v|}{|\vec v|}$

## 7) Spheres
- Standard: $\boxed{(x-h)^2+(y-k)^2+(z-\ell)^2=r^2}$ \; (center $(h,k,\ell)$, radius $r$)
- Complete the square to convert from expanded form
- Intersection with plane (if nonempty) is a circle; set the plane’s variable, solve

## 8) Cylinders, Cones, Paraboloids (quadric recognition)
- **Cylinders** (one variable missing):
  - $x^2+y^2=R^2$ → circular cylinder along $z$;
  - $\dfrac{x^2}{a^2}+\dfrac{z^2}{c^2}=1$ (indep. of $y$) → elliptic cylinder along $y$
- **Cone** about an axis: e.g., $y^2+z^2=(kx)^2$ (opens both $\pm x$)
- **Elliptic paraboloid**: one linear $=$ sum of squares, e.g., $x=\tfrac{y^2}{a^2}+\tfrac{z^2}{c^2}$ (vertex at origin; opens in $+x$)
- **Hyperbolic paraboloid** (saddle): $z=\tfrac{x^2}{a^2}-\tfrac{y^2}{b^2}$
- **Ellipsoid**: $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1$
- **Hyperboloid (one sheet)**: $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}-\dfrac{z^2}{c^2}=1$
- **Hyperboloid (two sheets)**: $-\dfrac{x^2}{a^2}-\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1$

**Traces** (quick ID):
- Fix $x=c$ → curve in $yz$‑plane; fix $y=c$ → curve in $xz$‑plane; fix $z=c$ → curve in $xy$‑plane
- Example: $x=y^2+3z^2$ gives
  - $z=0:\;x=y^2$ (parabola),\; $y=0:\;x=3z^2$ (parabola),\; $x=c>0:\;y^2+3z^2=c$ (ellipse)

## 9) Tangent & Normal (2D curves)
- For $y=f(x)$ at $x=x_0$: slope $m=f'(x_0)$
- A tangent direction vector: $\langle1,\,f'(x_0)\rangle$; unit: $\displaystyle \frac{1}{\sqrt{1+[f'(x_0)]^2}}\langle1,\,f'(x_0)\rangle$
- A normal direction: $\langle -f'(x_0),\,1\rangle$; unit: $\displaystyle \frac{1}{\sqrt{1+[f'(x_0)]^2}}\langle -f'(x_0),\,1\rangle$

## 10) Projectile components (angle $\theta$ above horizontal, speed $v$)
- Horizontal: $v_x=v\cos\theta$; Vertical: $v_y=v\sin\theta$
- Handy values: $\cos(\pi/6)=\sqrt3/2,\;\sin(\pi/6)=1/2;\;\cos(\pi/4)=\sin(\pi/4)=\sqrt2/2;\;\cos(\pi/3)=1/2,\;\sin(\pi/3)=\sqrt3/2$

---

**LMS input tip:** enter radicals as `sqrt( )` and vectors as `(a,b,c)`.

