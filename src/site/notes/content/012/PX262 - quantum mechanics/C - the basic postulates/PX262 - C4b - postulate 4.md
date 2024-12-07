---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c4b-postulate-4/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T15:50:56.040+00:00"}
---

> [!quote] postulate 4
> when a measurement of a dynamical variable represented by the hermitian operator is carried out on a system whose wavefunction is $\psi = \sum_{n}a_{n}\phi_n$, where $\phi_{n}$ are the eigenfunctions of $|hat Q$ corresponding to the eigenvalues $q_n$, then the probability to obtain the result being equal to a particular eigenvalue, $q_m$, will be $|a_{m}|^2$

- to find the values of the coefficients, $a_{n}:$ 
  $$\begin{align*}
	\int \phi_{n}^{*} \psi \,d\tau &= \int \phi_{n}^{*} \sum\limits_{m}a_{m}\phi_{m}\,d\tau \\
	&= \sum\limits_{m}a_{m} \int\phi_{n}^{*}\phi_{m}\,d\tau \\
	&= \sum\limits_{m}a_{m} \delta_{mn} \\
	\therefore a_{n} &= \int \phi_{n}^{*} \psi \,d\tau
\end{align*}$$
- this is called an **overlap integral**, which is the measurement of the extent to which the two functions are similar
- 