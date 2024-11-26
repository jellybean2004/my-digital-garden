---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/b-introduction/px-262-b2-time-independent-schroedinger-equation/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T01:06:39.387+00:00"}
---

- for systems in which the potential is independent of time$:V(x,t)=V(x)$
$$\begin{align*}
	\psi(x,t) &= \phi(x)\,T(t) \\\\
	i\hbar \frac{\partial }{\partial t}[\phi(x)T(t)] &= \frac{-\hbar^{2}}{2M} \frac{\partial ^{2}}{\partial x^{2}}[\phi(x)T(t)] + V(x)\phi(x)T(t) \\
	\phi i\hbar \frac{\partial T}{\partial t} &= -\frac{\hbar^{2}}{2M} T \frac{\partial ^{2}\phi}{\partial x^{2}} + V\phi T \\
	\frac{i\hbar}{T} \frac{\partial T}{\partial t} &= -\frac{\hbar^{2}}{2M} \frac{1}{\phi} \frac{\partial ^{2}\phi}{\partial x^{2}} + V\\
\end{align*}$$
- $LHS$ depends only on time, and $RHS$ depends only on position
- each side has to be constant
- $LHS:$ 
$$\begin{align*}
	i\hbar \frac{dT}{dt} &= E\,T \\
	\implies T(t) &= \exp\left(\frac{-iEt}{\hbar}\right)
\end{align*}$$
	- universal time dependence in systems where potential is time independent
- $RHS:$ 
  $$- \frac{\hbar^{2}}{2M} \frac{d^{2}\phi}{dx^{2}} + V\phi = E\phi$$
	- this is the time independent schrödinger equation
- for a free particle, ${} V(x)=0:$ 
  $$\phi(x) = A\exp(ikx)$$
	where, $k=\sqrt{\frac{2ME}{\hbar^2}}$
- full wave function: 
  $$\psi(x,t) = A\exp[-(kx-\omega t)]$$
