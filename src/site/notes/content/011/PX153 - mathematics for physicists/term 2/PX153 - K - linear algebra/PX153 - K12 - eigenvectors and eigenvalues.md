---
dg-publish: true
---
- if $A\,\vec x = \lambda\,\vec xA\,\vec x = \lambda\,\vec x$, $\vec x$ is the *eigenvector* of $A$, and $\lambda$ is its *eigenvalue*
	- '*eigen*': proper (german)
- generally, $\vec x=0$, or $\lambda=0$ are not acceptable values
- restricted to square matrices

- the $i^{th}$ eigenvector is denoted as $\vec x^{i}$, and eigenvalue as $\lambda_{i}$
- if $\lambda_{i}$ are distinct and non-zero, there are $n$ linearly independent eigenvectors for a $n\times n$ matrix
- if $\lambda_{i}=\lambda_{j}$, for $i\neq j$, ie: two eigenvalues are the same, there may or may not be $n$ independent eigenvectors

## finding eigenvalues and eigenvectors
$$\begin{align*}
	A\,\vec x &= \lambda\,\vec x \\
	A\,\vec x - \lambda\,\vec x &= 0 \\
	(A-I\,\lambda)\vec x &= 0 \\
	C\,\vec x &= 0
\end{align*}$$
- if $C\,\vec x=0$, $\det C =0$, so $\det(A-I\,\lambda)=0$
- think of $C\,\vec x=0$ as the "magnification" of $\vec x$ vectors
- if all vectors shrink to $0$, $\det C=0$
- **proof**: if $\det C \neq 0,\, C^{-1}$ exists, $C^{-1}C\,\vec x=0 \implies \vec x=0$
	- but $\vec x=0$ is a trivial solution
	- therefore, $C^{-1}$ does not exist and $\det C=0$

- always expect at least one free parameter per eigenvector (length of that vector)
- because the amplitude is not defined in a basis of vectors
- if $\vec x^{i}$ is an eigenvector, $\alpha\,\vec x^{i}$ is also an eigenvector:
$$A(\alpha\vec x^{i}) = A\vec x^{i}= (\lambda\vec x^{i}) = \lambda(\alpha\vec x^{i})$$

- 2D case:
	$$A = \begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix}$$
	$$\begin{align*}
		\det(A-\lambda\,I) &= (a_{11}-\lambda)(a_{22}-\lambda)- a_{12}a_{21} \\
		0 &= \lambda^{2} - \lambda(a_{11}+a_{22})+ a_{11}a_{22} - a_{12}a_{21} \\
	\end{align*}$$
- for eigenvectors, $A\,\vec x = \lambda_{i}\,\vec x$, plug in $\lambda_{i}$ 

- eg:
$$A= \begin{bmatrix}4 & 1 \\ 3 & 2\end{bmatrix}$$
	$A-\lambda\,I = \begin{bmatrix}4-\lambda & 1 \\ 3 & 2-\lambda \end{bmatrix}$
	$$\begin{align*}
		\det(A-\lambda\,I) &= \lambda^{2}- 6\lambda + 5 = 0 \\
		\lambda_{1}= 5&, \;\lambda_{2}=1 
	\end{align*}$$
	- taking $\lambda_{2}=1:$
$$\begin{align*}
			(A-\lambda\,I)\vec x &= 0 \\
			\begin{bmatrix}3 & 1 \\ 3 & 1\end{bmatrix}\begin{bmatrix}x_{1} \\ x_{2}\end{bmatrix} &= \begin{bmatrix}0 \\ 0\end{bmatrix} \\\\
			3x_{1}+x_{2} &= 0 \\
			let\,x_{1}=t&, x_{2}=-3t
		\end{align*}$$
		- the eigen vector is: $t\begin{bmatrix}1 \\ -3\end{bmatrix}$ , $t$ is a *free parameter*
		- normalizing:
$$\begin{align*}
			\vec x^{T}\cdot \vec x &= 1 \\
			t^{2}(1+9) &= 1 \\
			\therefore t &= \frac{1}{\sqrt{10}}
		\end{align*}$$
		- the normalized eigenvector is: $\frac{1}{\sqrt{10}}\begin{bmatrix}1 \\ -3\end{bmatrix}$
	
	- taking $\lambda_{2}=5:$
$$\begin{align*}
			(A-\lambda\,I)\vec x &= 0 \\
			\begin{bmatrix}-1 & 1 \\ 3 & -3\end{bmatrix}\begin{bmatrix}x_{1} \\ x_{2}\end{bmatrix} &= \begin{bmatrix}0 \\ 0\end{bmatrix} \\\\
			either,\,x_{1}+x_{2} &= 0 \\
			or,\;3x_{1}-3x_{2} &= 0 \\\\
			let\,x_{1}=t&, x_{2}= t
		\end{align*}$$
		- the eigen vector is: $t\begin{bmatrix}1 \\ 1\end{bmatrix}$ , $t$ is a *free parameter*
		- normalizing:
$$\begin{align*}
			\vec x^{T}\cdot \vec x &= 1 \\
			t^{2}(1+1) &= 1 \\
			\therefore t &= \frac{1}{\sqrt{2}}
		\end{align*}$$
		- the normalized eigenvector is: $\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\ 1\end{bmatrix}$
	
		- checking:
$$\begin{bmatrix}4 & 1 \\ 3 & 2\end{bmatrix} \frac{1}{\sqrt{2}}\begin{bmatrix}1 \\ 1\end{bmatrix} = \frac{1}{\sqrt{2}}\begin{bmatrix}5 \\ 5\end{bmatrix} = \frac{5}{\sqrt{2}}\begin{bmatrix}1 \\ 1\end{bmatrix}$$
			- $5$ is the eigenvalue, $\frac{1}{\sqrt{2}}\begin{bmatrix}1 \\ 1\end{bmatrix}$ is the eigenvector
 