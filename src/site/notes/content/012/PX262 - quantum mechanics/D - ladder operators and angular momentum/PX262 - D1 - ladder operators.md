---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/d-ladder-operators-and-angular-momentum/px-262-d1-ladder-operators/"}
---

- the hamiltonian operator: 
  $$\hat H = \frac{\hat{P}^{2}}{2m} + \frac{1}{2}m \omega^{2} \hat X^{2}$$
- the position, $x$, can be measured in the units $(\frac{\hbar}{m\omega})^{\frac{1}{2}}$, the momentum units are $(m\hbar\omega)^\frac{1}{2}$, and the energy units are $\hbar\omega$
- the expression for the energy of a given state becomes: 
  $$E_{n}= \frac{1}{2}+ n$$
- the hamiltonian operator is: 
  $$\hat H = \frac{1}{2}(\hat P ^{2}+\hat X^{2})$$
- the commutation relation: 
  $$[\hat P , \hat X] = -i$$
- the ladder operators are defined as: 
  $$\begin{align*}
	\hat R_{+} &= (\hat P + i \hat X) \\
	\hat R_{-} &= (\hat P - i \hat X)
\end{align*}$$
$$\begin{align*}
	\hat R_{+} \hat R_{-} &= (\hat P + i \hat X) (\hat P - i \hat X) \\
	&= \hat P^{2} + \hat X^{2} + i\hat X \hat P - i \hat P \hat X \\
	&= 2\hat H - i [\hat P, \hat X] \\
	\hat R_{+} \hat R_{-}&= 2\hat H - 1 \\\\
	\text{similarly, } \hat R_{-} \hat R_{+}&= 2\hat H + 1 
\end{align*}$$
- the hamiltonian operator can rewritten as: 
  $$\hat H = \frac{1}{2} (\hat R_{+}\hat R_{-} + 1) = \frac{1}{2} (\hat R_{-}\hat R_{+} - 1)$$
- commutation relations of the ladder operators with hamiltonian: 
  $$\begin{gather}
	[\hat R_{+}, \hat H] = \hat R_{+} \frac{1}{2}(\hat R_{-}\hat R_{+} -1) - \frac{1}{2}(\hat R_{+}\hat R_{-} + 1) \hat R_{-} = - \hat R_{+} \\\\
	[\hat R_{-}, \hat H] = + \hat R_{-}
\end{gather}$$
- applying $\hat R_{+}$ to some eigenfunction, $\phi_n$, and working out the energy of the resulting wavefunction: 
  $$\hat H \hat R_{+} \phi_{n} = \hat R_{+} \hat H \phi_{n} + \hat R_{+} \phi_{n} = \hat R_{+}E_{n}\phi_{n}+ \hat R_{+} \phi_{n} = (E_{n}+1)\hat R_{+}\phi_{n}$$
- this shows that the wavefunction, $\hat R \phi_{n}$, is an eigenfunction of the hamiltonian operator, with the eigenvalue, $E_{n}+1$
$$E_{n}+1 = n + 1 + \frac{1}{2} = E_{n+1}$$
- this shows that the result pf applying $\hat R_{+}$ on $\phi_n$ is $\phi_{n+1}$
- similarly, 
  $$\hat H \hat R_{-}\phi_{n} = (E_{n}-1) \hat R \phi_{n} = E_{n-1}\phi_{n-1}$$
- the two operators help move up and down the ladder of states, where each step is a particular energy eigenstate, hence called *ladder operators*
- if $\hat R_{-}$ is applied on the ground state, $\phi_0$ should get to zero because it is not possible to move any lower: 
  $$0 = \hat R_{+}\hat R_{-}\phi_{0} = (2\hat H -1) \phi_{0} = (2E_{0}-1)\phi_{0} \implies E_{0} = \frac{1}{2}$$
- this shows that the lowest energy state has an energy: $E_{0}=\frac{1}{2}\hbar \omega$
