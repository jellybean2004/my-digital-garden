---
dg-publish: true
---

## cartesian coordinates
- the laplacian or the grad-squared operator is given by: 
$$\nabla^{2}f = \frac{\partial^{2} {f}}{\partial {x}^{2}} + \frac{\partial^{2} {f}}{\partial {y}^{2}} + \frac{\partial^{2}{f}}{\partial {z}^{2}}$$
- $\nabla^{2}$ acts as a scalar, giving a scalar result
- eg: in [[content/012/PX262 - quantum mechanics/B - introduction/PX262 - B1 - the schrödinger equation\|the schrödinger equation]]: 
$$\frac{-\hbar^{2}}{2m} \nabla^{2}\psi + V \psi = E\psi$$
		where, $\psi=$ the wavefunction, $E=$ eigen value, $V=$ the potential function
	- the hamiltonian operators:
		- $\frac{-\hbar^{2}}{2m}\nabla^{2}\psi$ gives the kinetic energy
		- $V\psi$ gives the potential energy

- $\nabla^{2}$ can also act on vector quantities: 
$$\nabla^{2}\vec E = \frac{1}{c^{2}} \frac{\partial^{2} {\vec E}}{\partial {t}^{2}}$$
	- this is *vector calculus*
## plane polar coordinates
$$\frac{\partial^{2} {}}{\partial {x}^{2}} = \left(\cos\theta \frac{\partial }{\partial \rho} - \frac{1}{\rho}\sin\theta \frac{\partial }{\partial \theta}\right)^{2}$$
- **warning:** do not multiply out the bracket, it is the operator syntax
$$\begin{align*}
	\nabla^{2} &= \frac{\partial^{2}}{\partial x}+ \frac{\partial^{2} {}}{\partial {y}^{2}} \\
	&= \left(\frac{\partial^{2}}{\partial {\rho}^{2}} + \frac{1}{\rho} \frac{\partial }{\partial \rho} + \frac{1}{\rho^{2}} \frac{\partial^{2} {}}{\partial {\theta}^{2}}\right)
\end{align*}$$
## spherical polar coordinates
![Pasted image 20241007124450.png](/img/user/pics/Pasted%20image%2020241007124450.png)
$$\nabla^{2} = \frac{\partial^{2} {}}{\partial {r}^{2}} + \frac{2}{r}\frac{\partial }{\partial r}+ \frac{1}{r^{2}} \frac{\partial^{2} {}}{\partial {\theta}^{2}} + \frac{\cos\theta}{r^{2}\sin^{2}\theta} \frac{\partial }{\partial \theta} + \frac{1}{r^{2}\sin^{2}\theta} \frac{\partial^{2} {}}{\partial {\phi}^{2}}$$
