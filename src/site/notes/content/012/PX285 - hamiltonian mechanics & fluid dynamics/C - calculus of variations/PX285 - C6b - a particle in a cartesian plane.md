---
dg-publish: true
---
- consider a particle moving in a cartesian plane with a potential, $V(x,y)$
- the lagrangian: 
$$
L = \frac{1}{2}mv^{2}- V(x,y)
$$
	where, $v^{2}= \dot x^{2}+ \dot y^{2}$
- here, there are two position coordinates, ie: $d=2$, so expect two euler-lagrange equations: 
$$\begin{align*}
	-\frac{\partial V}{\partial x} &= \frac{d}{dt} m\dot x = \frac{d}{dt} p_{x} \\
	-\frac{\partial V}{\partial y} &= \frac{d}{dt} m\dot y = \frac{d}{dt} p_{y}
\end{align*}$$
- define the momentum vector:
$$
\vec p = \begin{pmatrix} p_{x} \\ p_{y}\end{pmatrix}
$$
$$
\frac{d}{dt} \begin{pmatrix} p_{x} \\ p_{y}\end{pmatrix} = \begin{pmatrix} -\frac{\partial V}{\partial x} \\ -\frac{\partial V}{\partial y}\end{pmatrix} = \vec F
$$
- therefore, a fully vectorized form of newton's second law is obtained: 
$$
\frac{d}{dt}\vec p = \vec F = -\vec\nabla V
$$
