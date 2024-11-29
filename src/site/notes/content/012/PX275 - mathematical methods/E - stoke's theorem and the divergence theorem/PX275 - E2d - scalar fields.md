---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/e-stoke-s-theorem-and-the-divergence-theorem/px-275-e2d-scalar-fields/","created":"2024-11-28T12:13:33.338+00:00","updated":"2024-11-28T12:29:59.010+00:00"}
---

- the [[content/012/PX275 - mathematical methods/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]] can also be used with scalar fields using a maths trick
- consider a scalar field, $\phi$, so a vector can be defined as: $\vec F = \phi \, \vec c = \phi (c_{x}\hat i + c_{y} \hat j  + c_{z} \hat k)$
- the divergence of this vector: 
$$\begin{align*}
	\vec\nabla\cdot\vec F &= \frac{\partial }{\partial x}(\phi c_{x}) + \frac{\partial }{\partial y}(\phi c_{y}) + \frac{\partial }{\partial z}(\phi c_{z}) \\
	&= \frac{\partial \phi}{\partial x} c_{x} + \phi_{x} \frac{\partial c_{x}}{\partial x}  + \dots
\end{align*}$$
$$\therefore \vec\nabla\cdot\vec F = \vec\nabla\cdot (\phi\vec c) = \vec c \cdot \vec\nabla\phi + \phi (\vec\nabla \cdot \vec c)$$
- if $\vec c$ is a constant:
$$\vec\nabla\cdot\vec F = \vec c \cdot \vec\nabla\phi$$
- now, applying the [[content/012/PX275 - mathematical methods/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]]:
$$\begin{align*}
	\iint _{S } \phi \vec c \cdot d\vec s &= \iiint_{V} (\vec c \cdot \vec\nabla \phi )\,dV \\
	\vec c \, \iint \phi\,d\vec s &= \vec c \, \iiint_{V} \vec\nabla \phi \,dV \\
\end{align*}$$
- therefore, the divergence theorem for a scalar field:
$$\boxed{ \therefore \iint \phi\,d\vec s =  \iiint_{V} \vec\nabla \phi \,dV  }$$
