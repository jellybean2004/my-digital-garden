---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k13-additional-properties/","noteIcon":"1","created":"2024-10-01T18:27:09.391+01:00","updated":"2024-11-26T19:40:35.401+00:00"}
---

- $(i):$ if $y$ is a column vector, $y^{T}$ is a row vector, and vice versa

- $(ii):$
$$(AB)^{T} = B^{T}A^{T}$$
	- **proof**:
$$\begin{align*}
		(AB)^{T}_{ik} &= \sum\limits_{j}a_{kj}b_{ji} \\
		&= \sum\limits_{j} a_{jk}^{T} b_{ij}^{T} \\
		&= (B^{T}A^{T})_{ik}
	\end{align*}$$

- ($iii):$ **orthogonality for vectors**
	- vectors are orthogonal if
$$\begin{align*}
			\vec y^{T}\cdot \vec y &= \beta \\
			\vec y^{\dagger} \cdot \vec x &= 0
		\end{align*}$$
		- if vectors are normalized, $\beta=1$
	- for [[content/011/PX153 - mathematics for physicists/term 2/PX153 - K - linear algebra/PX153 - K10 - special matrices#hermitian or anti-hermitian matrices\|hermitian matrices]] ($A^{\dagger}=A$):
		- [[content/011/PX153 - mathematics for physicists/term 2/PX153 - K - linear algebra/PX153 - K12 - eigenvectors and eigenvalues\|eigenvalues]] are always real
		- if $\lambda_{i}\neq\lambda_{j},\; i\neq j:$ then eigenvectors are all orthogonal
		- if $\lambda_{i}=\lambda_{j},\; i\neq j:$ then orthogonal eigenvectors as long as $\det A \neq 0$
	- **proof**: 
		- consider a hermitian matrix, $A$, with a distinct eigenvalue, $\lambda_{i}$, such that $\lambda_{i}\neq\lambda_{j},\; i\neq j$
		
$$A\,\vec x^{i} = \lambda_{i}\,\vec x^{i}$$
		- taking the hermitian conjugate of the equation:
$$\begin{align*}
				(A\,\vec x^{i})^{\dagger} &= (\lambda_{i}\,\vec x^{i})^{\dagger} \\
				\vec x^{i\dagger}A^{\dagger} &= \lambda_{i}^{*}\vec x^{i\dagger} \\
				\vec x^{i\dagger}A &= \lambda_{i}^{*}\vec x^{i\dagger}
			\end{align*}$$
		- multiplying by $\vec x^{j}$ (from the right):
$$\begin{align*}
				\vec x^{i\dagger}A\vec x^{j}  &= \lambda_{i}^{*}\vec x^{i\dagger}\vec x^{j} \\
				\vec x^{i\dagger}\lambda_{j}\vec x^{j}  &= \lambda_{i}^{*}\vec x^{i\dagger}\vec x^{j} \\
				(\lambda_{j}-\lambda_{i}^{*})(\vec x^{i\dagger}\vec x^{j}) &= 0  
			\end{align*}$$
		- if $i\neq j: \vec x^{i\dagger}\vec x^{j}=0$, giving the definition of orthogonality
		- if $i=j: \lambda_{i} = \lambda_{i}^{*}\implies\lambda_{i} \in \mathbb Re$ 
	
	- if the eigenvalues are *degenerate*, ie: $\lambda_{i}=\lambda_{j},\; i\neq j$, orthogonal eigenvectors can still be constructed

- real symmetric and anti-symmetric matrices
