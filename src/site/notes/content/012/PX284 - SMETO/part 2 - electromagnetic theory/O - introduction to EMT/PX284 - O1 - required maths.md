---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/o-introduction-to-emt/px-284-o1-required-maths/","noteIcon":"1","created":"2025-02-11T09:49:52.120+00:00","updated":"2025-02-17T10:22:14.317+00:00"}
---

## vector calculus
- the [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]] $\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}$
$$\oiint_{S} \vec W \cdot d\vec S = \iiint_{V} \vec\nabla \cdot \vec W \, dV$$
- [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E1a - stokes' theorem\|stokes' theorem]]
$$\oint_{C} \vec W \cdot d\vec s = \iint_{S}(\vec\nabla \times \vec W) \cdot d\vec S$$
- additionally:
	- if $\int_{V}W\,dV = 0 \; \forall V \implies W = 0$ everywhere
	- if $\int_{S}\vec W\cdot d\vec S = 0 \; \forall S \implies \vec W = 0$ everywhere
## vector identities
 - will be provided in exam
$$\begin{gather}
\vec{a} \times (\vec{b} \times \vec{c}) = (\vec{a} \cdot \vec{c}) \vec{b} - (\vec{a} \cdot \vec{b}) \vec{c} \\
\vec\nabla \times (\vec\nabla \times \vec{W}) = \vec\nabla(\vec\nabla \cdot \vec{W}) - \nabla^{2} \vec{\omega}\\\\
\vec\nabla \cdot (f \vec{W}) = (\vec\nabla f) \cdot \vec{W} + f \vec\nabla \cdot \vec{\omega} \\\\
\vec\nabla \times (f \vec{W}) = (\vec\nabla f) \times \vec{W} + f \vec\nabla \times \vec{W} \\\\
\vec\nabla \cdot (\vec\nabla \times \vec{W}) = 0 \\\\
\vec\nabla \cdot (\vec{V} \times \vec{\omega}) = \vec{W} \cdot (\vec\nabla \times \vec{V}) - \vec{V} \cdot (\vec\nabla \times \vec{W})
\end{gather}$$
