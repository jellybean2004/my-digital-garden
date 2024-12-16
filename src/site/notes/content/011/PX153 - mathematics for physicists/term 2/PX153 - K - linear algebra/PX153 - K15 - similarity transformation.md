---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k15-similarity-transformation/","noteIcon":"1","created":"2024-10-01T18:27:09.401+01:00","updated":"2024-11-26T19:40:39.806+00:00"}
---

- applying transformation matrix $A$ to $\vec y = A\vec x$
- from previous derivation: $\vec x = S\vec x'$, $\vec y = S\vec y':$
$$\begin{align*}
		S \vec y' &= AS\,\vec x' \\
		\vec y' &= S^{-1}AS\,\vec x'
	\end{align*}$$
- $S^{-1}AS$ describes the mapping of matrix $A$ in a new basis of vectors, and this  relation, $A\to S^{-1}AS$ , is called a *similarity transformation*

## properties of similarity transformation
- $(i):$
$$I' = S^{-1}IS = I$$
- **reminder:** for $A^{-1}A=I$,
$$\begin{align*}
		\det (A^{-1}A)=\det I &= 1 \\ 
		\det A^{-1} \times \det A &= 1 \\ 
		\implies \det A^{-1} &= \frac{1}{\det A}
	\end{align*}$$ 
- *(ii):*
$$\begin{align*}
		\det A' &= \det (S^{-1}AS) \\
		&= \det S^{-1} \det A \det S \\
		&= \frac{1}{\det S} \det A \det S \\
		\det A'&= \det A
	\end{align*}$$
- $(iii):$
$$\begin{align*}
		\det (A'-\lambda I') &= \det (S^{-1}(A-\lambda I)S) \\
		&= \det S^{-1} \det (A-\lambda S) \det S \\
		&= \det(A-\lambda I)
	\end{align*}$$
- $(iv):$
$$Tr\, A' = Tr\,A$$
	- this is a useful as a check for similarity
	- **proof:**
$$\begin{align*}
			Tr\, A' &= \sum\limits_{i}(S^{-1}AS)_{ii} \\
			&= \sum\limits_{i,j,k} S_{ij}^{-1}A_{jk}S_{ki} \\
			&= \sum\limits_{i,j,k} S_{ki}S_{ij}^{-1} A_{jk} \\
			&= \sum\limits_{i,j,k} I_{kj} A_{jk} \\
			&= \sum\limits_{j}(AI)_{jj} \\
			&= \sum\limits_{j}A_{jj} \\
			&= Tr\, A
		\end{align*}$$
