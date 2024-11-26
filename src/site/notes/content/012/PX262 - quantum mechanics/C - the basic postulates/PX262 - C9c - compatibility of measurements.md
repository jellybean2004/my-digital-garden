---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c9c-compatibility-of-measurements/"}
---

- take a case where $\phi_{1}$ and $\phi_{2}$ are degenerate eigenfunctions of an operator, $\hat Q$, with an eigenvalue, $q$
- take another operator $\hat R$, which commutes with $\hat Q$, ie: 
  $$[\hat Q, \hat R] = 0$$
$$\hat Q \hat R \phi_{1} = \hat R \hat Q \phi_{1} = q \hat R \phi_{1}$$
- this shows that $\hat R \phi_{1}$ is also an eigenfunction of the operator $\hat Q$
- the result of $\hat R\phi_{1}$ will also be an wavefunction, which can be written as a linear combination of some eigenfunctions: 
  $$\hat R \phi_{1} = a \phi_{1}+ b\phi_{2}$$
- similarly: 
  $$\hat R \phi_{2}= c\phi_{1}+ d\phi_{2}$$
- to show that there is a wavefunction: 
  $$\phi' = A\phi_{1} + B\phi_{2}$$
	which are eigenstates of $\hat R$
$$\hat R \phi' = A\hat R \phi_{1}+ B\hat R \phi_{2} = Aa\phi_{1}+ Ab\phi_{2}+ Bc\phi_{1} + Bd\phi_{2}$$
- the eigenvalue equation: 
  $$\hat R \phi' = r\phi' = rA\phi_{1}+ rB\phi_{2}$$
- comparing the coefficients: 
$$\begin{gather}
	(a-r)A + cB =0 \\
	bA + (d-r)B =0
\end{gather}$$
- this has solutions only if: 
  $$\left| \begin{matrix}a-r & c  \\ b & d-r \end{matrix} \right|=0$$
- this leads to a quadratic equations leading to two possible eigenvalues of $r$
- generally, if there is a degenerate system for one operator, there is another operate that can distinguish the degenerate states