---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/e-conservation-laws-and-symmetries/px-285-e4-rotation-of-space/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:04:42.700+00:00"}
---

- consider the isotropy of space (rotational symmetry)
- same dynamics expected, regardless of rotation, so there should be no 'special direction'

- consider a position vector, $\vec r$, rotated by a small angle, ${} \vec{\delta\phi}: {}$ $\vec r \to \vec r + \vec{\delta r}$, where, $\vec{\delta r} = \vec{\delta\phi} \times \vec r$
- the rotation also acts on velocities: $\vec{\delta v} = \vec{\delta\phi} \times \vec v$
- the lagrangian: 
$$L(\vec r, \vec v) \to L(\vec r + \vec{\delta r}, \vec v + \vec{\delta v}) = L(\vec r, \vec v) + \delta L$$
- if space is isotropic, $\delta L = 0:$ 
$$L(\vec r, \vec v) = L(\vec r + \vec{\delta r})$$
$$\delta L = \vec{\delta r} \cdot \vec\nabla L + \vec{\delta v} \cdot \vec\nabla_{v}L = (\vec{\delta\phi} \times \vec r) \cdot \vec\nabla L + (\vec{\delta\phi \times \vec v}) \cdot \vec\nabla_{v}L$$
$$\vec\nabla_{v}L = \begin{pmatrix}\frac{\partial L}{\partial v_{x}} \\ \frac{\partial L}{\partial v_{y}} \\ \frac{\partial L}{\partial v_{z}}\end{pmatrix}= \vec p$$
$$\vec\nabla L = \begin{pmatrix}\frac{\partial L}{\partial x} \\ \frac{\partial L}{\partial y} \\ \frac{\partial L}{\partial z}\end{pmatrix}= \dot{\vec p}$$
$$\begin{align*}
	\delta L &= (\vec{\delta\phi} \times \vec r) \cdot \dot{\vec p} + (\vec{\delta \phi} \times\vec v) \cdot \vec p \\
	&=  \vec{\delta \phi} \cdot (\vec r \times \dot{\vec p}) + \vec{\delta \phi} \cdot (\vec v \times \vec p) \\
	&= \vec{\delta \phi} \cdot [ \vec r \times \dot{\vec p} + \vec v \times \vec p] \\
	&= \vec{\delta \phi} \cdot [ \vec r \times \dot{\vec p} + \dot{\vec r} \times \vec p] \\
	&= \vec{\delta \phi} \cdot \frac{d}{dt}(\vec r \times \vec p)
\end{align*}$$
- if space is isotropic, $\delta L =0:$ 
$$\frac{d}{dt}\vec M = \frac{d}{dt}(\vec r \times\vec p) =0$$
- the angular momentum, $\vec M$, is an invariant, ie: a constant of the motion
- $\vec M$ contains $d$ invariant components, each arising from the rotational symmetries in $d$-dimensional space 
## general case
- more generally, for $N$ interacting particles, eg: bound in a solid body, there will be $3N$ coordinates and $3N$ velocities, giving the lagrangian: 
$$L(x_{1},\dots z_{n}, \dot x_{1},\dots \dot z_n)$$
- for a rotation, $L \to L + \delta L:$ 
$$\delta L = \sum\limits_{i=1}^{N} \left[ \begin{pmatrix}\frac{\partial L}{\partial x_{i}} \\ \frac{\partial L}{\partial y_{i}} \\ \frac{\partial L}{\partial z_{i}}\end{pmatrix} \cdot \begin{pmatrix}\delta x_{1} \\ \delta y_{1} \\ \delta z_{1}\end{pmatrix} + \begin{pmatrix}\frac{\partial L}{\partial \dot x_{i}} \\ \frac{\partial L}{\partial \dot y_{i}} \\ \frac{\partial L}{\partial \dot z_{i}}\end{pmatrix} \cdot \begin{pmatrix}\delta \dot x_{1} \\ \delta \dot y_{1} \\ \delta \dot z_{1}\end{pmatrix} \right]$$
- this is the first order taylor expansion in $6N$ dependent variables
$$\begin{align*}
	\delta L &= \sum\limits_{i} (\dot{\vec p_{i}} \cdot \vec{\delta r_{i}} + \vec p_{i} \cdot \vec{\delta v_{i}}) \\
	&= \sum\limits_{i} \vec{\delta\phi} \cdot \frac{d}{dt}(\vec r_{i}\times \vec p_{i}) \\
	&= \vec{\delta\phi} \cdot \frac{d}{dt}\sum\limits_{i} (\vec r_{i}\times \vec p_{i})
\end{align*}$$
- for an arbitrary rotation, $\delta L = 0$ only if $\frac{d}{dt}\sum\limits_{i} (\vec r_{i}\times \vec p_{i}) = 0$
- define the angular momentum, $\vec M = \sum\limits_{i} (\vec r_{i}\times \vec p_{i})$
- $\frac{d}{dt}\vec M =0$, so it is a conserved quantity
- $\vec M$ has $d=3$ components, one for each rotational symmetry
