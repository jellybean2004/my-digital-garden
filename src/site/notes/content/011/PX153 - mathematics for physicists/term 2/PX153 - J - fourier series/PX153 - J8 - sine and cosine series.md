---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j8-sine-and-cosine-series/","noteIcon":"1","created":"2025-08-27T13:14:05.114+01:00","updated":"2024-12-03T17:16:45.000+00:00"}
---

- it is possible to use only sines or cosines:
- cosine series: 
$$f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}a_{n} \cos\left(\frac{n\pi x}{L}\right)$$
	for $x \in [0,L)$
- sine series: 
$$f(x) =  \sum\limits_{n=1}^{\infty}b_{n} \sin\left(\frac{n\pi x}{L}\right)$$ 
	for $x \in [0,L)$
- the only differences with full intervals:
	- $a_{n},\; b_{n},\; a_{0}$ coefficients will be calculated slightly differently
	- periodic extensions outside of $x \in [0,L)$ will be different
	- convergence properties
## periodic extensions
- can be evaluated $\forall x$
- periodic over $2\pi$, but only represent $f(x)$ in the interval $[0,L)$
- sine (odd) series has antisymmetric periodic extensions, and cosine (even) series has symmetric periodic extensions
![Pasted image 20240131115229.png](/img/user/pics/Pasted%20image%2020240131115229.png)

## finding the coefficients
- multiply by $\cos(\frac{n'\pi x}{L})$, then by $\sin(\frac{n'\pi x}{L})$, and integrate from $0$ to $L$
- eg: $b_{n}$ for sine series, taking the general case, $x \in [0,L)$
$$\begin{align*}
	& \int_{0}^{L}f(x)\, \sin\left(\frac{n'\pi x}{L}\right) \\
	&= \sum\limits_{n}b_{n} \int_{0}^{L} \sin\left(\frac{n\pi x}{L}\right) \sin\left(\frac{n'\pi x}{L}\right) dx \\\\
	&let \; x' = \frac{\pi x}{L} \implies dx' = \frac{\pi}{L}dx \\
	&= \sum\limits b_{n}\int_{0}^{\pi} \frac{L}{2\pi} (\cos((n-n')x') - \cos((n+n')x'))\,dx' \\
	&= \sum\limits_{n \neq n'} \frac{b_{n}L}{2\pi} \left[ \frac{\sin((n-n')x')}{n-n'} - \frac{\sin((n-n')x')}{n+n'}\right]_{0}^{\pi}\\
	&+ \frac{b_{n}L}{2\pi} \left[x' - \frac{\sin((n+n')x)}{n+n'}\right]\\
	&= \frac{b_{n}L}{2}
\end{align*}$$
$$b_{n} = \frac{2}{L}\int _{0}^{L} f(x)\, \sin\left(\frac{n'\pi x}{L}\right)\, dx$$
- similarly, 
$$\begin{align*}
	a_{n} &= \frac{2}{L} \int_{0}^{L} f(x)\,\cos\left(\frac{n'\pi x}{L}\right)\, dx\\
	a_{0} &= \frac{2}{L} \int_{0}^{L} f(x)\,dx
\end{align*}$$
- eg: $f(x) = \cos x$ for $x \in [0,\pi)$
	- cosine series: $f(x) = \cos(x)$
	- sine series: point-wise convergence 
$$\begin{align*}
	b_{n} &= \frac{2}{\pi} \int \cos x \, \sin(nx)\, dx \\
	&= \frac{2}{\pi} \int_{0}^{\pi} \frac{1}{2}(\sin((n+1)x)+ \sin((n-1)x))\,dx \\
	&= \frac{1}{\pi} \left[ -\frac{\cos((n+1)x)}{n+1} -\frac{\cos((n-1)x)}{n-1}\right]_{0}^{\pi} \\
	&= \frac{1}{\pi} \left[ \frac{-(-1)^{n+1}+1}{n+1} + \frac{-(-1)^{n-1}+1}{n-1}\right] \\
	&= \frac{1}{\pi}\left[ \frac{(-1)^{n}+1}{n+1} + \frac{(-1)^{n}+1}{n-1}\right]
\end{align*}$$
	- for $n \in even:$ 
$$b_{n} = \frac{1}{\pi} \left(\frac{2}{n+1} + \frac{2}{n-1}\right) = \frac{4n}{n^{2}-1}\left(\frac{1}{\pi}\right)$$
	- for $n\in odd:$ 
	$$b_{n}=0$$
$$\begin{align*}
		\cos x &= \frac{1}{\pi}\left( \frac{8}{3}\sin\left(2x\right) + \frac{16}{15}\sin(4x)+...\right)\\
		&= \sum\limits_{n=1}^{\infty} \frac{4n}{n^{2}-1} \frac{1}{\pi}\sin(nx), \;\;for\;n\in even
\end{align*}$$
