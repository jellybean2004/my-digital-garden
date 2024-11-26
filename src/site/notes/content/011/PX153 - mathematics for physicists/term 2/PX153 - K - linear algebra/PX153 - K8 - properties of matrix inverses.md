---
dg-publish: true
---
- $(i):$ if $A$ and $B$ are *invertible* (have inverses), and have the shape, $n\times n$, then $AB$ is also invertible, and $(AB)^{-1} = B^{-1}A^{-1}$
	- proof: $(B^{-1}A^{-1})(AB) = B^{-1}(A^{-1}A)B = B^{-1}(I)B = I$

- $(ii):$ if $A$ is a $n\times n$ invertible matrix, then $A^{T}$ is invertible, and $(A^{T})^{-1} = (A^{-1})^{T}$
	- proof: 
$$\begin{align*}
	((A^{-1})^{T}A^{T})_{ik} &= \sum\limits_{j=1}^{n} (a^{-1})_{ij}^{T} (a)_{jk}^{T} \\
	&= \sum\limits_{j=1}^{n} (a^{-1})_{ji} (a)_{kj} \\
	&= \sum\limits_{j=1}^{n}a_{kj}a_{ji}^{-1} \\
	&= (AA^{-1})_{ki} \\
	&= (I)_{ki} \\
	&= (I)_{ik}
\end{align*}$$
- in principle, the inverse of a matrix can be used to compute solutions to simultaneous equations
	- eg: to solve $A\vec x=\vec b:$ if $A^{-1}$ exists, then $\vec x = A^{-1}\,\vec b$
- earlier, [[content/011/PX153 - mathematics for physicists/term 2/PX153 - K - linear algebra/PX153 - K4 - row-reduced echelon form (gaussian elimination)\|gaussian elimination]] was used from interchanges of lines (rows)
- the inverse method of finding $A^{-1}$ and solving for $\vec x$ needs of the order of $O(n\times n!)$, which is very inefficient for $n>3$
- methods using gaussian elimination are actually faster in most cases

