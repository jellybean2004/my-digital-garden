---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/g-measurement-of-angular-momentum/px-262-g3-matrix-representation/","created":"2024-11-25T11:21:45.798+00:00","updated":"2024-11-27T23:06:59.497+00:00"}
---

- taking a dynamical variable, $\hat Q$, and adding the state, $\psi$, which has an eigenvalue, ${} q: {}$
$$\hat Q \psi = q\psi$$
- suppose eigenfunctions of some operator (can be different from $\hat Q$), $\phi_n$
$$\psi = \sum\limits_{n}a_{n}\phi_{n}$$
- applying $\hat Q:$
$$\begin{align*}
\sum\limits_{n} a_{n} \hat Q \phi_{n} &= q \sum\limits_{n}a_{n}\phi_{n}\\
\int \sum\limits a_{n} \phi_{m}^{*}\hat Q \phi_{n} \,d\tau &= q \int \sum\limits_{n} a_{n}\phi_{m}^{*} \phi_{n}\,d\tau = q a_{m} \\
\sum\limits_{n}Q_{mn}a_{n} &= qa_{m}
\end{align*}$$
	where,
	$$Q_{mn}= \int \phi_{m}^{*} \hat Q \phi_{n}\,d\tau$$
- expressing as matrices:
$$\begin{pmatrix}Q_{11} & Q_{12} &\dots \\ Q_{21} & Q_{22} & \dots \\ \vdots & \vdots & \ddots \end{pmatrix} \begin{pmatrix} a_{1} \\ a_{2} \\ \dots \end{pmatrix} = q \begin{pmatrix} a_{1} \\ a_{2} \\ \dots \end{pmatrix}$$
- matrices still obey the same commutation relations
- replacing complex conjugate by hermitian conjugate, ie: $A^{\dagger} = A^{T*}$
- a few places where matric representation is widely used:
	- spin
	- numerical calculations
