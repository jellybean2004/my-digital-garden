---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h8-multidimensional-convolutions/","noteIcon":"1","created":"2025-08-27T13:15:23.803+01:00","updated":"2025-02-12T16:04:25.000+00:00"}
---

- in 2D:
$$\begin{gather}
f(x,y) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik_{x}x} \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik_{y}y} \tilde f(k_{x} , k_{y}) \, dk_{x} \, dk_{y} \\
f(k_{x},k_{y}) = \int_{-\infty}^{\infty} e^{-ik_{x}x} \int_{-\infty}^{\infty} e^{-ik_{y}y} f(k_{x} , k_{y}) \, dx \, dy \\
\end{gather}$$

- generalising to $N$ dimensions:
$$\begin{gather}
\vec r = (x_{1}, x_{2}, \dots x_{N}) \\
\vec k = (k_{1}, k_{2}, \dots k_{N}) \\\\
\tilde f(\vec k) = \int_{\mathbb R^{N}}  \exp(-i \vec k \cdot \vec r) f(\vec r)  \, d^{N} \vec r \\
f(\vec r) = \left(\frac{1}{2\pi}\right)^{N} \int_{\mathbb R^{N}} \exp(-i\vec k \cdot \vec r) \tilde f(\vec k)  \, d^{N} \vec k
\end{gather}$$- $\mathbb R^N$ indicates that there is a family of $N$ integrals, one for each $x_{i}:$
$$\int_{\mathbf R} d^{N}\vec r = \int_{x_{1}} \int_{x_{2}} \dots \int_{x_{N}}\,dx_{1}\, dx_{2}\dots dx_{N}$$
- therefore, $N$ dimensional convolutions are given by:
$$f*g(\vec r) = \int_{\mathbb R} f(\vec r) \, g(\vec r - \vec z) \, d^{N} \vec z$$

- considering a 2D gaussian:
$$\begin{gather}
f(x,y) = \frac{1}{2\pi\sigma^{2} }\exp\left(- \frac{x^{2}+y^{2}}{2\sigma^{2}}\right) \\
\tilde f(k_{x}, k_{y}) = \iint_{-\infty}^{\infty} \exp(-i(k_{x}x + k_{y}y)) f(x,y)\, dx\, dy \\
= \exp\left(\frac{1}{2} (k_{x}^{2} + k_{y}^ {2})\sigma^{2} \right)
\end{gather}$$
- so, the gaussian remains a gaussian after FT
- the variance in $k$-space is the inverse of the variance in $x$-space ($1/\sigma^{2}$)
