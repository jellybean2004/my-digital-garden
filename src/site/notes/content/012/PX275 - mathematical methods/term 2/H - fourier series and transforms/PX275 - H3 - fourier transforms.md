---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h3-fourier-transforms/","noteIcon":"1","created":"2025-01-29T13:57:02.491+00:00","updated":"2025-02-04T18:06:29.680+00:00"}
---

- considering a function defined over $x \in [-\infty, \infty]$, but it is not periodic
- eg: $f(x) = \exp(-x^{2})$

- considering the limit where the interval of periodicity, $L \to \infty$
$$f(x) = \sum\limits_{\{k\}} C_{k} \exp(ikx)$$
- the above is the sum of plane waves with wave number, $k = 2\pi n/L$
- the separation between $k$ values:
$$\delta k = \frac{2\pi}{L}$$
- as $L$ increases, $\delta k$ gets smaller and smaller
$$\lim_{L\to \infty} \delta k \to 0$$
- this forms a continuum of $k$
- the forward transform:
$$C_{k} = \frac{1}{L}\int_{-L/2}^{L/2}f(x) e^{-ikx}\,dx$$
- considering the limit:
$$\mathscr{F}(f(x)) = \int_{\infty}^{\infty} f(x) e^{-ikx}\,dx = \tilde f(k)  \bigg(= \lim_{L\to\infty} L C_{k}\bigg) $$
- this is defined to be the **fourier transform** of $f(x)$

$$\begin{align*}
f(x) &= \sum\limits_{\{k\}} C_{k}e^{ikx} \\ 
&= \sum\limits_{\{k\}}  \delta k \, \frac{L}{2\pi} C_{k} e^{ikx} \\ 
&= \frac{1}{2\pi} \sum\limits_{\{k\}}  L C_{k} e^{ikx}  \delta k\\ 
\end{align*}$$
- as $L \to \infty$, $\delta k \to 0 \to dk$

$$\lim_{L\to\infty} \frac{1}{2\pi} \sum\limits_{\{k\}}  L C_{k} e^{ikx}  \delta k = \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde f(k) e^{ikx}\, dk = f(x)$$
- this is defined as the **inverse fourier transform**
$$f(x) = \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde f(k) e^{ikx}\, dk$$

- fourier transforms map between 'real space', $x$, and the corresponding reciprocal 'fourier space', $k$
