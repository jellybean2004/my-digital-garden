---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/c-the-basic-postulates/px-262-c3-orthonormality/","noteIcon":"1","created":"2025-08-27T13:14:15.830+01:00","updated":"2024-12-07T14:40:06.000+00:00"}
---

- orthonormality is an important property of hermitian operators: 
  $$\int \phi_{m}^{*} \phi_{n}\,d\tau = \delta_{mn} = \begin{cases} 1 & \text{for }m = n \\ 0 & \text{for }m\neq n\end{cases}$$
	where, $\delta_{mn}$ is **kronecker delta**
$$\begin{gather}
	\hat Q \phi_{n}= q_{n}\phi_{n} \\\\
	\int \phi_{n}^{*} \hat Q \phi_{m}\,d\tau = q_{m}\int \phi_{n}^{*} \phi_{m}\,d\tau \\
	\int \phi_{m} \hat Q^{*} \phi_{n}^{*}\,d\tau = q_{n}\int \phi_{m}\phi_{n}^{*}\,d\tau \\
\end{gather}$$
- if $\hat Q$ is hermitian, the two integrals on the $LHS$ must be the same, so: 
  $$\text{either, } q_{m}= q_{n}, \;\text{or, }\; \int\phi_{n}^{*}\phi_{m}\,d\tau = 0 \;\text{for } m\neq n$$
- this implies that the eigenfunctions are **degenerate**, ie. they correspond to the same eigenvalue
