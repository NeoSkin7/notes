---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/linear-transformations/","dg-note-properties":{}}
---

Linear transformations obey the following equation:
$$
T(a\mathbf{n}+b\mathbf{m})=aT(\mathbf{n})+bT(\mathbf{m})
$$
where $T$ is a linear transformation applied to the vectors $\mathbf{n}$ and $\mathbf{m}$, $a$ and $b$ are scalar multipliers.
This equation is comprised of two conservation laws:
<!-- Column 1 -->
# Conservation of Additivity
$$
T(\mathbf{n}+\mathbf{m})=T(\mathbf{n})+T(\mathbf{m})
$$

<!-- Column 2 -->
# Conservation of Scalar Multiplication
$$
T(k\mathbf{n})=kT(\mathbf{n})
$$
# Properties of Linear Transformations
The linear transformation $T$ maps the set $V$ onto the set $W$, mathematically, $T:V\to W$.
## Injective
Linear transformations *may* be injective, whereby every input gives a distinct (unique) output. This is also known as a one-to-one mapping.
This is only true if the kernel of the transformation is equal to the zero vector only:
$$
\ker{T}=\{\mathbf{v}\in V\mid T(\mathbf{v})=0\}=\{0\}
$$
where the kernel $\ker{T}$ is the subset of the domain (input) which is transformed into the zero vector under the transformation.
### Linear Independence
The set of $n$ vectors, $V=\{\mathbf{v}_1,\mathbf{v}_2,\cdots,\mathbf{v}_n\}$, is linearly independent if none of the vectors are collinear/coplanar (multiples of each other):
$$
\sum_{i=1}^n{c_i\mathbf{v}_i}=0\iff c_1=c_2=\cdots=c_n=0
$$
This states that the sum of multiples of vectors can only be zero if all of the scalar coefficients are zero.
> Injective linear transformations will always preserve linear independence.

## Surjective
Linear transformations *may* also be surjective, when every element of the domain exists within the codomain (output). This means that every element of the codomain maps onto an element (not necessarily distinct) of the domain
This is only true when the image of the transformation is equal to the codomain:
$$
\operatorname{im}{T}=\{T(\mathbf{v})\mid\mathbf{v}\in V\}\subseteq W
$$
where the image $\operatorname{im}{T}$ gives the codomain found by applying the function to a domain.
## Bijective
If a linear transformation is both injective and surjective, it is bijective. Only bijective transformations can be inverted.