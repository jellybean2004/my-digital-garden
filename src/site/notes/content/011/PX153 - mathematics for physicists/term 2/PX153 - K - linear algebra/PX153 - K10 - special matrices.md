---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k10-special-matrices/","created":"2024-10-01T18:27:09.383+01:00","updated":"2024-11-26T19:40:20.490+00:00"}
---

## symmetric and anti-symmetric matrices
- if $A^{T}=A: A$ is a *symmetric matrix*
- if $A^{T}=-A:A$ is an *anti-symmetric matrix*

- any $n\times n$ matrix is the sum of a symmetric and an anti-symmtric matrix
- **proof**: 
$$\begin{align*}
	A &= \frac{(A + A^{T}) + (A-A^{T})}{2}\\\\
	B &= \frac{A+A^{T}}{2}=B^{T}: symmetric\\\\
	C &= \frac{A-A^{T}}{2} \\
	C^{T} &= \frac{A^{T}-A}{2} = -C : anti-symmetric \\
\end{align*}$$
## orthogonal matrices
- if $A^{T}=A^{-1}: A$ is an *orthogonal matrix*

- eg: $A = \begin{bmatrix}\cos\theta & -\sin\theta \\ \sin\theta & \cos\theta\end{bmatrix}: A^{T} = \begin{bmatrix}\cos\theta & \sin\theta \\ -\sin\theta & \cos\theta\end{bmatrix}$
	- $AA^{T}= \begin{bmatrix}1 & 0 \\ 0 & 1\end{bmatrix} = I: A$ is orthogonal
## singular matrices
- if $\det A =0: A$ is a *singular matrix*
## hermitian conjugate matrix
- the *hermitian conjugate* of a matrix is the transpose of the complex conjugate of the matrix: 
$$\begin{align*}
	A^{\dagger}= (A^{*})^{T} &= (A^{T})^{*} \\
	(a^{\dagger})_{ij}&= a_{ji}^{*}
\end{align*}$$
### hermitian or anti-hermitian matrices
- if $A^{\dagger}=A : A$ is a *hermitian matrix*
- if $A^{\dagger}=-A : A$ is an *anti-hermitian matrix*
	- eg: $A = \begin{bmatrix}0 & -i \\ i & 0\end{bmatrix}$
		$A^{*} = \begin{bmatrix}0 & i \\ -i & 0\end{bmatrix}$
		$A^{\dagger}= A: A$ is a hermitian matrix

- any $n\times n$ matrix can be written as a sum of a hermitian and an anti-hermitian matrix
- **proof**: 
$$\begin{align*}
	A &= \frac{1}{2}(A + A^{\dagger}) + \frac{1}{2}(A - A^{\dagger}) \\\\
	B &= \frac{1}{2}(A + A^{\dagger}) = B: hermitian \\\\
	C &= \frac{1}{2}(A - A^{\dagger}) \\
	C^{\dagger} &= \frac{1}{2}(A^{\dagger}-A)=-C: anti-hermitian
\end{align*}$$
## unitary matrices
- $A$ is a unitary matrix if $A^{\dagger}=A^{-1}$
- eg: 
$$\begin{align*}
	A &= \begin{bmatrix}0 & -i \\ i & 0\end{bmatrix} \\
	A^{\dagger} &= \begin{bmatrix}0 & i \\ -i & 0\end{bmatrix} \\
	A^{\dagger}A &= \begin{bmatrix}1 & 0 \\ 0 & 1\end{bmatrix} = I \\
	\therefore \;& A\;is\;unitary
\end{align*}$$
- for unitary matrices: 
$$\begin{align*}
	|\lambda_{i}|^{2} &= 1 \\
	\lambda_{i}^{*}\lambda_{i} &= 1
\end{align*}$$
- **proof**: 
$$\begin{align*}
	U\,\vec x^{i} &= \lambda_{i}\vec x^{i} \\
	U^{-1}U\,\vec x^{i} &= U^{-1}\lambda_{i}\vec x^{i}  \\
	\frac{1}{\lambda_{i}} \vec x^{i} &= U^{-1}\vec x^{i} \\
	\frac{1}{\lambda_{i}} \vec x^{i\dagger} \vec x^{i} &= \vec x^{i\dagger}U^{\dagger}\vec x^{i} \\
	\frac{1}{\lambda_{i}} \vec x^{i\dagger} \vec x^{i} &=  (U\vec x^{i})^{\dagger}\vec x^{i} \\
	\frac{1}{\lambda_{i}} \vec x^{i\dagger} \vec x^{i} &=  \lambda_{i}^{*}\vec x^{i\dagger}\vec x^{i} \\
	\left(\frac{1}{\lambda_{i}}- \lambda_{i}^{*}\right)(\vec x^{i\dagger} \vec x^{i}) &= 0 
\end{align*}$$
	- $(\vec x^{i\dagger} \vec x^{i})$ cannot be $0:$ 
	
$$\frac{1}{\lambda_{i}}- \lambda_{i}^{*} = 0 \implies \lambda_{i}^{*}\lambda_{i}=1$$
	- the modulus of eigenvalues is unity

	