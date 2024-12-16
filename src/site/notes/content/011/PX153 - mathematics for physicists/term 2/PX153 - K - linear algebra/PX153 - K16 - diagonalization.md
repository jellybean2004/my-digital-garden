---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k16-diagonalization/","noteIcon":"1","created":"2024-10-01T18:27:09.403+01:00","updated":"2024-11-26T19:40:41.899+00:00"}
---

o use similarity transformations to diagonalize matrices:
$$S = \begin{bmatrix}\vdots & \vdots & \vdots && \vdots \\ \vec x^{1} & \vec x^{2} & \vec x^{3} &  \dots & \vec x^{n} \\ \vdots & \vdots & \vdots && \vdots \end{bmatrix}$$
- make the $n^{th}$ column the $n^{th}$ eigenvector of $A$
- transforming $A$ with $S$ will make $A'$, a diagonal matrices

- if $n$ independent eigenvectors can be found , $A'$ is diagonal, if $S$ has column vectors composed of the $n$ independent eigenvectors

- for [[content/011/PX153 - mathematics for physicists/term 2/PX153 - K - linear algebra/PX153 - K10 - special matrices#hermitian or anti-hermitian matrices\|hermitian matrices]], the eigenvectors are orthogonal:
$$(\vec x^{i})^{\dagger} (\vec x^{j})=0\; for\; i\ne j$$
 - $S$ with columns as eigenvectors:
$$\begin{align*}
	S^{\dagger} &= \begin{bmatrix}\dots & (\vec x^{1})^{*} & \dots \\ \dots & (\vec x^{2})^{*} & \dots \\  & \vdots &  \\  \dots & (\vec x^{n})^{*} & \dots\end{bmatrix} \\
	S^{\dagger}S &= I
\end{align*}$$
- hence, $S$  is unitary

-  considering $S^{-1}AS = S^{\dagger}AS:$
$$S^{-1}AS = \lambda_{n}I$$
- the similarity transformation has made $A$ a diagonal matrix with eigenvalues in the diagonals

- eg: diagonalize $A= \begin{bmatrix}3 & 2 \\ 2 & 0\end{bmatrix}$
	- the matrix is hermitian: $A^{\dagger}=A \implies S^{-1}=S^{\dagger}$
	- for eigenvalues and eigenvectors:
$$\begin{align*}
			\det(A-I\lambda) &= 0 \\
			\lambda^{2} -3\lambda-4 &= 0 \\
			(\lambda-4)(\lambda+1) &= 0  \\\\
			\begin{bmatrix}3 & 2 \\ 2 & 0\end{bmatrix} \begin{bmatrix}a \\ b\end{bmatrix} &= \lambda \begin{bmatrix}a \\ b\end{bmatrix} \\\\
			for\,\lambda_{1}=4:\\
			3a+2b &= 4a \\
			2a &= 4b \\
			\therefore a &= 2b \\
			\therefore \vec x^{1}&= \frac{1}{\sqrt{5}} \begin{bmatrix}2 \\ 1\end{bmatrix}
			\\\\
			for\,\lambda_{1}=-1:\\
			3a+2b &= -a \\
			2a &= -b \\
			\therefore -2a &= b \\
			\therefore \vec x^{2}&= \frac{1}{\sqrt{5}} \begin{bmatrix}1 \\ -2\end{bmatrix}
		\end{align*}$$
	- to diagonalize:
$$\begin{align*}
			S &= \begin{bmatrix} \vec x^{1} & \vec x^{2}  \\ \vdots & \vdots\end{bmatrix} \\

			S^{-1}AS &= S^{\dagger}AS\\
			&= \frac{1}{\sqrt{5}}\frac{1}{\sqrt{5}} \begin{bmatrix}1 & -2 \\ 2 & 1\end{bmatrix}\begin{bmatrix}3 & 2 \\ 2 & 0\end{bmatrix} \begin{bmatrix}1 & 2 \\ -2 & 1\end{bmatrix} \\
			&= \frac{1}{5}\begin{bmatrix}-5 & 0 \\ 0 & 20\end{bmatrix} \\
			&= \begin{bmatrix}-1 & 0 \\ 0 & 4\end{bmatrix}
		\end{align*}$$
