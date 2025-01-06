---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/c-the-basic-postulates/px-262-c6a-commutation-relations/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-15T15:03:57.861+00:00"}
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
- the form of the operators, $\hat P_{i}$, $\hat X$, are not unique
- the representation used here is called *positional representation*
- a few useful identities: 
	$[\hat A, \hat B] = -[\hat B, \hat A]$
	$[\hat A, \hat B \hat C] = [\hat A, \hat B] + [\hat A, \hat C]$
	$[\hat A, \hat B, \hat C] = [\hat A, \hat B]\hat  C + \hat  B [\hat A, \hat  C]$
		$\hat A\hat B\hat C - \hat B\hat C\hat A + \hat B\hat A\hat C - \hat B\hat A\hat C = \hat B[\hat A,\hat C] + [\hat A,\hat B]\hat C$