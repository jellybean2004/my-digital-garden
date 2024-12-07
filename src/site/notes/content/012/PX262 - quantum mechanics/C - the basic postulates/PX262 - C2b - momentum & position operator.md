---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c2b-momentum-and-position-operator/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T14:18:58.266+00:00"}
---

## momentum operator
- the kinetic energy, classically given as $T = \cfrac{p^{2}}{2M}$, can we written as:
$$T = \frac{1}{2M} \hat p^{2} = - \frac{\hbar^{2}}{2M}\nabla^{2}$$
	where, $\hat p$ is the momentum operator
- the momentum operator in vector form: 
$$\begin{gather}
	\hat{\vec{p}} = -i\hbar \vec\nabla \\
	\hat p_{x}= -i\hbar \frac{\partial }{\partial x}
\end{gather}$$
- the eigenvalues and eigenfunctions of the momentum operator: 
  $$-i\hbar \frac{\partial }{\partial x} \phi = p\phi$$
- the solutions are plane waves: $\phi = A \exp(ikx)$, where $k= \frac{p}{\hbar}$
- if $V(\vec r)\neq 0:$ eigenfunctions of $\hat H$ and $\hat p$ are not the same
## position operator
$$\hat x \phi = x_{0}\phi$$
- the eigenfunctions in this case are non-zero at a given position, and zero everywhere else $\implies \delta(x-x_{0}):$ 
  $$\hat x \, \delta(x-x_{0}) = x_{0}\,\delta(x-x_{0})$$
- above is satisfied by $\hat x = x$
- back to the hamiltonian operator: 
  $$\hat H = - \frac{\hbar^{2}}{2m} \vec\nabla^{2}+ V(\vec r)$$
- it can be constructed using the momentum and the position operators
- the relation between $\hat H$, and $\hat p, \hat x$ is the same as in classical physics

- only hermitian operators can be used
- the operators can be complex, but the measurements have to be real
- if two well behaved functions, $f,g$, are taken, then the hermitian operator satisfies: 
  $$\int f \hat Q g\,d\tau = \int g \hat Q^{*} f d\tau$$
	where, $\hat Q$ is the operator 
- eigenvalues: 
		$\hat Q \phi_{n} = q_{n}\phi_{n}$
		${} \hat Q^{*} \phi_{n}^{*} = q_{n}^{*}\phi_{n}^{*} {}$
	- multiplying by the complex conjugate:
		$\phi_{n}^{*} \hat Q \phi_{n} = \phi_{n}^{*} q_{n} \phi_{n}$
		${} \phi_{n} \hat Q^{*} \phi_{n}^{*} = \phi_{n} q_{n}^{*} \phi_{n} {}$
	- integrating:
		$\int \phi_{n}^{*} \hat Q \phi_{n} d \tau = \int \phi_{n}^{*} q_{n} \phi_{n} d\tau = q_{n}$
		$\int \phi_{n} \hat Q ^{*}\phi_{n}^{*}\, d\tau = \int \phi_{n} q_{n}^{*} \phi_{n}\,d\tau = q_{n}^{*}$
- from the definition of hermitian operators, the two integrals on the $LHS$ are the same, and therefore $q_{n} = q_{n}^{*} \implies q_{n}\in \mathbb R$
