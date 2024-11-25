---
dg-publish: true
---
$$\begin{align*}
	x_{1}+ 2x_{2} &= 7 \\
	2x_{1}+ 3x_{2}&= 12 
\end{align*}$$
$$\begin{align*}
	\begin{pmatrix}a_{1} & a_{2} \\ a_{3} & a_{4} \end{pmatrix} \cdot \begin{pmatrix}x_{1} \\x_{2} \end{pmatrix} &= \begin{pmatrix}b_{1} \\ b_{2}\end{pmatrix} \\\\
	A \cdot \vec x &= \vec b
\end{align*}$$
- $A^{-1}$ such that $A^{-1}A = I:$ 
$$\begin{align*}
		A\vec x &= \vec b \\
		A^{-1}A\vec x &= A^{-1}\vec b \\
		I\vec x &= A^{-1}\vec b \\
		\therefore \vec x &= A^{-1}\vec b
	\end{align*}$$
- assume: 
$$A^{-1} = \begin{pmatrix} -a_{4} & a_{3} \\ a_{2 } & -a_{1}\end{pmatrix}$$
- check that $A^{-1}A = I$
- so: 
$$\begin{pmatrix}x_{1} \\ x_{2}\end{pmatrix} = \begin{pmatrix} -a_{4} & a_{3} \\ a_{2 } & -a_{1}\end{pmatrix} \begin{pmatrix}b_{1} \\ b_{2}\end{pmatrix}$$
