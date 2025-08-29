---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k1-terminology-of-matrices/","noteIcon":"1","created":"2025-08-27T13:14:05.128+01:00","updated":"2024-11-26T19:39:57.000+00:00"}
---

## introduction
- a matrix is a rectangular array of numbers
- if there are $m$ rows and $n$ columns, the matrix has a size of $m\times n:$ 
$$A_{m\times n} = \begin{pmatrix} 
  a_{11} & a_{12} &\dots& a_{1n} \\ 
  a_{21} & a_{22} && \vdots \\
  \vdots  && \ddots & \vdots\\ 
  a_{m1} &...&...& a_{mn}
  \end{pmatrix}$$
  - $a_{ij}$ represents the element in the $i^{th}$ row and $j^{th}$ column
  - often written as: 
  $$A = (a_{ij})_{m\times n}$$
-  if a matrix has shape, $m\times 1$, it is a *column vector*: 
$$A= \begin{pmatrix}a_{1} \\ a_{2}  \\ \vdots \\ a_{m}\end{pmatrix}$$
- if a matrix has shape, $1\times n$, it is a *row vector*: 
$$B = \begin{pmatrix}b_{1} & b_{2} & \dots & b_{n}\end{pmatrix}$$
## transpose
- if a matrix, $A = (a_{ij})_{m\times n}$, the transpose of $A$ is the matrix, $A^{T}$, has dimensions $n\times m$, and is obtained by transposing the rows and columns of $A:$ 
$$A^{T}= (\alpha_{ij})_{n\times m}= (a_{ji})_{n\times m}$$
- eg: 
$$\begin{align*}
  A &= \begin{pmatrix} 1 & 2 & 3 \\
  4 & 5 & 6\end{pmatrix} \\\\
  A^{T} &= \begin{pmatrix}1 & 4 \\ 2 & 5  \\ 3 & 6\end{pmatrix}
\end{align*}$$
## special matrices
  - $m\times n$ matrices with all elements equal to $0$ is denoted by '$0_{m\times n}$', and is called a *zero matrix*
  - a $n\times n$ matrix is called a *square matrix* of order $n$
	  - $a_{ij}$, for $i=j$, are called the elements of the diagonal
  - a square matrix is a *diagonal matrix* if $a_{ij}=0 \; \forall \; i\neq j$
  - a diagonal matrix is an *identity matrix* if the diagonal elements are $1$
