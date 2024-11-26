---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/c-vector-calculus/px-275-c2b-examples-of-using-the-laplacian/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:28.872+00:00"}
---

## laplace's equation
$$\nabla^{2}\phi =0$$
where, $\phi$ is a scalar
- heat transfer in a steady state
## poisson's equation
$$\nabla^{2}\phi = k$$
where, $\phi$ is a scalar, and $k$ is a constant
- potential field from a charge/mass
- wave equation: 
$$\nabla^{2}\phi = \frac{1}{c^{2}} \frac{\partial^{2} {\phi}}{\partial {t}^{2}}$$
	where, $\phi$ is a scalar, and $c=$ phase speed
- it can be rearranged and written as $\square \phi =0:$ **d'alembert's equation** with applications in electrodynamics
### on vectors
$$\nabla^{2}\vec E = \frac{1}{c^{2}} \frac{\partial^{2} {E}}{\partial {t}^{2}}$$
- in cartesians (only): 
$$\begin{align*}
	\nabla^{2} \vec E &= (\nabla^{2}E_{x})\,\hat i + (\nabla^{2}E_{y})\,\hat j + (\nabla^{2}E_{z})\,\hat k \\\\
	\nabla^{2}E_{x} &= \frac{\partial^{2} {E_{x}}}{\partial {x}^{2}} + \frac{\partial^{2} {E_{x}}}{\partial {y}^{2}} + \frac{\partial^{2} {E_{x}}}{\partial {z}^{2}} \\
	\nabla^{2}E_{y} &= \frac{\partial^{2} {E_{y}}}{\partial {x}^{2}} + \frac{\partial^{2} {E_{y}}}{\partial {y}^{2}} + \frac{\partial^{2} {E_{y}}}{\partial {z}^{2}} \\
	\nabla^{2}E_{z} &= \frac{\partial^{2} {E_{z}}}{\partial {x}^{2}} + \frac{\partial^{2} {E_{z}}}{\partial {y}^{2}} + \frac{\partial^{2} {E_{z}}}{\partial {z}^{2}}
\end{align*}$$
