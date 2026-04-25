---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/matrices/","dg-note-properties":{}}
---

# Rotations
A linear transformation $T_\vartheta$ that rotates anticlockwise through an angle $\vartheta$ about the origin can be represented as a matrix:
$$
\mathbf{T}_\vartheta=\begin{pmatrix}
\cos{\vartheta} & -\sin{\vartheta} \\
\sin{\vartheta} & \cos{\vartheta}
\end{pmatrix}
$$
# Determinant
The determinant of a matrix $\mathbf{A}$ can be determined using the following formula:
$$
\det{\mathbf{A}}=\left|\mathbf{A}\right|=\sum_{j=1}^n{(-1)^{i+j}a_{ij}M_{ij}}=\sum_{j=1}^n{a_{ij}C_{ij}}
$$
where matrix $\mathbf{A}$ has $i$ rows and $j$ columns, $a_{ij}$ is the matrix element in row $i$ and column $j$, $M_{ij}$ is the minor of $ij$, and $C_{ij}$ is the cofactor of $ij$ - defined as $(-1)^{i+j}M_{ij}$.
The determinant formula holds for any choice of row $i$, but the first row is generally used (arbitrarily).