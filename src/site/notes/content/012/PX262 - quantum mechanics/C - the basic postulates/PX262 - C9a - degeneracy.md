---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c9a-degeneracy/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-15T15:05:06.575+00:00"}
---

- in the case of [[content/012/PX262 - quantum mechanics/C - the basic postulates/PX262 - C3 - orthonormality\|orthonormality]], it was assumed that all eigenvalues are different, which is not always true
- in a degenerate system there can be multiple states with distinct eigenfunctions with the same eigenvalue of a given dynamical variable, ie: $q_{m}= q_{n}$ for $\hat Q \phi_{n}= q_{n}\phi_n$ and $\hat Q \phi_{m}= q_{m}\phi_{m}$
- there are two places where the arguments go wrong:
	- [[content/012/PX262 - quantum mechanics/C - the basic postulates/PX262 - C3 - orthonormality\|orthonormality]]
	- [[content/012/PX262 - quantum mechanics/C - the basic postulates/PX262 - C6b - compatibility of operators\|compatibility of operators]]

- in [[content/012/PX262 - quantum mechanics/C - the basic postulates/PX262 - C3 - orthonormality\|orthonormality]], the following equation was obtained:
$$(q_{m}-q_{n}) \int \phi_{m}^{*} \phi_{n}\,d\tau = 0$$
- by the fact that there are different eigenvalues $(q_{m} \neq q_{n})$, it was concluded: 
  $$\int \phi_{m}^{*} \phi_{n}\,d\tau = 0\; \text{for } m\neq n$$
  
- in case of degeneracy, ${} q_{m} = q_{n} {}$ for $m\neq n$, so the **integral may be non-zero**
- if there are several eigenfunctions, $\phi_{n}$, with the same eigenvalue, $q$, it can be used to create another wavefunction as a linear superposition, eg: $\psi = \sum\limits_{n} c_{n}\phi_{n}$
- the outcome of measurement of a quantity can be evaluated as: 
  $$\hat Q \sum\limits_{n}c_{n}\phi_{n} = \sum\limits_{n}c_{n}\hat Q \phi_{n} = q \sum\limits_{n}c_{n}\phi_{n} = q\psi$$
- this shows that $\psi$ is an eigenfunction of $\hat Q$, with the same eigenvalue, $q$
- to check for orthogonality: 
  $$\int \phi_{m}^{*}\psi\,d\tau = \int \phi_{m}^{*}\sum\limits_{n}c_{n}\phi_{n} \,d\tau = \sum\limits_{n}c_{n} \int \phi_{m}^{*}\phi_{n} \,d\tau = \sum\limits_{n}c_{n} \delta_{mn} = c_{m}$$
- thus, none of the eigenfunctions used to construct $\psi$ is orthogonal to $\psi$

- while in general, the linear combination of eigenfunctions is not an eigenfunction, if the eigenfunctions are degenerate, it will be
