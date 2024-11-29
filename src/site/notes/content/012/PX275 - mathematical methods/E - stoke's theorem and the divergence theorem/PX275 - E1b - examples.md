---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/e-stoke-s-theorem-and-the-divergence-theorem/px-275-e1b-examples/","created":"2024-11-28T12:29:28.396+00:00","updated":"2024-11-28T12:56:49.077+00:00"}
---

## a maths example
![Pasted image 20241128123318.png|500](/img/user/pics/Pasted%20image%2020241128123318.png)
- considering a field:
$$\vec F = x^{2} \hat i + x^{2} \hat j + x^{2} \hat k$$
- to apply stokes' theorem:
$$d\vec s = dA\, \hat n = dx\, dy \, \hat n = dx\,dy \, \hat k$$
$$\begin{align*}
	\nabla \times \vec{F} &= \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ F_x & F_y & F_z \end{vmatrix} \\
	&= \hat{i} \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z} \right) - \hat{j} \left( \frac{\partial F_z}{\partial x} - \frac{\partial F_x}{\partial z} \right) + \hat{k} \left( \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right) \\
\end{align*}$$
$$\begin{align*}
	\iint_{R}(\vec\nabla\times \vec F)\cdot d\vec s &= \int_{0}^{a} \int_{0}^{a} \left(\frac{\partial F_{y}}{\partial x}  - \frac{\partial F_x}{\partial y}\right)\,dx\,dy \\
	&= \int_{0}^{a} \int_{0}^{a} \left( 2x \right)\,dx\,dy \\
	&= a^{3}
\end{align*}$$
- to check if it a conservative field, find $\oint \vec F\cdot d\vec r$

## magnetic field around a current carrying wire
![Pasted image 20241128125020.png|500](/img/user/pics/Pasted%20image%2020241128125020.png)
- the following maxwell equation gives the static magnetic field:
$$\vec\nabla \times \vec B = \mu_{0} \vec J$$
- integrating over the surface:
$$ \int_{S} (\vec\nabla \times \vec B) \cdot d\vec s = \iint_{S} \mu_{0} \vec J\cdot d\vec s$$
- using [[content/012/PX275 - mathematical methods/E - stoke's theorem and the divergence theorem/PX275 - E1a - stokes' theorem\|stokes' theorem]]:
$$\oint_{C} \vec B \cdot d\vec r = \iint_{S} \mu_{0} \vec J \cdot d\vec s = \mu_{0}I$$
- this is [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|ampere's law]]
- evaluating the $LHS:$ 
$$\begin{align*}
	\oint_{C} \vec B \cdot d\vec r &= \int_{\phi=0}^{2\pi} B(r ) \, \hat e_{\phi}\cdot r \,d\phi \, \hat e_\phi
	
\end{align*}$$