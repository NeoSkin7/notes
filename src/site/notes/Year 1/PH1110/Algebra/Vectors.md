---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/vectors/","dg-note-properties":{}}
---

# Products
## Scalar/Dot
$$
\mathbf{a}\cdot\mathbf{b}=\left|\mathbf{a}\right|\left|\mathbf{b}\right|\cos{\vartheta}
$$
where $\vartheta$ is the angle between the two vectors.
Alternatively:
$$
\mathbf{a}\cdot\mathbf{b}=a_xb_x+a_yb_y+a_zb_z
$$
where $\mathbf{a}=a_x\mathbf{\hat{i}}+a_y\mathbf{\hat{j}}+a_z\mathbf{\hat{k}}$ and $\mathbf{b}=b_x\mathbf{\hat{i}}+b_y\mathbf{\hat{j}}+b_z\mathbf{\hat{k}}$.
## Vector/Cross
$$
\mathbf{a}\times\mathbf{b}=\begin{vmatrix}
\mathbf{\hat{i}} & \mathbf{\hat{j}} & \mathbf{\hat{k}} \\
a_x & a_y & a_z \\
b_x & b_y & b_z
\end{vmatrix}=
\begin{vmatrix}
a_y & a_z \\
b_y & b_z
\end{vmatrix}\mathbf{\hat{i}}-
\begin{vmatrix}
a_x & a_z \\
b_x & b_z
\end{vmatrix}\mathbf{\hat{j}}+
\begin{vmatrix}
a_x & a_y \\
b_x & b_y
\end{vmatrix}\mathbf{\hat{k}}
$$
# Projections
## Scalar
The scalar projection of $\mathbf{b}$ onto $\mathbf{a}$ is:
$$
\operatorname{proj}_{\mathbf{a}}{\mathbf{b}}=b_a=\cos{\vartheta}\left|\mathbf{b}\right|=\frac{\mathbf{a}\cdot\mathbf{b}}{\left|\mathbf{a}\right|}=\mathbf{a}\cdot\mathbf{\hat{b}}
$$
## Vector
The vector projection of $\mathbf{b}$ onto $\mathbf{a}$ is:
$$
\overrightarrow{\operatorname{proj}_{\mathbf{a}}{\mathbf{b}}}=\mathbf{b_{a}}=b_a\mathbf{\hat{a}}=b_a\frac{\mathbf{a}}{\left|\mathbf{a}\right|}=\mathbf{a}\frac{\mathbf{a}\cdot\mathbf{b}}{\left|\mathbf{a}\right|^2}=\mathbf{a}\frac{\mathbf{a}\cdot\mathbf{b}}{\mathbf{a}\cdot\mathbf{a}}
$$
# Triple Products
## Scalar
$$
\mathbf{a}\cdot(\mathbf{b}\times\mathbf{c})=
\begin{vmatrix}
\mathbf{a} & \mathbf{b} & \mathbf{c}
\end{vmatrix}=
\begin{vmatrix}
a_x & a_y & a_z \\
b_x & b_y & b_z \\
c_x & c_y & c_z
\end{vmatrix}
$$
where $a_x=\mathbf{a}\cdot\mathbf{\hat{i}}$, the dot product of the vector $\mathbf{a}$ and the $x$ basis vector $\mathbf{\hat{i}}$, equivalent to the scalar projection.
This is equivalent to the volume of the parallelepiped defined by the vectors $\mathbf{a}$, $\mathbf{b}$, and $\mathbf{c}$.
### Properties
$$
\begin{align*}
\mathbf{a}\cdot(\mathbf{b}\times\mathbf{c})&=\mathbf{b}\cdot(\mathbf{c}\times\mathbf{a})\\
&=-\mathbf{b}\cdot(\mathbf{a}\times\mathbf{c})\\
&=\mathbf{c}\cdot(\mathbf{a}\times\mathbf{b})\\
&=-\mathbf{c}\cdot(\mathbf{b}\times\mathbf{a})
\end{align*}
$$
## Vector
$$
\mathbf{a}\times(\mathbf{b}\times\mathbf{c})=(\mathbf{a}\cdot\mathbf{c})\mathbf{b}-(\mathbf{a}\cdot\mathbf{b})\mathbf{c}
$$
### Properties
$$
\mathbf{a}\times(\mathbf{b}\times\mathbf{c})=(\mathbf{b}\times\mathbf{c})\times-\mathbf{a}
$$
# Distances
## Line to Point
The shortest distance from a point to a line, $d$, is calculated as follows:
$$
d=\frac{\left|(\mathbf{c}-\mathbf{a})\times\mathbf{b}\right|}{\left|\mathbf{b}\right|}
$$
for a line $\mathbf{r}=\mathbf{a}+\lambda\mathbf{b}$ and a point $\mathbf{c}$.
## Plane to Line
The shortest distance from a point to a plane, $d$, is calculated as follows:
$$
d=\frac{(\mathbf{c}-\mathbf{a})\cdot\mathbf{n}}{\left|\mathbf{n}\right|}=(\mathbf{c}-\mathbf{a})\cdot\mathbf{\hat{n}}=\mathbf{c}\cdot\mathbf{\hat{n}}-k
$$
for a plane $\mathbf{r}\cdot\mathbf{\hat{n}}=\mathbf{a}\cdot\mathbf{\hat{n}}=k$ and a point $\mathbf{c}$.