---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h1-complex-fourier-series/","noteIcon":"1","created":"2025-08-27T13:15:23.739+01:00","updated":"2025-03-21T08:10:34.000+00:00"}
---

[[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J1 - introduction\|PX153 - J1 - introduction]]

- the fourier series of a function that is periodic over $2L:$
$$f(x) = \frac{A_{0}}{2} + \sum\limits_{n=1}^{\infty}\left[A_{n} \cos \left(\frac{n\pi x}{L}\right) + B_{n}\sin \left(\frac{n\pi x}{L}\right)\right]$$
- for periodic over $L:$
$$f(x) = \frac{A_{0}}{2} + \sum\limits_{n=1}^{\infty}\left[A_{n} \cos \left(\frac{2n\pi x}{L}\right) + B_{n}\sin \left(\frac{2n\pi x}{L}\right)\right]$$

- using complex exponential notation:
$$\begin{gather}
\cos\theta  = \frac{e^{i\theta} + e^{-i\theta}}{2} \\
\sin\theta  = \frac{e^{i\theta} - e^{-i\theta}}{2i}
\end{gather}$$
- the fourier series can be written as:
$$\begin{gather}
f(x) = \frac{A_{0}}{2} + \sum\limits_{n=1}^{\infty} \left[ A_{n} \frac{1}{2}\big(e^{i2\pi nx/L}+e^{i2\pi nx/L} \big) + B_{n}  \frac{1}{2i}\big(e^{i2\pi nx/L}-e^{i2\pi nx/L} \big) \right]\\
f(x) = \frac{A_{0}}{2} + \sum\limits_{n=1}^{\infty} \left[ A_{n} \frac{1}{2}\big(e^{ikx}+e^{ikx} \big) + B_{n}  \frac{1}{2i}\big(e^{ikx}-e^{ikx} \big) \right]\\
= \frac{A_{0}}{2} + \sum\limits_{n=1}^{\infty} \left[e^{ikx}\left(\frac{A_{n}}{2} - \frac{iB_{n}}{2}\right) + e^{-ikx} \left(\frac{A_{n}}{2} + \frac{iB_{n}}{2}\right)\right]
\end{gather}$$
- the bracketed terms are complex coefficients, calling them $C_n$, and exploiting the symmetry:
$$f(x) = \sum\limits_{n=-\infty}^{\infty} C_{n}e^{ikx}$$
$$\begin{gather}
C_{0} = \frac{A_{0}}{2}  & n=0\\
C_{n}= \frac{A_{n}-iB_{n}}{2} & n\geq 1 \\
C_{-n} = \frac{A_{n}+iB_{n}}{2} & n \leq -1
\end{gather}$$
- this is the **complex fourier series**

- in physics, often only concerned with the real part
- if $f(x)$ is real valued, ie: $f(x) = f^{*}(x):$
$$\begin{gather}
f(x) = \sum\limits_{n=-\infty}^{\infty} C_{n}e^{ikx} \\
f^{*}(x) = \sum\limits_{n=-\infty}^{\infty} C_{n}^{*}e^{-ikx}
\end{gather}$$
- this requires:
$$\begin{gather}
C_{n}^{*} = C_{-n} \\
C_{-n}^{*} = C_{n}
\end{gather}$$
