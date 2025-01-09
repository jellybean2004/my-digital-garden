---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/h/px-262-h2-quantum-mechanics-and-many-particles/","noteIcon":"1","created":"2025-01-06T19:08:47.143+00:00","updated":"2025-01-09T17:18:32.636+00:00"}
---

- in classical mechanics, for several particles $(N)$, the kinetic and the potential energies are given by:
$$\begin{gather}
	T = \sum\limits_{i=1}^{N} \frac{p_{i}^{2}}{2m_{i}} \\\\
	V = V(\vec r_{1},  \vec r_{2}, \dots)
\end{gather}$$
- in quantum mechanics, the system is defined by a wavefunction, which is a function of the positions and spins of the particles:
$$\psi(\vec r_{1}, \sigma_{1} ; \vec r_{2}, \sigma_{2}; \dots \vec r_{N ,}\sigma_{N}, t)$$
- it must satisfy the schrödinger equation:
$$\hat H \psi = i \hbar \frac{\partial \psi}{\partial t}$$
- $\hat H$ is the hamiltonian operator:
$$\hat H = \sum\limits_{i=1}^{N }\left(\frac{\hat{p}_{i}^{2}}{2m} + \hat V\right)$$
	where, $\hat p_{i} = - i\hbar \vec\nabla$ is the momentum operator

- for identical particles, $\psi$ is either symmetric or antisymmetric

- it is symmetric when the coordinates of any two particles are swapped if they are bosons (eg: $\pi$-mesons, phonons, photons, etc)
$$\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{a}, \sigma_{a};\dots \dots\vec r_{b}, \sigma_{b}; \dots \vec r_{N ,}\sigma_{N}, t) = \psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{b}, \sigma_{b};\dots \dots\vec r_{a}, \sigma_{a}; \dots \vec r_{N ,}\sigma_{N}, t)$$
- and it is antisymmetric when the particles are fermions (eg: electrons, protons, etc)
$$\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{a}, \sigma_{a};\dots \dots\vec r_{b}, \sigma_{b}; \dots \vec r_{N ,}\sigma_{N}, t) = -\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{b}, \sigma_{b};\dots \dots\vec r_{a}, \sigma_{a}; \dots \vec r_{N ,}\sigma_{N}, t)$$

- this captures the **pauli exclusion principle:** no two electrons can occupy the same state

- eg: putting several non-interacting electrons in a box (1D)
- the single electron is bound by: $0<x<L$
- the energy is given by:
$$- \frac{\hbar}{2m} \frac{d^{2}}{dx^{2}} \phi(x) = E \phi(x)$$
- the solutions are in the form: 
$$\phi(x) = Ae^{ikx} + B e^{-ikx} = C\cos(kx) + D\sin(kx)$$

- trapping the electron in the box:
	$\phi(0) = 0 \implies C = 0$
	$\phi(L) = 0 \implies kL = n\phi$, $n\in\mathbb{Z}$
- therefore, the wavenumbers:
$$k_{n} = \frac{n\pi}{L}$$
- and the energies:
$$E+n  = \frac{\hbar}{2m_{e}}\left(\frac{n\pi}{L}\right)^{2}$$
- the states:
$$\phi_{n} = D\sin\left(\frac{n\pi x}{L}\right)$$

![PX262 - H2 - quantum mechanics and many particles.png|500](/img/user/pics/PX262%20-%20H2%20-%20quantum%20mechanics%20and%20many%20particles.png)

- the ground state energy, $E_g$, for a system of several electrons, using the pauli exclusion principle:
$$E_{g} = E_{1} + E_{1} + E_{2} + E_{2} + \dots$$
	where, the two $E_1$ terms are for spin $\uparrow$ and spin $\downarrow$
