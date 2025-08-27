---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j2-convergence/","noteIcon":"1","created":"2025-08-27T13:14:05.107+01:00","updated":"2024-12-03T17:12:51.000+00:00"}
---

- let $L=\pi$ : 
$$f_{N}(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty} (a_{n}\cos(nx) + b_{n}\sin(nx))$$
for $-\pi\leq x \leq\pi$
## minimum requirement (convergence in the mean)
- any function for which $\int_{-\pi}^{\pi} (f(x))^{2}\,dx < \infty$ can be expressed as a fourier series
- a weak form of convergence: 
$$\lim_{N\to\infty}f_{N}(x) \neq f(x)$$
at all $-\pi \leq x \leq \pi$
## point-wise convergence
- if $f(x)$ and $f'(x)$ are continuous at $[-\pi,\pi)$, except possibly at a finite number of points, the fourier series converges at every point, $\tilde f(x) = \frac{1}{2}(f(x^{+})+f(x^{-}))$, where, $f(x^{+})= \lim_{\epsilon\to0}f(x+\epsilon)$, $f(x^{-})= \lim_{\epsilon\to0}f(x-\epsilon)$, and $\epsilon$ is a scalar

- eg: 
$$\lim_{N\to\infty} f_{N}(x) = {} \tilde f(x) = \frac{1}{2}(f(x^{+})+f(x^{-})) {}$$
	- at discontinuities, the series converges to the midpoints

- what happens at the boundaries? ie: at $x=\pi$ and $-\pi$
	- **note**: 
	$$f_{N}(x+2\pi) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty} (a_{n}\cos(nx+2\pi) + b_{n}\sin(nx+2\pi))$$
	$$f_{N}(\pi) = f_{N}(-\pi+2\pi) = f_{N}(-\pi)$$
$$\begin{align*}
	\lim_{N\to\infty} f_{N}(-\pi) &= \lim_{\epsilon\to0} \frac{1}{2}[f(-\pi+\epsilon)+f(-\pi-\epsilon)] \\
	&= \lim_{\epsilon\to0} \frac{1}{2}[f(-\pi+\epsilon)+f(\pi-\epsilon)]
\end{align*}$$
	- so, the series converges at the average of the original function at the boundaries
## uniform convergence
- if $f(x)$ and $f'(x)$ exist and are continuous everywhere in $[-\pi,\pi)$, and $f(\pi) = f(-\pi)$, the fourier series converges uniformly to $f(x)$
- $|f(x)-f_{N}(x)|$ has a maximum value within $[-\pi,\pi)$ for given $N$, which is useful if $1\%$ precision is needed, and $\lim_{N\to\infty}|f(x)-f_{N}(x)|=0$

- [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J1 - introduction#^142629\|why is this needed?]]
	- sines and cosines are well behaved (differentiate and integrate infinite number of times), and are easy to work with
	- natural separation between slowly varying terms with $x$ (small $n$), and rapidly varying terms with $x$ (large $n$)
	- many systems in physics involve waves. eg: light, particles in QM, electronics, signal propagation, etc
