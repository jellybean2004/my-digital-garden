---
dg-publish: true
---

- [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J1 - introduction#^04a8fb\|Q]] : given a function, $f(x)$, how can $a_{0}$, $a_{n}$, and $b_{n}$ be calculated?
	- orthogonality relations:
		(1) 
		$$\int_{-\pi}^{\pi} \sin nx \cos mx \,dx =0$$
			where, $n,m \in \mathbb Z$
		(2) 
		$$\int_{-\pi}^{\pi} \sin nx \sin mx \,dx =\begin{cases}
		0 & n\neq m \\
		\pi & n=m
		\end{cases}$$
		(3) 
		$$\int_{-\pi}^{\pi} \cos nx \cos mx \,dx =\begin{cases}
		0 & n\neq m \\
		\pi & n=m
		\end{cases}$$
	- trigonometric identities: 
		$(a):\cos\alpha\cos\beta = \frac{1}{2}(\cos(\alpha+\beta)+ \cos(\alpha-\beta))$
		$(b):\sin\alpha\sin\beta = \frac{1}{2}(\cos(\alpha-\beta)- \cos(\alpha+\beta))$
		$(c): \sin\alpha\cos\beta = \frac{1}{2}(\sin(\alpha+\beta)+\sin(\alpha-\beta))$
## proofs of relations
(1) 
$$I_{1} = \int_{-\pi}^{\pi} \sin nx \cos mx \,dx$$
- using relation $(c):$ 
$$\begin{align*}
	I_{1} &= \frac{1}{2} \int_{-\pi}^{\pi} (\sin[(n+m)x]+\sin[(n-m)x])\,dx \\
	&= \frac{1}{2} \left[ \frac{-\cos[(n+m)x]}{n+m} - \frac{\cos[(n-m)x]}{n-m} \right]_{-\pi}^{\pi} \\
	&= 0 
\end{align*}$$
$$I_{2} = \int_{-\pi}^{\pi} \sin nx \sin mx \,dx$$
- using relation $(b):$ 
$$I_{2} = \frac{1}{2} \int_{-\pi}^{\pi} (\cos[(n-m)x] - \cos[(n+m)x])\,dx$$
- when $n\neq m:$ 
$$\begin{align*}
	I_{2} &= \frac{1}{2} \left[ \frac{\sin[(n-m)x]}{n-m} - \frac{\sin[(n+m)x]}{n+m} \right]_{-\pi}^{\pi} \\ 
	&= 0
\end{align*}$$
- when $n=m:$ 
$$\begin{align*}
	I_{2} &= \frac{1}{2}\int_{-\pi}^{\pi} (1-\cos(2nx)) \,dx \\
	&= \frac{1}{2} \left[x-\frac{\sin(2nx)}{2n}\right]_{-\pi}^{\pi} \\
	&= \pi
\end{align*}$$
(3) 
$$I_{3} = \int_{-\pi}^{\pi} \cos nx \cos mx \,dx$$
- using relation $(a):$ 
$$\begin{align*}
	I_{3} &= \frac{1}{2} \int_{-\pi}^{\pi} (\cos[(n+m)x] + \cos[(n-m)x])\,dx \\
	&= \frac{1}{2} \left[ \frac{\sin[(n+m)x]}{n+m} + \frac{\sin[(n-m)x]}{n-m} \right]_{-\pi}^{\pi} \\
\end{align*}$$
- when $n\neq m:$ 
$$I_{3} = 0$$
- when $n=m:$ 
$$I_{3} =\pi$$
## finding constants
$$f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty} [a_{n}\cos(nx) + b_{n}\sin(nx)]$$
- integrating both sides: 
$$\int_{-\pi}^{\pi} f(x)\, dx = \left[ \frac{a_{0}x}{2} + \sum\limits_{n=1}^{\infty} \left[\frac{a_{n}\sin(nx)}{n} - \frac{b_{n}\cos(nx)}{n}\right] \right]_{-\pi}^{\pi} = a_{0}\pi$$
$$\frac{a_{0}}{2} = \frac{1}{2\pi} \int_{-\pi}^{\pi} f(x)\,dx$$
- now, multiplying by $\cos(mx)$ and integrating over $x$: 
$$\begin{align*}
	\int_{-\pi}^{\pi} f(x) \cos(mx) \, dx &= \left[\frac{a_{0}x}{2} \frac{\sin(mx)}{m}\right]_{-\pi}^{\pi} + \sum\limits_{n=1}^{\infty} \left(a_{n} \int_{-\pi}^{\pi} \cos(nx) \cos(mx) \,dx  + b_{n} \int_{-\pi}^{\pi} \sin(nx) \cos(mx)\,dx \right) \\
	&= a_{m}\pi
\end{align*}$$
	- because: 
	$$\left[\frac{a_{0}x}{2} \frac{\sin(mx)}{m}\right]_{-\pi}^{\pi} =0$$
		- from relation $(3):$ 
		$$\int_{-\pi}^{\pi} \cos(nx) \cos(mx) \,dx = \begin{cases}
	0 & n\neq m \\ \pi & n=m
	\end{cases}$$
		- from relation $(1):$ 
		$$\int_{-\pi}^{\pi} \sin(nx) \cos(mx)\,dx = 0$$
