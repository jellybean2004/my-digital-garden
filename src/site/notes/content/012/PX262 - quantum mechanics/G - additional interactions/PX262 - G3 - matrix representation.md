---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/g-additional-interactions/px-262-g3-matrix-representation/","noteIcon":"1","created":"2024-11-25T11:21:45.798+00:00","updated":"2024-12-19T18:52:10.889+00:00"}
---

- taking a dynamical variable, $\hat Q$, with an eigenstate, $\psi$, with eigenvalue, $q:$
$$\hat Q \psi = q\psi$$
- expanding $\psi$ in terms of some complete orthonormal set of functions, $\phi_n$ which may not necessarily be eigenfunctions of $\hat Q:$
$$\psi = \sum\limits_{n}a_{n}\phi_{n}$$
- applying $\hat Q:$
$$\sum\limits_{n} a_{n} \hat Q \phi_{n} = q \sum\limits_{n}a_{n}\phi_{n}$$
- multiplying it by the $\phi_m^*$ and integrating over all space:
$$\begin{gather*}
\int \sum\limits a_{n} \phi_{m}^{*}\hat Q \phi_{n} \,d\tau = q \int \sum\limits_{n} a_{n}\phi_{m}^{*} \phi_{n}\,d\tau  = q a_{m} \\\\
\therefore \sum\limits_{n}Q_{mn}a_{n} = qa_{m}
\end{gather*}$$
	where,
	$$Q_{mn}= \int \phi_{m}^{*} \hat Q \phi_{n}\,d\tau$$
- expressing as matrices:
$$\begin{pmatrix}Q_{11} & Q_{12} &\dots \\ Q_{21} & Q_{22} & \dots \\ \vdots & \vdots & \ddots \end{pmatrix} \begin{pmatrix} a_{1} \\ a_{2} \\ \dots \end{pmatrix} = q \begin{pmatrix} a_{1} \\ a_{2} \\ \dots \end{pmatrix}$$
- matrices still obey the same commutation relations
- replacing complex conjugate by hermitian conjugate, $A^{\dagger} = A^{T*}$

- matrix representation is helpful for:
	- working with spin
	- numerical calculations
