---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/f-3-d-systems/px-262-f1-the-schroedinger-equation-in-3-d/","noteIcon":"1","created":"2025-08-27T13:14:15.878+01:00","updated":"2024-12-15T11:25:08.000+00:00"}
---

## time-dependent
- the time-dependent schrödinger equation in 3D is:
  $$i \hbar \frac{\partial \psi}{\partial t} = - \frac{\hbar^{2}}{2m} \nabla^{2} \psi + V(\vec r) \psi = \hat H \psi \tag{1}$$
	where, 
		$\nabla^{2} = \left( \frac{\partial^{2}}{\partial {x}^{2}} + \frac{\partial^{2}}{\partial {y}^{2}} + \frac{\partial^{2}}{\partial {z}^{2}}\right)$ ,
		$\hat H = \left(- \frac{\hbar^{2}}{2m} \nabla^{2} + \hat V\right)$ is the hamiltonian operator
## time-independent
- considering the cases of time-independent potential, $V(\vec r)$
- using separation of variables in the wavefunction: 
  $$\psi (\vec r, t) = \mu (\vec r) T(t)$$
- substituting it into equation $(1):$ 
$$\begin{gather*}
	\mu(\vec r) i\hbar \frac{\partial T(t)}{\partial t} = T(t)\hat H \mu(\vec r) \\
	\frac{i\hbar}{T(t)} \frac{\partial T(t)}{\partial t} = \frac{1}{\mu(\vec r)}\hat H \mu(\vec r) = E
\end{gather*}$$
- the time-dependent part is: 
  $$\frac{i\hbar}{T(t)} \frac{\partial T(t)}{\partial t} = E \implies T(t) = \exp\left(-\frac{iEt}{\hbar}\right)$$
\1\n\2\n