---
dg-publish: true
---

- in classical physics, the order of dynamical variables does not matter, as they commute
- this is not the case in quantum mechanics
- consider the position and momentum operators: 
$$\begin{align*}
	(\hat P_{x}\hat X - \hat X \hat P_{x}) \psi &= -i\hbar \frac{\partial}{\partial x}(x\psi) - x \left(-i\hbar \frac{\partial \psi}{\partial x}\right) \\
	&= -i\hbar \left(\psi +x \frac{\partial \psi}{\partial x}\right) + i\hbar x\frac{\partial \psi}{\partial x} \\
	&= -i\hbar \psi
\end{align*}$$
- it can be seen that the operation is independent of the wavefunction itself
- the commutator can be written as: 
$$[\hat P_{x}, \hat X] = \hat P_{x}\hat X - \hat X \hat P_{x}= -i \hbar$$
- extending it to 3D: 
$$\begin{gather}
	[\hat X_{i},\hat X_{j}] =[\hat P_{i}, \hat P_{j}] = 0 \\
	[\hat P_{i},\hat X_{j}] = - [\hat X_{j}, \hat P_{i}] = -i\hbar \,\delta_{ij}
\end{gather}$$
- **note:** these commutators are fundamental in quantum mechanics
- the form of the operators, ${} \hat P_{i} {}$, $\hat X$, are not unique
- the representation used here is called *positional representation*
- a few useful identities: 
	$[\hat A, \hat B] = -[\hat B, \hat A]$
	$[\hat A, \hat B \hat C] = [\hat A, \hat B] + [\hat A, \hat C]$
	$[\hat A, \hat B, \hat C] = [\hat A, \hat B]\hat  C + \hat  B [\hat A, \hat  C]$
		$\hat A\hat B\hat C - \hat B\hat C\hat A + \hat B\hat A\hat C - \hat B\hat A\hat C = \hat B[\hat A,\hat C] + [\hat A,\hat B]\hat C$
## compatibility of operators
- if two operators commute, they are called *compatible operators*
- for two compatible operators, $\hat Q, \hat R$ and a generic wave function: $\psi = \sum_{n}a_{n}\phi_{n}$
- take $\phi_{n}$ to be the eigenstate of $\hat Q:$ $\hat Q\hat R \phi_{n} = \hat R \hat  Q \phi_{n} = \hat R q_{n}\phi_{n} = q_{n}\hat R\phi_{n}$
- so, if operators are compatible, then $\hat R\phi_{n}$ is an eigenfunction of $\hat Q$ 