$$\therefore a_{n}= \frac{1}{\pi}\int_{-\pi}^{\pi} f(x) \cos(mx)\,dx$$
- finally, multiplying by $\sin(mx)$ and integrating over $x$: 
$$\begin{align*}
	\int_{-\pi}^{\pi} f(x) \sin(mx) \, dx &= \left[\frac{a_{0}x}{2} \frac{\cos(mx)}{m}\right]_{-\pi}^{\pi} + \sum\limits_{n=1}^{\infty} \bigg(a_{n} \int_{-\pi}^{\pi} \cos(nx) \sin(mx) \,dx  \\ 
	&+ b_{n} \int_{-\pi}^{\pi} \sin(nx) \sin(mx)\,dx\bigg) \\
	&= a_{m}\pi
\end{align*}$$
	- because: 
	$$\left[\frac{a_{0}x}{2} \frac{\cos(mx)}{m}\right]_{-\pi}^{\pi}=0$$
		- from relation $(1):$ 
		$$\int_{-\pi}^{\pi} \cos(nx) \sin(mx) \,dx =0$$
		- from relation $(2):$ 
		$$\int_{-\pi}^{\pi} \sin(nx) \sin(mx)\,dx = \pi$$
		for $m=n$
$$\therefore b_{n} = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin(nx)\,dx$$
## summary
$$\begin{align*}
	\frac{a_{0}}{2} &= \frac{1}{2\pi} \int_{-\pi}^{\pi} f(x)\,dx \\
	a_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi} f(x) \cos(nx)\,dx \\
	b_{n} &= \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin(nx)\,dx
\end{align*}$$
- eg: $f(x) = |x|$ in $[-\pi,\pi]$
$$f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}\left(a_{n}\cos\left(\frac{n\pi x}{L}\right) +b_{n}\sin\left(\frac{n\pi x}{L}\right) \right)$$
$$\begin{align*}
	\frac{a_{0}}{2} &= \frac{1}{2\pi} \int_{-\pi}^{\pi} |x|\,dx \\
	&= \frac{1}{2\pi} \left(\int_{0}^{\pi} x\,dx + \int_{-\pi}^{0} -x\,dx\right) \\
	&= \frac{1}{2\pi} \left(2\int_{0}^{\pi} x\,dx\right) \\
	&= \frac{\pi}{2}
\end{align*}$$
$$\begin{align*}
	a_{n} &= \frac{1}{\pi} \left[\int_{-\pi}^{0} -x \cos(nx)\,dx + \int_{0}^{\pi} x\cos(nx)\,dx \right] \\\\
	&let\; x'=-x \implies dx'=-dx\\
	&= \frac{1}{\pi} \left[\int_{\pi}^{0} x' \cos(-nx)\,(-dx') + \int_{0}^{\pi} x\cos(nx)\,dx \right] \\
	&= \frac{1}{\pi} \left[\int_{0}^{\pi} x' \cos(-nx)\,dx' + \int_{0}^{\pi} x\cos(nx)\,dx \right] \\
	&= \frac{1}{\pi} \left[\int_{0}^{\pi} x \cos(-nx)\,dx + \int_{0}^{\pi} x\cos(nx)\,dx \right] \\
	&= \frac{2}{\pi}\int_{0}^{\pi} x \cos(-nx)\,dx \\
	&= \frac{2}{\pi} \left[\frac{x\sin{nx}}{n}\right]_{0}^{\pi}- \int\frac{2}{\pi} \frac{\sin{nx}}{n}dx \\
	&= - \frac{2}{\pi} \left[\frac{-\cos{nx}}{n^{2}}\right]_{0}^{\pi} \\
	&= \frac{2}{n^{2}\pi} ((-1)^{n}-1) \\
	\therefore a_{n}&= \begin{cases}
	-\frac{4}{n^{2}\pi} & n\in odd \\
	0 & n\in even
\end{cases}
\end{align*}$$
$$\begin{align*}
	b_{n} &= \frac{1}{\pi} \left[\int_{-\pi}^{0} -x \sin(nx)\,dx + \int_{0}^{\pi} x \sin(nx)\,dx \right ] \\
	&= \frac{1}{\pi} \left[\int_{\pi}^{0} x' \sin(nx')\,dx' + \int_{0}^{\pi} x \sin(nx)\,dx \right ] \\
	&= \frac{1}{\pi} \left[\int_{\pi}^{0} x' \sin(-nx')\,(-dx') + \int_{0}^{\pi} x \sin(nx)\,dx \right ] \\
	&= \frac{1}{\pi} \left[-\int_{0}^{\pi} x' \sin(nx')\,dx' + \int_{0}^{\pi} x \sin(nx)\,dx \right ] \\
	&= \frac{1}{\pi} \left[-\int_{0}^{\pi} x \sin(nx)\,dx + \int_{0}^{\pi} x \sin(nx)\,dx \right ] \\
	&= 0
\end{align*}$$
$$\therefore f(x) = |x| = \frac{\pi}{2}- \frac{4}{\pi}\left( \cos x + \frac{\cos{3x}}{9} + \frac{\cos{5x}}{25}+...\right)$$

{ #feb2c0}
