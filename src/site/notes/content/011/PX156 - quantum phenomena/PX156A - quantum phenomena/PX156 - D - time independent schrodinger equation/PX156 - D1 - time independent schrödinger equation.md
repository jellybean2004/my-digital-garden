---
dg-publish: true
---

- [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C1 - the schrodinger equation\|TDSE]]: 
$$i\hbar \frac{\partial}{\partial t} \psi(x,t) = - \frac{\hbar^{2}}{2m} \frac{\partial^{2}}{\partial {x}^{2}}\psi(x,t) + V(x)\psi(x,t)$$
- let $\psi(x,t) = \phi(x)\rho(t):$ 
$$\begin{align*}
	i\hbar \frac{\partial}{\partial t} [\phi(x)\rho(t)] &= - \frac{\hbar^{2}}{2m} \frac{\partial^{2}}{\partial {x}^{2}}[\phi(x)\rho(t)] + V(x)\phi(x)\rho(t) \\
	i\hbar\phi(x) \frac{\partial\rho(t)}{\partial t} &= - \frac{\hbar^{2}}{2m}\rho(t) \frac{\partial^{2}\phi(x)}{\partial {x}^{2}} + V(x)\phi(x)\rho(t) \\
	\frac{i\hbar}{\phi(x)} \frac{\partial\rho(t)}{\partial t} &= - \frac{\hbar^{2}}{2m\phi(x)} \frac{\partial^{2}\phi(x)}{\partial {x}^{2}} + V(x) = E 
\end{align*}$$
- $E$ is constant, hence: 
$$\begin{align*}
	\frac{i\hbar}{\rho} \frac{d\rho}{dt}=E &\implies i\hbar \frac{d\rho}{dt} = E\rho \\
	- \frac{\hbar^{2}}{2m\phi} \frac{d^{2}\phi}{dx^{2}} + V(x) = E &\implies - \frac{\hbar^{2}}{2m} \frac{d^{2}\phi}{dx^{2}} + V\phi = E\phi
\end{align*}$$
- time independent schrödinger equation (TISE):
$$- \frac{\hbar^{2}}{2m} \frac{d^{2}\phi}{dx^{2}} + V\phi = E\phi$$
- for $i\hbar \frac{d\rho}{dt} = E\rho$, the solution is: 
$$\rho(t) = \exp(-\frac{iEt}{\hbar})$$
- solution of the *TISE* depends on the precise form of $V(x)$, but the probability density is given by: 
$$|\psi|^{2}=\phi\phi^{*}\rho\rho^{*} = |\phi|^{2}$$
- hence the probability density is independent of time as $\rho$ is essentially a phase term
- solutions of this type are called *stationary states*
- energy doesn't change with time
- all components of the wave function oscillate with the same well-defined fixed frequency, therefore energy, $E=\hbar\omega$, is constant