---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k7-matrix-inverse/","noteIcon":"1","created":"2024-10-01T18:27:09.423+01:00","updated":"2024-11-26T19:40:15.078+00:00"}
---

## some definitions
- *minor:* $m_{ij}$ is determinant of $(n-1)\times(n-1)$ matrix where the $i^{th}$ row and $j^{th}$ column of $A$ are removed
- *[[content/011/PX153 - mathematics for physicists/term 2/PX153 - K - linear algebra/PX153 - K5 - trace and determinants#cofactor\|co-factor]]:* $(-1)^{i+j}m_{ij} = c_{ij}$
	- $\det A = a_{11}c_{11}+\dots + a_{1n}c_{1n}$
	- this formula suggests that the $1^{st}$ row is special
	- the rows and columns can be exchanged
		- $(i): \det A = \sum\limits_{j=1} a_{ij}c_{ij}$ (*co-factor rule*)
		- $(ii): \sum\limits_{j=1} a_{ij}c_{kj}=0 \;\forall\; i\neq k$ (*false co-factor rule)
- co-factor rule for $3\times 3:$ 
$$\det \begin{bmatrix}e_{1} & e_{2} & e_{3} \\ f_{1} & f_{2} & f_{3} \\ g_{1} & g_{2} & g_{3}\end{bmatrix} = - \det \begin{bmatrix}f_{1} & f_{2} & f_{3} \\ e_{1} & e_{2} & e_{3} \\ g_{1} & g_{2} & g_{3}\end{bmatrix} = f_{1}c_{21}+f_{2}c_{22}+ f_{3} c_{23}$$
	- switching row 1 and row 2 is equivalent to expanding from the $2^{nd}row$
- false co-factor rule: $A = \begin{bmatrix}e_{1} & e_{2} & e_{3} \\ f_{1} & f_{2} & f_{3} \\ g_{1} & g_{2} & g_{3}\end{bmatrix}$
	- $\det A = \vec e \cdot (\vec f \times \vec g)$
	- using false co-factor rule: $\sum\limits_{j} a_{ij}c_{kj} \stackrel{?}{=} 0$
	- using $i=2,\; k=1:$ 
$$\sum\limits_{j} a_{2j}c_{1j} = f_{1}c_{11}+ f_{2}c_{12}+ f_{3}c_{13} = \vec f \cdot (\vec f \times \vec g)=0$$
	- in general, $\det A = 0$ if two rows are the same
### the adjugate matrix
- if $A = (a_{ij})_{n\times m}$, the adjugate (AKA adjoint) of $A$, $Adj(A) = (c_{ij}^{T})$, where $c_{ij}$ are co-factors of matrix $A:$ 
$$Adj(A) =   \begin{bmatrix} c_{11} &  \dots & c_{n1} \\ \vdots & \ddots & \vdots \\ c_{1n} & \dots & c_{nn}\end{bmatrix}$$
## the inverse
- $A_{n\times n}$ is inversible if and only if $\det A \neq 0$
$$A^{-1} = \frac{1}{\det A} Adj(A)$$
- let $B = A\, Adj(A)$
$$\begin{align*}
	 B_{ij} &= \sum\limits_{k=1}^{n} a_{ik} (Adj (A))_{kj} \\
	 &= \sum\limits_{k=1}^{n}a_{ik}c_{jk}\\
	 &= \begin{cases}
	 \det A & if \;i=j & cofactor\;rule\\
	 0 & if\;i\neq j & false\;cofactor\;rule
\end{cases}
\end{align*}$$
- hence,  
$$\begin{align*}
	A\, Adj(A) &= \det A\, I \\ 
	A^{-1} &= \frac{1}{\det A} Adj(A) & if\; \det A&\neq 0
\end{align*}$$
- the inverse method is not quick because the determinant and co-factors need to be calculated
- $A\, Adj(A)=\det A\,I$ can be used to infer $\det A$

- eg: find $Adj\, A$, then $A^{-1}$, for $A = \begin{bmatrix}1 & 0 & 2 \\ -1 & 1 & 3 \\ 0 & 2 & 1\end{bmatrix}$
		$c_{11} = (-1)^{1+1} \begin{vmatrix}1 & 3 \\ 2 & 1\end{vmatrix} = -5$
		$c_{12} = (-1)^{1+2} \begin{vmatrix}-1 & 3 \\ 0 & 1\end{vmatrix} = 1$
		$c_{13} = (-1)^{1+3} \begin{vmatrix}-1 & 1 \\ 0 & 2\end{vmatrix} = -2$
		$c_{21} = (-1)^{2+1} \begin{vmatrix}0 & 2 \\ 2 & 1\end{vmatrix} = 4$
		$\vdots$
	$$Adj\, A = \begin{bmatrix}-5 & 4 & -2 \\ 1 & 1 & -5 \\ -2 & -2 & 1\end{bmatrix}$$
	- using $Adj\, A \cdot A = |A|\, I:$ 
$$\begin{align*}
	Adj\, A \cdot A &= \begin{bmatrix}-5 & 4 & -2 \\ 1 & 1 & -5 \\ -2 & -2 & 1\end{bmatrix}\begin{bmatrix}1 & 0 & 2 \\ -1 & 1 & 3 \\ 0 & 2 & 1\end{bmatrix} \\
	&= \begin{bmatrix}-9 & 0 & 0 \\ 0 & -9 & 0 \\ 0 & 0 & -9\end{bmatrix} \\
	&= -9I \\\\
	or,\;|A| &= -9 \\\\
	\therefore A^{-1}&= \frac{1}{-9}A
\end{align*}$$

- eg: $\begin{bmatrix}1 & 6 & -4 \\ 3 & -20 & 1 \\ -1 & 3 & 5\end{bmatrix} \begin{bmatrix}x_{1} \\ x_2 \\ x_{3}\end{bmatrix} = \begin{bmatrix}8 \\ 12 \\ 3\end{bmatrix}$
$$\begin{align*}
	Adj(A) &= \begin{bmatrix} (-100-3) & -(30+12) & (6-8-) \\ -(15+1) & (5-4) & - (1+12) \\ (9-20) & -(3+6) & (-20-18) \end{bmatrix} \\
	&= \begin{bmatrix} -103 & -42 & -74 \\ -16 & 1 & -13 \\ -11 & -9 & -38 \end{bmatrix}
\end{align*}$$
$$\begin{align*}
	Adj(A)\cdot A &= |A|\cdot I \\\\
	Adj(A)\cdot A &= \begin{bmatrix} -103 & -42 & -74 \\ -16 & 1 & -13 \\ -11 & -9 & -38 \end{bmatrix} \begin{bmatrix}1 & 6 & -4 \\ 3 & -20 & 1 \\ -1 & 3 & 5\end{bmatrix} \\
	&= \begin{bmatrix} -155 & 0 & 0 \\ 0 & -155 & 0 \\ 0 & 0 & -155 \end{bmatrix} \\
	&= -155 \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}
\end{align*}$$
$$\begin{align*}
	\vec x &= A^{-1}\,\vec b \\
	\vec x &= \frac{1}{|A|} Adj(A)\,\vec b \\
	\vec x &= \frac{1}{-155} \begin{bmatrix} -103 & -42 & -74 \\ -16 & 1 & -13 \\ -11 & -9 & -38 \end{bmatrix} \begin{bmatrix}8 \\ 12 \\ 3\end{bmatrix} \\
	&= \begin{bmatrix}10 \\ 1 \\ 2\end{bmatrix}
\end{align*}$$
