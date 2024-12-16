---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c2a-the-dynamical-variables/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T14:11:18.581+00:00"}
---

 - **dynamical variables**: position, momentum, energy, etc
- in **classical physics**, they are represented by algebraic variables: ${} x$, $p_x$, $E$, which can have all possible (continuous) values

- in **quantum mechanics**, only some values are allowed
- this also needs to work together with the wavefunction to obtain information
## operators
- from the [[content/012/PX262 - quantum mechanics/B - introduction/PX262 - B2 - time-independent schrödinger equation\|time independent schrödinger equation]]: 
$$\begin{gather*}
	\left[- \frac{\hbar^{2}}{2M} \vec\nabla^{2}+ V(\vec r)\right]\mu  = E\mu \\
	\hat H \mu = E \mu
\end{gather*}$$
	where, $\hat H$ is the hamiltonian (energy) operator

- a **mathematical operator** is an object which acts on a function and produces a new function, which need not be the same function
- in the above case, the same function is obtained
- the special cases are called eigenfunctions, and the values of $E$ are called eigenvalues:
	  $\hat H =$ operator
	  $\mu =$ eigenfunction
	  $E=$ eigenvalue
- eigenfunctions correspond to the single eigenvalue of the system
- if there is a system described by the eigenfunction of the given operator, and measurements of the corresponding variable is taken, the given eigenvalue is obtained
- it is reasonable to expect that if a second measurement is taken, the same answer is obtained
- if the measurement of a given value is obtained, the wavefunction immediately after the measurement should be the corresponding eigenfunction ($\phi_{n}$)

- the dynamical variables are represented by operators, and the eigenvalues of these operators correspond to the possible measurement outcomes

### hermitian
- if $\hat Q$ is a hermitian operator: 
  $$\int f\,\hat Q\,g \,d\tau = \int g\,\hat Q^{*}\,f\,d\tau$$
	where $f$ and $g$ are well-defined functions that vanish at infinity
- the momentum operator: $$\begin{align*}
	\int f \hat P_{x} g \,d\tau &= -i\hbar \int_{-\infty}^{\infty} f \frac{\partial g}{\partial x}\,dx \\
	&= -i\hbar \left( [fg]_{-\infty}^{\infty}- \int_{-\infty}^{\infty} g \frac{\partial f}{\partial x}\,dx \right) \\
	&= + i\hbar \int_{-\infty}^{\infty} g \frac{\partial f}{\partial x}\,dx \\
	\therefore \int f \hat P_{x} g \,d\tau &= \int_{-\infty}^{\infty} g \hat P_{x}^{*} f\,dx
\end{align*}$$
