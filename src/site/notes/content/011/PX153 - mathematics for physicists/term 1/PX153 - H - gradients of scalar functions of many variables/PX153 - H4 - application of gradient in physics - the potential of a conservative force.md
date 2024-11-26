---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-h-gradients-of-scalar-functions-of-many-variables/px-153-h4-application-of-gradient-in-physics-the-potential-of-a-conservative-force/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:52.300+00:00"}
---

- similar to *[[content/011/PX153 - mathematics for physicists/term 1/PX153 - G - functions of many variables, calculus/PX153 - G2 - the total differential, and exact and inexact differentials\|exact and inexact differentials]]*
	- a differential is exact if and only if: 
	$$df = A.dx + B.dy =  \frac{\partial f}{\partial x}.dx + \frac{\partial f}{\partial y}.dy$$
	- such that $\frac{\partial A}{\partial y} = \frac{\partial B}{\partial x}$, and there is some function, $f(x,y)$, from which this differential is based
- for a conservative field, $\vec a$, there exists a single-values scalar function of position such that $\vec\nabla \phi = \vec a$ (equivalent to $\vec a \cdot d\vec r$ is an exact differential), and the integral along a path between two points $\int_{A}^{B}\vec a \cdot d\vec r$ does not depend on the path taken

- eg: consider two charges, $q_{1}$ and $q_{2}$, separated by a distance, $r$, with $q_{1}$ at the origin
	- the potential energy is given by: 
	$$U(r) = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r} = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}}\cdot \frac{1}{\sqrt{x^{2}+y^{2}+z^{2}}}$$ 
$$\vec\nabla U(x,y,z) = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}}
	\begin{pmatrix}	\frac{-2x}{2(x^{2}+y^{2}+z^{2})^{\frac{3}{2}}} \hat{\vec i} \\ - \frac{y}{2(x^{2}+y^{2}+z^{2})^{\frac{3}{2}}} \hat{\vec j} \\ - \frac{z}{2(x^{2}+y^{2}+z^{2})^{\frac{3}{2}}} \hat{\vec k}\end{pmatrix}$$
- recall: 
	$$ \hat{\vec r} = \frac{1}{\sqrt{(x^{2}+y^{2}+z^{2}}} \left [x\hat{\vec i} + y\hat{\vec j} + z\hat{\vec k} \right]$$
	$$\vec\nabla U = - \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r^{2}} \hat{\vec r} = -\vec F$$
- coulomb force on $q_{2}$ due to $q_{1}$: 
$$\vec F = -\vec\nabla U(x,y,z)$$
- forces can be described as gradients of potentials are called *conservative forces*
- the work done by a conservative force is given by the potential difference between the start($A$), and the end($B$), independent of the path ![Pasted image 20240102170654.png](/img/user/pics/Pasted%20image%2020240102170654.png)

- we have: 
$$W = Fl\cos\theta$$
- can be generalised in: 
$$dW = \vec F \cdot d\vec{l}$$
- such that: 
$$W = \int_{A}^{B} \vec F.d \vec l$$
- parameterising the trajectory: 
$$\vec l(t) = x(t)\hat{\vec i} + y(t)\hat{\vec j}  + z(t)\hat{\vec k}$$
- as $t=t_{A}$, we  are at $A$; at $t=t_{B}$, we are at $B$
- then: 
$$W = \int_{t_{A}}^{t_{B}}\vec F \frac{d\vec l}{dt}.dt$$
- assuming the force is conservative: $F= -\vec\nabla U$, and using $\frac{d\vec l}{dt}=( \frac{dx}{dt}, \frac{dy}{dt}, \frac{dx}{dt})$: 
$$W = \int_{t_{A}}^{t_{B}}-\vec\nabla U \frac{d\vec l}{dt}.dt$$
$$W = -\int_{t_{A}}^{t_{B}} \left( \frac{\partial U}{\partial x} \frac{dx}{dt} + \frac{\partial U}{\partial y} \frac{dy}{dt} + \frac{\partial U}{\partial z} \frac{dz}{dt} \right).dt$$ 
- using chain rule: 
$$\frac{dU}{dt} =  \frac{\partial U}{\partial x} \frac{dx}{dt} + \frac{\partial U}{\partial y} \frac{dy}{dt} + \frac{\partial U}{\partial z} \frac{dz}{dt}$$
- we get: 
$$W = - \int_{t_{A}}^{t_{B}} \frac{dU}{dt}.dt = -\int_{A}^{B} dU$$
- this gives: 
$$W = U(A)-U(B)$$
	- ie: work done does not depend on the the path for a conservative field

- showing how to determine a scalar field from a conservative vector field
- eg: find the scalar function $U(x,y,z)$, for which the vector function: $\vec a = -\vec\nabla U = -2x\hat{\vec i}-2y\hat{\vec j}-2z\hat{\vec k}$, and such that $U(0,0,9)=0$
	- exact differential?
		- $\vec a\cdot d\vec r = -2xdx -2ydy - 2zdz$
		- if $A_{y}= B_{x}$, $B_{z}= C_{y}$, and $C_{x}=A_{z}$
	$$- \frac{\partial U}{\partial x} = -2x \implies U = x^{2}+ F_{x}(y,z)$$
	$$- \frac{\partial U}{\partial y} = -2x \implies U = y^{2}+ F_{y}(x,z)$$
	$$- \frac{\partial U}{\partial z} = -2z \implies U = z^{2}+ F_{z}(x,y)$$
	$$U(x,y,z) = x^{2}+y^{2}+(z-9)^{2}+c$$
	$$ U(0,0,9) = 0 \implies c=0$$
	$$\therefore U(x,y,z) x^{2}+ y^{2}+ (z-9)^{2}$$
	