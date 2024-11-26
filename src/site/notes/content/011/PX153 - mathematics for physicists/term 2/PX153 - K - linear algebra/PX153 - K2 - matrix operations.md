---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k2-matrix-operations/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:39:59.436+00:00"}
---

## addition
- let $A=(a_{ij})_{m\times n}$ and $B= (b_{ij})_{p\times q}$
- $A=B$ if and only if: $(i)\; m=p,\;n=q$, and $(ii)\; a_{ij}= b_{ij} \; \forall \; i,j$

- for matrices with the *same dimensions*: 
$$A+B = \begin{bmatrix}a_{11}+b_{11} & \dots & a_{1n}+b_{1n} \\ 
  \vdots & \ddots & \vdots \\ 
  a_{m1}+b_{m1} & \dots & a_{mn}+b_{mn}
  \end{bmatrix}$$
## scalar multiplication
  - for a scalar, $\lambda$, and a matric, $A=(a_{ij})_{m\times n}:$ 
  $$\lambda A = \begin{bmatrix}\lambda\,a_{11}  &  \dots & \lambda\,a_{1n} \\ 
    \vdots & \ddots & \vdots \\ 
    \lambda\,a_{m1} & \dots  & \lambda\,a_{mn}\end{bmatrix}$$
## multiplication
- let $A=(a_{ij})_{m\times n}$ and $B= (b_{ij})_{n\times q}$
	- note: $col._{A} = row_{B}$
	- if $col_{A} \neq row_{B}$, $AB$ is not defined
- the product, $AB$, is matrix $C = (c_{ij})_{m\times q}$, where, 
$$c_{ij} = a_{i1}b_{ij}+ a_{i2}b_{2j}+\dots = \sum\limits_{k=1}^{n}a_{ik}b_{kj}$$
$$c_{1j} = \begin{bmatrix}a_{i1} & a_{i2} & \dots & a_{in} \end{bmatrix} \times \begin{bmatrix}b_{1j} \\ b_{2j} \\ \vdots \\ b_{nj}\end{bmatrix} = \sum\limits_{k=1}^{n}a_{ik}b_{kj}$$
- dot product of the $i^{th}$ row of $A$ with the $j^{th}$ column of $B$

- matrix multiplication of square matrices of order $n$ can result in $AB\neq BA$
 - matrix multiplication is not commutative
 - the commutator: 
 $$[A,B] \equiv AB-BA$$
 - generally, $[A,B]\neq 0$

- for a square matrix, $A$, there exists $A^{k},\;k\in\mathbb{Z}>0$
### dot product 
$$A_{i\times n}B_{n\times1} = (\sum\limits_{k=1}^n a_{k}b_{k})_{1\times1}$$
### outer product
$$A_{n\times1}B_{1\times n} = \begin{bmatrix}a_{1}b_{1}  & \dots & a_{1}b_{n} \\  \vdots & \ddots & \vdots \\ a_{n}b_{1} & \dots & a_{n}b_{n}\end{bmatrix}$$

### examples
- eg: $A = \begin{bmatrix} 1 & 2 \\-1 & 3 \end{bmatrix}_{2\times2}$, and $B = \begin{bmatrix} 5 & -3 \\ 0 & -2 \end{bmatrix}_{2\times2}$
	  $$AB = \begin{bmatrix} 5+0 & -3-4 \\ -5+0 & 3-6 \end{bmatrix}  = \begin{bmatrix} 5 & -7 \\ -5 & -3\end{bmatrix}$$
	  $$BA = \begin{bmatrix} 5+3 & 10-9 \\ 0+2 & 0-6\end{bmatrix} = \begin{bmatrix}8 & 1 \\ 2 & -6\end{bmatrix}$$
	  $$[A,B] = \begin{bmatrix}-3 & -8 \\ -7 & 3 \end{bmatrix}$$

- eg: $C = \begin{bmatrix}2 & 1 & 4 \\ 0 & 3 & -1\end{bmatrix}_{2\times3}$, and $A = \begin{bmatrix}1 & 2 \\ -1 & 3\end{bmatrix}_{2\times2}$
	$$AC = \begin{bmatrix}2 & 7 & 2 \\ -2 & 8 & -7\end{bmatrix}_{2\times3}$$
	- $CA$ is not a valid product
	- however, $C^{T} = \begin{bmatrix}2 & 0 \\ 1 & 3 \\ 4 & -1\end{bmatrix}_{3\times2}$
	$$C^{T}A = \begin{bmatrix}2 & 4  \\ -2 & 11 \\ 5 & 5\end{bmatrix}_{3\times2}$$

- eg: $A = \begin{bmatrix}0 & 1 \\ 0 & 0\end{bmatrix}$
	$A^{2} = \begin{bmatrix}0 & 0  \\ 0 & 0\end{bmatrix}$
	$$A^{k} = 0_{2\times2}$$
- $A^{k} = 0_{n\times n}$ but $A\neq 0_{n\times n}$
