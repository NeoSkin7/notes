---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/polar-coordinates/","dg-note-properties":{}}
---

# Two Dimensions
In two dimensions, a polar coordinate system is defined using a combination of a radial vector $r$ and an angular vector $\varphi$:
<!-- Column 1 -->
$$
\begin{align*}
\text{2D Polar: }&(r,\varphi)\\
\text{2D Cartesian: }&(x,y)
\end{align*}
$$

<!-- Column 2 -->
$$
x=r\cos{\varphi}\\
y=r\sin{\varphi}
$$

<!-- Column 3 -->
$$
r=\sqrt{x^2+y^2}\\
\varphi=\arctan{\frac{y}{x}}
$$
# Cylindrical
In three dimensions, we can choose to add an additional radius vector $z$:
<!-- Column 1 -->
$$
\begin{align*}
\text{Cylindrical: }&(r,\varphi,z)\\
\text{3D Cartesian: }&(x,y,z)
\end{align*}\\
0\le\varphi<2\pi
$$

<!-- Column 2 -->
$$
x=r\cos{\varphi}\\
y=r\sin{\varphi}\\
z=z
$$

<!-- Column 3 -->
$$
r=\sqrt{x^2+y^2}\\\ \\
\varphi=\arctan{\frac{y}{x}}
$$
This produces a coordinate system which is bounded by a cylinder.
# Spherical
We could, in three dimensions, choose to instead add an extra angular vector $\vartheta$:
<!-- Column 1 -->
$$
\begin{align*}
\text{Spherical: }&(r,\vartheta,\varphi)\\
\text{3D Cartesian: }&(x,y,z)
\end{align*}\\
0\le\vartheta\le\pi\\
0\le\varphi<2\pi
$$

<!-- Column 2 -->
$$
x=r\sin{\vartheta}\cos{\varphi}\\
y=r\sin{\vartheta}\sin{\varphi}\\
z=r\cos{\vartheta}
$$

<!-- Column 3 -->
$$
r=\sqrt{x^2+y^2+z^2}\\
\vartheta=\arccos{\frac{z}{r}}\\
\varphi=\arctan{\frac{y}{x}}
$$
This produces a coordinate system which is bounded by a sphere.