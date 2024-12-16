---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j5-symmetric-and-antisymmetric-functions/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:39:36.310+00:00"}
---

- if $f(x) = f(-x): f(x)$ is symmetric. eg: $\cos{nx}$ 
- if $f(x) = -f(-x): f(x)$ is antisymmetric. eg: $\sin{nx}$ 

- for symmetric functions: $b_{n} =0 \, \forall \, n$
- for anti-symmetric functions: ${} a_{n} =0 \, \forall \, n$

- symmetric functions have only cosine terms, and anti-symmetric functions have only sine terms in their fourier series
## proof of the anti-symmetric case
$$\begin{align*}
	a_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi} f(x) \cos(nx)\,dx \\
	&= \frac{1}{\pi} \left[\int_{-\pi}^{0} f(x) \cos(nx)\,dx + \int_{0}^{\pi} f(x) \cos(nx)\,dx\right] \\\\
	&let\; x'=-x \implies dx' = -dx \\
	&= \frac{1}{\pi} \left[\int_{\pi}^{0} -f(x') \cos(nx')\,(-dx') + \int_{0}^{\pi} f(x) \cos(nx)\,dx\right] \\
	&= \frac{1}{\pi} \left[-\int_{0}^{\pi} f(x) \cos(nx)\,dx + \int_{0}^{\pi} f(x) \cos(nx)\,dx\right] \\
	&= 0 
\end{align*}$$
## proof for the symmetric case
$$\begin{align*}
	a_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi} f(x) \sin(nx)\,dx \\
	&= \frac{1}{\pi} \left[\int_{-\pi}^{0} f(x) \sin(nx)\,dx + \int_{0}^{\pi} f(x) \sin(nx)\,dx\right] \\\\
	&let\; x'=-x \implies dx' = -dx \\
	&= \frac{1}{\pi} \left[\int_{\pi}^{0} f(x') (-\sin(nx'))\,(-dx') + \int_{0}^{\pi} f(x) \sin(nx)\,dx\right] \\
	&= \frac{1}{\pi} \left[-\int_{0}^{\pi} f(x) \sin(nx)\,dx + \int_{0}^{\pi} f(x) \sin(nx)\,dx\right] \\
	&= 0 
\end{align*}$$