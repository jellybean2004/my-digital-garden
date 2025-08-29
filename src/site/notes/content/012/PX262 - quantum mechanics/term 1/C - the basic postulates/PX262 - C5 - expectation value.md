---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/c-the-basic-postulates/px-262-c5-expectation-value/","noteIcon":"1","created":"2025-08-27T13:14:15.840+01:00","updated":"2024-11-26T01:07:23.000+00:00"}
---

-  when measurements of a dynamical variable represented by the operator, $\hat Q$, are repeated on identical copies of a system, the average value obtained is called the expectation value
- the prediction for the expectation value is: 
$$\begin{align*}
	\langle{\hat Q}\rangle &= \int \psi^{*} \hat Q \psi \,d\tau \\ 
	&= \int \left(\sum\limits_{m}a_{m}^{*} \phi_{m}^{*}\right) \hat Q \left(\sum\limits_{n}a_{n} \phi_{n} \right) \,d\tau \\
	&= \sum\limits_{m,n} a_{m}^{*}a_{n}q_{n} \int \phi_{m}^{*}\phi_{n}\,d\tau \\
	&= \sum\limits_{m,n} a_{m}^{*}a_{n}q_{n}\,\delta_{mn} \\
	&= \sum\limits_{n} a_{n}^{*}a_{n}q_{n} \\
	\therefore \langle{\hat Q}\rangle &= \sum\limits_{n}|a_{n}|^{2} q_{n}
\end{align*}$$
- the standard deviation can be defined as: 
  $$\sqrt{\delta Q} = \sqrt{\langle{\hat Q^{2}}\rangle - \langle{\hat Q}\rangle^{2}}$$
