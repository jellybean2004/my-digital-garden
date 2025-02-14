---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/k-circulation-and-vorticity/px-285-k1-vorticity/","noteIcon":"1","created":"2025-02-13T14:16:13.843+00:00","updated":"2025-02-13T14:28:00.181+00:00"}
---

## definition
- **vorticity** is the curl of a flow:
$$\vec \omega = \vec\nabla \times \vec u$$
- a flow is **irrotational** if $\vec\omega = 0$ everywhere
## circulation
- the circulation is defined around an arbitrary closed path $(\Gamma):$
$$K = \oint_{\Gamma} \vec u \cdot d\vec l$$
- using [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E1a - stokes' theorem\|stokes' theorem]]:
$$K = \oint_{\Gamma} \vec u \cdot d\vec l = \iint_{S} (\vec\nabla \times \vec u) \cdot d\vec S$$
	where, $S$ is the surface bounded by the contour, $\Gamma$

- in irrotational flows, $\omega = \vec\nabla \times \vec u = 0 \implies K = 0$
## irrotational rotation
- considering a vortex:
$$\vec u = \left(\frac{A}{r}\right) \hat \theta$$
	where, $\hat\theta$ is the polar angle in cylindrical coordinate system
$$\begin{align*}
\vec \omega &= \vec\nabla \times \vec u \\
&= \begin{vmatrix} \hat r & r \,\hat \theta  &  \hat z \\ \frac{\partial }{\partial r} & \frac{\partial }{\partial \theta}  & \frac{\partial }{\partial z} \\ u_{r} & r\,u_\theta & u_{z}\end{vmatrix} \\
&= \begin{vmatrix} \hat r & r \,\hat \theta  &  \hat z \\ \frac{\partial }{\partial r} & \frac{\partial }{\partial \theta}  & \frac{\partial }{\partial z} \\ 0 & A & 0\end{vmatrix}\\
&= 0
\end{align*}$$
- thus, the flow is irrotational
