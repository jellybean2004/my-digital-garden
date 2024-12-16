---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k9-lu-decomposition-method/","noteIcon":"1","created":"2024-10-01T18:27:09.430+01:00","updated":"2024-11-26T19:40:24.151+00:00"}
---

- $A=LU$, where $L$ and $U$ are lower and upper triangular matrices
- eg: in $3\times3$ case, 
$$\begin{align*}
	A &= \begin{bmatrix}1 & 0 & 0 \\ L_{21} & 1 & 0 \\ L_{31} & L_{32} & 1 \end{bmatrix} \begin{bmatrix}U_{11} & U_{12} & U_{13} \\ 0 & U_{22} & U_{23} \\ 0 & 0 & U_{33} \end{bmatrix} \\
	&= \begin{bmatrix} U_{11} && U_{12} & U_{13} \\ L_{21}U_{11} && L_{21}U_{12}+U_{22} & L_{21}U_{13}+U_{23} \\ L_{31}U_{11} && L_{31}U_{12}+L_{32}U_{22} & L_{31}U_{13}+L_{32}U_{23}+U_{33} \end{bmatrix}
\end{align*}$$
- $9$ equations to solve for $a_{ij}$, and then, 
$$\det A = \det L \cdot \det U = U_{11}\times U_{22} \times U_{33}$$
- usually the fastest method to find the determinant, $|A|$, and the solution vector, $\vec x$, for simultaneous equations
- $O(n\times n)$ operations

- eg: $A = \begin{bmatrix}2 & 4 & 3 \\ 1 & -2 & -2 \\ -3 & 3 & 2\end{bmatrix},\; \vec x = \begin{bmatrix}x_1 \\ x_{2}  \\ x_{3}\end{bmatrix},\; \vec b = \begin{bmatrix}4 \\ 0 \\ -7\end{bmatrix}$
	- $1^{st}$ row ${} :U_{11}=2$, $U_{12}=4$, $U_{13}=3$
	- $2^{nd}$ row ${} :L_{21}U_{11}= 1 \implies L_{21} = \frac{1}{2}$ 
	- $3^{rd}$ row $:L_{31}U_{11}= -3 \implies L_{31}= -\frac{3}{2}$
	- *remaining*:
		$L_{21}U_{12}+ U_{22}=-2 \implies U_{22}=-4$
		$L_{21}U_{13}+U_{23}=-2 \implies U_{23}= -\frac{7}{2}$
		$L_{31}U_{12}+L_{32}U_{22} = 3 \implies L_{32}=- \frac{3}{4}$
		$L_{31}U_{13}+L_{32}U_{23}+U_{33} = 2 \implies U_{33}=- \frac{11}{8}$
$$A = \begin{bmatrix}1 & 0 & 0 \\ \frac{1}{2} & 1 & 0 \\ - \frac{3}{2} & - \frac{9}{4} & 1\end{bmatrix} \begin{bmatrix}2 & 4 & 3 \\ 0 & -4 & - \frac{7}{3} \\ 0 & 0 & - \frac{11}{8}\end{bmatrix}$$
$$\det A = (1)\times \left(2\times (-4) \times \left(- \frac{11}{8}\right)\right)= -11$$
$$\begin{gather*}
	A\vec x = \vec b \\
	LU\vec x = \vec b \\
	let,\; U\vec x=\vec y \implies L \vec y = b  \\\\
	L \vec y = b \\
	\begin{bmatrix}1 & 0 & 0 \\ \frac{1}{2} & 1 & 0 \\ - \frac{3}{2} & - \frac{9}{4} & 1\end{bmatrix} \begin{bmatrix}y_{1} \\ y_{2} \\ y_{3}\end{bmatrix} = \begin{bmatrix}4 \\ 0 \\ -7\end{bmatrix} \\\\
	y_{1} = 4 \\
	y_{2} = -2 \\
	y_{3} = -\frac{11}{2} \\\\
	U\vec x=\vec y \\
	\begin{bmatrix}2 & 4 & 3 \\ 0 & -4 & - \frac{7}{3} \\ 0 & 0 & - \frac{11}{8}\end{bmatrix} \begin{bmatrix}x_1 \\ x_{2}  \\ x_{3}\end{bmatrix} = \begin{bmatrix}4 \\ -2 \\ - \frac{11}{2}\end{bmatrix} \\\\
	x_{3}= 4 \\
	x_{2}= -3 \\
	x_{1}= 2 \\\\
	\therefore \vec x = \begin{bmatrix}2 \\ -3 \\ 4\end{bmatrix}
\end{gather*}$$
