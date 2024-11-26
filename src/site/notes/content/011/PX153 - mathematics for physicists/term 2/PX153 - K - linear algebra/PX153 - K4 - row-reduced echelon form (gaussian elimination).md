---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k4-row-reduced-echelon-form-gaussian-elimination/","created":"2024-10-01T18:27:09.415+01:00","updated":"2024-11-26T19:40:05.826+00:00"}
---

$$\begin{align*}
	x_{1}+ 2x_{1} &= 3 & L_{1} \\
	x_{1}+ x_{2} &= 7 & L_{2} 
\end{align*}$$
$$\begin{align*}
L_{1}\to L_{1} &: x_{1}+ 2x_{1} = 3  \\
L_{2}\to L_{2}-L_{1} &: -x_{2}=-4  
\end{align*}$$
$$\begin{align*}
L_{1}\to L_{1} + 2L_{2} &: x_{1}=11  \\
L_{2}\to -L_{2} &: -x_{1}-x_{2}=-7  
\end{align*}$$
- in the general case, for a system of $m$ linear equations, and $n$ unknowns of the form: 
$$\begin{align*}
	a_{11}x_{1}+ a_{12}x_{2}+ \dots + a_{1n}x_{n} &= b_{1}& L_{1} \\
	a_{21}x_{1}+ a_{22}x_{2}+ \dots + a_{2n}x_{n} &= b_{2}& L_{2} \\
	\vdots \\
	a_{m1}x_{1}+ a_{m2}x_{2}+ \dots + a_{mn}x_{n} &= b_{m}& L_{m} \\
\end{align*}$$
- $a_{ij}$ and $b_{i}$ are all known coefficients
- let, $A - (a_{ij})_{m\times n}$ , $\vec x = (x_{j})_{n}$ , $\vec b = (b_{i})_{m}$

$$A\,\vec x = \vec b$$
- usually, $m=n$, but sometimes, $m\neq n$, so solution may be unique, incomplete, or non-existent

- eg: 
$$\begin{align*}
	2x_{1}+ x_{2} + x_{3} &= 1 \\
	3x_{1}+(-x_{2})- 2x_{3}&= 1 
\end{align*}$$
	- $L_{1}\to \frac{L_{1}}{2}$ ; $L_{2}\to L_{2}:$ 
$$\begin{bmatrix}2 & 1 & 1 & | & 1 \\
	3  & -1 & -2 & | & 1
\end{bmatrix}$$
	- $L_{1}\to L_{1}$ ; $L_{2}\to L_{2}-3L_{1}:$ 
$$\begin{bmatrix}
	1 & 1/2 & 1/2 & | & 1/2 \\ 
	0 & -5/2 & -7/2 & | & -1/2
\end{bmatrix}$$
	- $L_{1}\to L_{1}$ ; $L_{2}\to \frac{-2}{5}L_{2}:$ 
$$\begin{bmatrix}
	1 & 1/2 & 1/2 & | & 1/2 \\ 
	0 & 1 & 7/5 & | & 1/5
\end{bmatrix}$$
	- $L_{1}\to L_{1}- \frac{1}{2}L_{2}$ ; $L_{2}\to L_{2}:$ 
$$\begin{bmatrix}
	1 & 0 & \frac{1}{2}(1- \frac{7}{5}) & | & \frac{1}{2}(1- \frac{1}{5}) \\ 
	0 & 1 & 7/5 & | & 1/5
\end{bmatrix}$$
	$$\begin{align*}
x_{1}+ \frac{1}{5}x_{3}&= \frac{2}{5} \\
x_{2}+ \frac{7}{5}x_{3}&= \frac{1}{5}
\end{align*}$$
	- setting $x_{3}=\lambda$, solution set: 
$$\begin{bmatrix}x_{1} \\ x_{2}\\ x_{3}\end{bmatrix} = \begin{bmatrix} \frac{2}{5}- \frac{1}{5}\lambda \\ \frac{1}{5}- \frac{7}{5}\lambda \\ \lambda \end{bmatrix}$$

- eg: 
$$\begin{align*}
	x_{1}-2x_{2}+ x_{3} &= 1 \\
	2x_{1}+ x_{2}+ x_{3} &= 1 \\
	5x_{2}-x_{3} &= -1 \\
 \end{align*}$$
 $$\begin{bmatrix}1 & -2 & 1 & | & 1 \\
	2 & 1 & 1 & | & 1 \\
	0 & 5 & -1 & | & -1
 \end{bmatrix}$$
	 - $L_{2}\to L_{2}-2L_{1}:$ 
 $$\begin{bmatrix}1 & -2 & 1 & | & 1 \\
	0 & 5 & -1 & | & -1 \\
	0 & 5 & -1 & | & -1
 \end{bmatrix}$$
	 - $L_{3}\to L_{3}-L_{2}:$ 
 $$\begin{bmatrix}1 & -2 & 1 & | & 1 \\
	0 & 5 & -1 & | & -1 \\
	0 & 0 & 0 & | & 0
 \end{bmatrix}$$
	- $L_{2}\to \frac{1}{5}L_{2}:$ 
$$\begin{bmatrix}1 & -2 & 1 & | & 1 \\
	0 & 1 & -\frac{1}{5} & | & - \frac{1}{5}
 \end{bmatrix}$$
	 - $L_{1}\to L_{1}+2L_{2}:$ 
 $$\begin{bmatrix}1 & 0 & \frac{3}{5} & | & \frac{3}{5} \\
	0 & 1 & -\frac{1}{5} & | & - \frac{1}{5}
 \end{bmatrix}$$
$$\begin{bmatrix}x_1 \\ x_2 \\ x_3\end{bmatrix} = \begin{bmatrix}\frac{3}{5}(1-\lambda) \\ \frac{1}{5}(\lambda-1) \\ \lambda\end{bmatrix}$$
- for 2D: 
$$\begin{align*}
	\alpha x_{1} + \beta x_{2} &= a & L_{1} \\ 
	\alpha x_{1} + \beta x_{2} &= b & L_{2} 
\end{align*}$$
	- only consistent if $a=b$
- for 3D: 
$$\begin{align*}
	\alpha x_{1} + \beta x_{2} + \gamma x_{3} &= a & P_{1} \\ 
	\alpha x_{1} + \beta x_{2} + \gamma x_{3} &= b & P_{2} 
\end{align*}$$
	- if there are three equations with one linearly independent from the others, they can be parallel planes
