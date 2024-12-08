---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c9a-degeneracy/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-08T13:08:40.925+00:00"}
---

- it was assumed that all eigenvalues are different, which is not always true
- in a degenerate system there can be multiple states with distinct eigenfunctions with the same eigenvalue of a given dynamical variable
- there are two places where the arguments go wrong:
	- orthogonality
	- compatibility of measurements
## orthogonality
- by the fact that there are different eigenvalues, it was concluded that: 
  $$\int \phi_{m}^{*} \phi_{n}\,d\tau = 0\; \text{for } m\neq n$$
- this was implied from the equation: 
  $$(q_{m}-q_{n}) \int \phi_{m}^{*} \phi_{n}\,d\tau = 0$$
- in case of degeneracy, $m\neq n$ , but $q_{m}=q_{n}$, so the integral may be non-zero
- if there are several eigenfunctions, $\phi_{n}$, with the same eigenvalue, $q$, it can be used to create another wavefunction as a linear superposition, eg: $\psi = \sum\limits_{n} c_{n}\phi_{n}$
- the outcome of measurement of a quantity can be evaluated as: 
  $$\hat Q \sum\limits_{n}c_{n}\phi_{n} = \sum\limits_{n}c_{n}\hat Q \phi_{n} = q \sum\limits_{n}c_{n}\phi_{n} = q\psi$$
- this shows that $\psi$ is an eigenfunction of $\hat Q$, with the same eigenvalue, $q$
- to check for orthogonality: 
  $$\int \phi_{m}^{*}\psi\,d\tau = \int \phi_{m}^{*}\sum\limits_{n}c_{n}\phi_{n} \,d\tau = \sum\limits_{n}c_{n} \int \phi_{m}^{*}\phi_{n} \,d\tau = \sum\limits_{n}c_{n} \delta_{mn} = c_{m}$$
- thus, none of the eigenfunctions used to construct $\psi$ is orthogonal to $\psi$

- while in general, the linear combination of eigenfunctions is not an eigenfunction, if the eigenfunctions are degenerate, it will be
## schmidt orthogonalization
- a way of restoring orthogonality
- considering  $\phi_{1}$ and $\phi_{2}$, which are not orthogonal, but have the same eigenvalue
- defining a new eigenfunction, which is a linear combination of the two: 
  $$\phi_{2}' = S_{12}\phi_{1}- \phi_{2}$$
	where ${} S_{12} = \int \phi_{1}^{*} \phi_{2}\,d\tau$
- checking if the new function is orthogonal to $\phi_{1}:$ 
$$\begin{align*}
	\int \phi_{1}^{*} \phi_{2}' \,d\tau &= S_{12}\int \phi_{1}^{*}\phi_{1} \,d\tau- \int\phi_{1}^{*}\phi_{2}\,d\tau \\
	&= S_{12} - S_{12} \\
	&= 0 
\end{align*}$$
- this shows that $\phi_{1}$ and $\phi_{2}'$ are orthogonal

- if there is another eigenfunction, $\phi_{3}$, with the same eigenvalue: 
  $$\phi_{3}' = s_{13}\phi_{1}+ s_{23}\phi_{2}' - \phi_{3}$$
	where, ${} s_{13} = \int \phi_{1}^{*}\phi_{3}\,d\tau {}$, and $s_{23}= \frac{\int\phi_{2}'^{*}\phi_{3}\,d\tau}{\int|\phi_{2}'|^{2}\,d\tau}$
- the factors, $s_{12}$, $s_{13}$, and $s_{23}$ are called overlap integrals
- if there are further degenerate states, the process can be continued until a full set of orthogonal functions is obtained
