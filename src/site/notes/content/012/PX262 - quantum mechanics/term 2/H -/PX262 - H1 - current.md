---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/h/px-262-h1-current/","noteIcon":"1","created":"2025-01-06T18:16:36.405+00:00","updated":"2025-01-06T19:44:47.848+00:00"}
---

- current can be analogised with conservation of mass in a fluid

![PX262 - H1 - current.png|500](/img/user/pics/PX262%20-%20H1%20-%20current.png)

- flux through the surface is equal to the rate of decrease of mass inside it:
$$ \iint \vec j \cdot d\vec S = - \iiint_{V} \frac{\partial \rho}{\partial t}\,dV$$
	where, $\vec j$ is the current density vector
- using the [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]]:
$$\vec\nabla\cdot \vec j = - \frac{\partial \rho}{\partial t} \tag{1}$$

- in quantum mechanics, the density:
$$\begin{gather*}
\rho = \psi^{*}(x,t) \psi(x,t) \\ \\
\implies \frac{\partial \rho}{\partial t} = \frac{\partial }{\partial t} (\psi ^{*}\psi) = \psi^{*}(x,t) \frac{\partial \psi(x,t)}{\partial t} + \frac{\partial \psi^{*}(x,t)}{\partial t} \psi(x,t)
\end{gather*}$$

- multiplying the schrödinger equation by $\psi^*:$
$$i\hbar \psi^{*}\frac{\partial \psi}{\partial t} = - \frac{\hbar^{2}}{2m} \psi^{*}\frac{\partial^{2} {\psi}}{\partial {x}^{2}} + V(x) \psi^{*}\psi \tag{2}$$
- taking its complex conjugate:
$$-i\hbar \psi\frac{\partial \psi^*}{\partial t} = - \frac{\hbar^{2}}{2m} \psi\frac{\partial^{2} {\psi^{*}}}{\partial {x}^{2}} + V(x) \psi\psi^{*} \tag{3}$$
- subtracting equation $(3)$ from $(2):$
$$i\hbar \left( \psi^{*}\frac{\partial \psi}{\partial t} + \psi\frac{\partial \psi^{*}}{\partial t} \right) = i\hbar \frac{\partial}{\partial t} (\psi ^*\psi) = - \frac{\hbar^{2}}{2m}  \left(\psi^{*}\frac{\partial^{2} {\psi} }{\partial {x}^{2}} - \psi \frac{\partial^{2} {\psi^{*}}}{\partial {x}^{2}} \right)$$
- in the $RHS:$ 
$$\begin{gather}
\psi^* \frac{\partial^2 \psi}{\partial x^2} = \frac{\partial}{\partial x} \left( \psi^* \frac{\partial \psi}{\partial x} \right) - \frac{\partial \psi^*}{\partial x} \frac{\partial \psi}{\partial x} 
\\ \psi \frac{\partial^2 \psi^*}{\partial x^2} = \frac{\partial}{\partial x} \left( \psi \frac{\partial \psi^*}{\partial x} \right) - \frac{\partial \psi}{\partial x} \frac{\partial \psi^*}{\partial x}
\end{gather}$$
- therefore, it can be written as: 
$$i\hbar \frac{\partial }{\partial t} (\psi^{*}\psi) = - \frac{\hbar^{2}}{2m} \left(\psi^{*}\frac{\partial{\psi} }{\partial {x}} - \psi \frac{\partial {\psi^{*}}}{\partial {x}} \right) \tag{4}$$
- using the 1D form of equation $(1):$
$$\frac{\partial \vec j}{\partial x}= - \frac{\partial \rho}{\partial t}$$
- comparing it with equation $(4):$ 
$$\vec j = \frac{\hbar}{2im} \left(\psi^{*} \frac{\partial \psi}{\partial x} - \psi \frac{\partial \psi^{*}}{\partial x} \right)$$
- in 3D:
$$\vec j = \frac{\hbar}{2im} (\psi^{*} \vec\nabla \psi - \psi \vec\nabla \psi^{*})$$

- checking this result for a plane wave:
$$\psi(\vec r, t) = A \, \exp\left[i \left(\vec k \cdot \vec r - \frac{Et}{\hbar}\right) \right]$$
- the charge density:
$$\begin{gather}
\vec j = \frac{\hbar}{2im} A^{*}A \big[\exp(-\vec k \cdot \vec r ) ik \exp(i \vec k \cdot \vec r) - \exp(i \vec k \cdot \vec r) \{-i\vec k \exp(-i \vec k \cdot \vec r)\}\big] \\ 
\therefore \vec j = \frac{\hbar\vec{k}}{m} A^{*}A
\end{gather}$$
	where, ${} \cfrac{\hbar \vec k}{m} {}$ is equivalent to the velocity, and $A^{*}A$ to the density as $\vec j = \text{velocity} \times \text{density}$

