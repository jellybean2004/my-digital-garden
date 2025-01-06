---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/px-262-h2-quantum-mechanics-and-many-particles/","noteIcon":"1","created":"2025-01-06T19:08:47.143+00:00","updated":"2025-01-06T19:27:15.368+00:00"}
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
- $\hat H$ is the hamiltonian:
$$\hat H = \sum\limits_{i=1}^{N }\left(\frac{\hat{p}_{i}^{2}}{2m} + \hat V\right)$$
	where, $\hat p_{i} = - i\hbar \vec\nabla$ is the momentum operator

- for identical particles, $\psi$ is either symmetric or antisymmetric

- it is symmetric when the coordinates of any two particles are swapped if they are bosons (eg: $\pi$-mesons, phonons, photons, etc)
$$\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{a}, \sigma_{a};\dots \dots\vec r_{b}, \sigma_{b}; \dots \vec r_{N ,}\sigma_{N}, t) = \psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{b}, \sigma_{b};\dots \dots\vec r_{a}, \sigma_{a}; \dots \vec r_{N ,}\sigma_{N}, t)$$
- and it is antisymmetric when the particles are fermions (eg: electrons, protons, etc)
$$\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{a}, \sigma_{a};\dots \dots\vec r_{b}, \sigma_{b}; \dots \vec r_{N ,}\sigma_{N}, t) = -\psi(\vec r_{1}, \sigma_{1} ; \dots\vec r_{b}, \sigma_{b};\dots \dots\vec r_{a}, \sigma_{a}; \dots \vec r_{N ,}\sigma_{N}, t)$$

- this captures the **pauli exclusion principle:** no two electrons can occupy the same state
