---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/g-additional-interactions/px-262-g4-pauli-spin-matrices/","noteIcon":"1","created":"2024-11-25T11:32:10.229+00:00","updated":"2024-11-26T18:12:42.824+00:00"}
---

- representation for spin $1/2$ operators
- suitable matrices:
$$\sigma_{x}= \begin{pmatrix}0 & 1 \\ 1 & 0\end{pmatrix} ,\; \sigma_{y}= \begin{pmatrix}0 & -i \\ i & 0\end{pmatrix} ,\; \sigma_{z}= \begin{pmatrix}1 & 0 \\ 0 & -1\end{pmatrix}$$
with these spin operators for spin $1/2$
$$\hat S_{i}= \frac{1}{2}\hbar \sigma_{i}$$
- verifying commutation relations:
$$\begin{align*}
[\hat S_{x}, \hat S_{y}] &= \frac{\hbar^{2}}{4} \left[ \begin{pmatrix} 0 & 1 \\ 1 & 0  \end{pmatrix} \begin{pmatrix} 0 & -i \\ i & 0  \end{pmatrix} - \begin{pmatrix} 0 & -i \\ i & 0  \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0  \end{pmatrix} \right] \\
&= \frac{\hbar^{2}}{4} \left[ \begin{pmatrix} i & 0 \\ 0 & -i  \end{pmatrix} - \begin{pmatrix} -i & 0 \\ 0 & i  \end{pmatrix} \right] \\ &= i\hbar \frac{\hbar}{2} \begin{pmatrix} 1 & 0 \\ 0 & -1  \end{pmatrix} \\
\therefore [\hat S_{x}, \hat S_{y}] &= i\hbar \hat S_{z}
\end{align*}
$$
- the eigenvalues of $\hat S_z$ are ${} + \frac{1}{2}\hbar {}$ and $-\frac{1}{2}\hbar$, with the eigenvectors $\begin{pmatrix}1 \\ 0\end{pmatrix}$ and $\begin{pmatrix}0  \\ 1\end{pmatrix}$
- for $\hat S_{x}$, the eigenvalues are $\pm \frac{1}{2}\hbar$, and the eigenvectors are ${} \frac{1}{\sqrt 2}\begin{pmatrix}1 \\ i\end{pmatrix} {}$ and $\frac{1}{\sqrt2}\begin{pmatrix}1  \\ -i\end{pmatrix}$
- the operator:
$$\hat S^{2} = \hat S_{x}^{2} + \hat S_{y}^{2}+ \hat S_{z}^{2} = \frac{3}{4} \hbar^{2} \begin{pmatrix}1 & 0 \\ 0 & 1\end{pmatrix}$$
