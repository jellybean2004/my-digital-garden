---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/m-basic-postulates-revisited/px-262-m1-introduction-to-spin/","noteIcon":"1","created":"2025-02-24T11:28:59.760+00:00","updated":"2025-02-25T12:05:34.903+00:00"}
---

- experimental evidence points to an electron possessing an intrinsic spin
- there is an associated magnetic moment
$$\hat {\vec \mu} = - \frac{ge}{2m_{e}} \hat {\vec s}$$
	where, ${} g = 2.00232\dots {}$
$$\hat H_{int} = - \hat{\vec \mu}  \cdot \vec B^{ext} = - \hat\mu_{z} B^{ext}$$
- orbital motion also generates a moment $\propto \hat l$, with $\hat H_{int}= -e/2m_{e} \;\hat l \cdot\vec B^{ext}$
- ${} \hat s_{z}$ is associated with spin, $s = 1/2$
- the operator has two eigenvalues: $\pm \hbar/2$ ($-s,-2+1,\dots,+s$)

- choosing $2\times2$ matrices:
$$\hat s_{z} = \frac{\hbar}{2} \begin{pmatrix}1 & 0 \\ 0 &-1\end{pmatrix}$$
- checking:
$$\begin{gather}
\frac{\hbar}{2} \begin{pmatrix}1 & 0 \\ 0 &-1\end{pmatrix} \begin{pmatrix}a \\ b\end{pmatrix} = \lambda \begin{pmatrix}a \\ b\end{pmatrix} \\
\frac{\hbar}{2} a = \lambda a \\
- \frac{\hbar}{2}b = \lambda b \\
\lambda = \frac{\hbar}{2} \implies a = 1,\; b =0 \\
\lambda = -\frac{\hbar}{2} \implies a = 0,\; b =1
\end{gather}$$
- for the eigenvalue, $\lambda = \hbar/2:$
$$\begin{pmatrix}a \\ b\end{pmatrix} = \begin{pmatrix}1\\0\end{pmatrix} = X_{1/2,\,m_{s}=1/2}$$
- for the eigenvalue, $\lambda = \hbar/2:$
$$\begin{pmatrix}a \\ b\end{pmatrix} = \begin{pmatrix}0\\1\end{pmatrix} = X_{1/2,\,m_{s}=-1/2}$$
- spin is an intrinsic angular momentum, so it is set up with the same structure as regular angular momentum

$$\hat l^{2} Y_{lm}(\theta,\varphi) = l(l+1)\hbar^{2} \,Y_{lm}(\theta,\varphi)$$
	where, $l \geq 0$
$$\hat l_{z} Y_{lm}(\theta,\varphi) = m_{l} \hbar \,Y_{lm}(\theta,\varphi)$$
	where, $m_{l} = [-l,+l]$

- these are commutable, ie: 
$$[\hat l^{2}, \hat l_{z}] = 0$$
- but: 
$$\begin{gather}
[\hat l_{x}, \hat l_{y}] = i\hbar\hat l_{z} \\
[\hat l_{y}, \hat l_{z}] = i\hbar\hat l_{x}
\end{gather}$$

- similarly, setting up a structure for spin angular momentum:
- so, $s = \frac{1}{2}\implies m_{} = 1/2, -1/2$
$$\hat s_{z} X_{s,m_{s}} = m_{s} \hbar X_{s,m_{s}}$$
$$[\hat S_{x}, \hat S_{y}] = i\hbar \hat S_{z}$$
- by ensuring the above pattern, it is found that:
$$\begin{gather}
\hat S_{x} = \frac{\hbar}{2} \begin{pmatrix}0&1\\1&0\end{pmatrix} = \frac{\hbar}{2} \hat\sigma_{x} \\
\hat S_{y} = \frac{\hbar}{2} \begin{pmatrix}0&-i\\i&0\end{pmatrix} = \frac{\hbar}{2} \hat\sigma_{y} \\
\hat S_{z} = \frac{\hbar}{2} \begin{pmatrix}1&0\\0&-1\end{pmatrix} = \frac{\hbar}{2} \hat\sigma_{z} \\
\end{gather}$$
$$\begin{gather}
\hat \sigma_{x}^{2} = \hat \sigma_{y}^{2} = \hat\sigma_{z}^{2} = \begin{pmatrix}1&1\\0&1\end{pmatrix} \\
\hat S^{2} = \hat S_{x}^{2} + \hat S_{y}^{2} + \hat S_{z}^{2}  = \frac{3\hbar^{2}}{4} \begin{pmatrix}1&0\\0&1\end{pmatrix}   \\
\hat S^{2} = \frac{1}{2}\left(\frac{1}{2}+1 \right)\hbar^{2} \begin{pmatrix}1&0\\0&1\end{pmatrix} \\
[\hat S^{2}, \hat S_{z}] = 0, \; \text{etc.}
\end{gather}$$
- this is the right pattern for an angular momentum with spin $=1/2$
``