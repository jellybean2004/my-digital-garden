---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/m-basic-postulates-revisited/px-262-m2-recap/","noteIcon":"1","created":"2025-08-27T13:15:23.260+01:00","updated":"2025-02-27T10:32:02.000+00:00"}
---

- the wavefunction, $\psi(x,t)$, contains all the information about the system
- the behaviour is governed by the schrödinger equation:
$$i\hbar \frac{\partial \psi}{\partial t} = \hat H \psi$$
	where, $\hat H$ is the hamiltonian
$$\hat H \phi_{n}(x) = E_{n} \phi_{n} (x)$$
	where, $\phi_{n}$ and $E_{n}$ are the eigenfunctions and eigenvalues of the hamiltonian
$$\psi(x,t) = \sum\limits_{n} c_{n}\phi_{n}(x) \exp\left(\frac{-iE_{n}t}{\hbar}\right)$$
- for an observable, $A$, described by an operator, $\hat A$, there will be eigenfunctions, $u_{a}(x)$, corresponding to real eigenvalues, ${} \lambda_{a}: {}$
$$\hat A u_{a}(x) = \lambda_{a} u_{a}(x)$$
$$\int u_{a_{1}}^{*}(x') \, u_{a_{2}}(x')\,dx' = \delta_{a_{1},a_{2}} = \begin{cases} 1 & a_{1} = a_{2},\\ 0 & a_{1} \neq a_{2}.\end{cases}$$
- any function, $g(x) = \sum\limits_{a} c_{a} u_{a}(x)$ (complete set)
$$c_{a} = \int u_{a}^{*} (x' ) \, g(x') \, dx'$$
- if a system is described by the wavefunction, $\psi(x)$, measuring $A$ will give one of the eigenvalues, $\lambda_a$, with probability:
$$P(\lambda_{a}) = c_{a}^{*} c_{a} = |c_{a}|^{2}$$
	where, $\psi(x) = \sum\limits_{n} c_{a} u_{a}(x)$
- it can be written as:
$$\psi(x) = \sum\limits_{a}\int u_{a}^{*} (x') \, \psi(x')\, dx' \, u_{a}(x)$$
- to show: $\sum\limits_{a} u_{n}(x) u_{a}^{*}(x') = \delta(x-x')$, ie: $\psi(x) = \int \delta(x-x') \psi(x')\,dx'$
- from $\int \psi^{*}\psi\,dx = 1:$
$$\begin{align*}
&= \int\sum\limits_{a} c_{a}^{*} u_{a}^{*}(x) \psi(x)\,dx  \\
&= \sum\limits_{a}c_{a}^{*} c_{a} \\
&= \sum\limits_{a}P(\lambda_{a}) \\
&= 1
\end{align*}$$

## vector space analogy
- thinking of  vector in 3D space: $$\vec v = v_{x} \hat i + v_{y}\hat j + v_{z} \hat k$$
- the unit vectors satisfy: $\hat i \cdot \hat j = \hat j \cdot \hat k = \hat k \cdot \hat i = 0$ and $\hat i \cdot \hat i = \hat j \cdot \hat j = \hat k \cdot \hat k= 1$
- the scalar products: $v_{x} = \vec v \cdot \hat i$, $v_{y} = \vec v \cdot \hat j$ and $v_{z} = \vec v \cdot \hat k$
- $v_x$, $v_y$ and $v_{z}$ are analogs of $c_{a}$'s
- the projection of $\psi(x)$ along a basis 'vector', $u_a(x)$, is $c_{a}:$
$$c_{a}= \int u_{a}^{*} (x') \psi(x')\,dx'$$
- ie. the 'scalar product' of $u_{a}(x)$ and $\psi(x)$
$$\begin{gather}
\vec v = \sum\limits_{i} v_{i}\, \hat e_{i} \\
\psi(x) = \sum\limits_{a}c_{a} \, u_{a}(x)
\end{gather}$$
- a 'vector space' in quantum mechanics is called a **hilbert space**
