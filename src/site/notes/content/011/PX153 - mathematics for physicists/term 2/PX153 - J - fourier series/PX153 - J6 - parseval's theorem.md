---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j6-parseval-s-theorem/","noteIcon":"1","created":"2025-08-27T13:14:05.125+01:00","updated":"2024-11-26T19:39:41.000+00:00"}
---

- if $f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}\left(a_{n}\cos(nx) +b_{n} \sin(nx) \right)$, then, $$\frac{1}{\pi} \int_{-\pi}^{\pi} (f(x))^{2}\,dx = \frac{a_{0}^{2}}{2} + \sum\limits_{n=1}^{\infty} (a_{n}^{2}+ b_{n}^{2})$$
- application in physics: physical waves
- if the energy of a wave is the square of the wave function,  the sum of $a_{n}^{2}$, $b_{n}^{2}$, $\frac{a_{0}^{2}}{2}$ is the sum of the energy of individual vibration modes.
$$\begin{align*}
\frac{1}{\pi} \int_{-\pi}^{\pi} |f(x)|^{2}\,dx &= \frac{1}{\pi} \int_{-\pi}^{\pi} \bigg[\frac{a_{0}^{2}}{4} + \left(\sum\limits_{n} (a_{n}\cos nx + b_{n}\sin nx) \right)^{2} \\
&+ 2\, \frac{a_{0}}{2}\,\sum\limits_{n} (a_{n}\cos nx + b_{n}\sin nx) \bigg]\,dx \\
&= \frac{1}{\pi} \int_{-\pi}^{\pi} \bigg[\frac{a_{0}^{2}}{4} + \left(\sum\limits_{n} (a_{n}\cos nx + b_{n}\sin nx) \right)  \\
& \times \left(\sum\limits_{n'} (a_{n'}\cos n'x + b_{n'}\sin n'x) \right) \bigg]\,dx \\
&= \frac{a_{0}^{2}}{2} + \sum\limits_{n} (a_{n}^{2} + b_{n}^{2})\\
\end{align*}$$

- for a complex fourier series, $f(x)^{2} = f(x)f(x)^{*}$
 ![Pasted image 20240205140904.png](/img/user/pics/Pasted%20image%2020240205140904.png)