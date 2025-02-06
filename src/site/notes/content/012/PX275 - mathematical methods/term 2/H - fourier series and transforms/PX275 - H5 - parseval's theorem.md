---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h5-parseval-s-theorem/","noteIcon":"1","created":"2025-02-06T14:21:47.936+00:00","updated":"2025-02-06T14:39:47.412+00:00"}
---


- considering the power/intensity:
$$I_{total} = \int_{\infty}^{\infty} |u(x)|^{2} \, dx$$
	where, $|u|^{2} = uu^{*}$
- using fourier transform:
$$u(x) = \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde u(k)\, e^{ikx} \, dk$$
$$\begin{align*}
I_{total}  &= \int_{-\infty}^{\infty} \underbrace{\frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde u(k)\, e^{ikx} \, dk}_{u(x)} \, \underbrace{\frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde u^{*}(k')\, e^{-ik'x} \, dk'}_{u^{*}(x)}\,dx \\
 &= \iiint_{-\infty}^{\infty} \frac{1}{2\pi}\frac{1}{2\pi} \tilde u(k)\tilde u^{*}(k')\, e^{i(k-k')x} \, dk\, dk'\,dx \\
 &= \iint_{-\infty}^{\infty} \frac{1}{2\pi} \tilde u(k) \tilde u^{*}(k') \delta(k-k')\,dk\,dk' \\
 &= \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde u^{*}(k') \tilde u(k')\,dk' \\
 \therefore I_{total} &= \frac{1}{2\pi} \int_{-\infty}^{\infty} |\tilde u(k)|^{2} \,dk
\end{align*}$$
- this result is known as **parseval's theorem:**
$$\int_{\infty}^{\infty} |u(x)|^{2} \,dx = \frac{1}{2\pi} \int_{-\infty}^{\infty} |\tilde u(k)|^{2} \,dk$$
- generalized as:
$$\int_{\infty}^{\infty} f(x)g^{*}(x) \,dx = \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde f(k) \tilde g^* (k) \,dk$$
