---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c4b-postulate-4/"}
---

- when a measurement of a dynamical variable represented by an operator, $\hat Q$, is carried out on a system with a wavefunction, $\psi = \sum_{n}a_{n}\phi_n$,  were $\phi_n$ is an eigenfunction of the operator, then the probability to obtain the result $q_m$ will be $|a_{m|^2}$
- to find the values of the coefficients, $a_{n}:$ 
  $$\begin{align*}
	\int \phi_{n}^{*} \psi \,d\tau &= \int \phi_{n}^{*} \sum\limits_{m}a_{m}\phi_{m}\,d\tau \\
	&= \sum\limits_{m}a_{m} \int\phi_{n}^{*}\phi_{m}\,d\tau \\
	&= \sum\limits_{m}a_{m} \delta_{mn} \\
	\therefore a_{n} &= \int \phi_{n}^{*} \psi \,d\tau
\end{align*}$$
- this is called an **overlap integral**