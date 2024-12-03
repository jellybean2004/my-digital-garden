---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j10-examples/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-03T17:17:16.186+00:00"}
---

## Q1
- *find the fourier series for $f(x)=x; \; x\in [0,2); \; f(x+2)=f(x)$*
- discontinuous at $x=0$
- point-wise convergence
- neither odd or even
$$\begin{align*}
	a_{0}&= \frac{1}{L}\int_{-L}^{L} f(x)\,dx \\
	 &= \frac{1}{1} \int_{0}^{2}x\,dx \\
	 &= 2
\end{align*}$$
$$\begin{align*}
	a_{n} &= \int_{0}^{2}x\cos\left(\frac{n\pi x}{L}\right)\,dx \\
	&= \left[\frac{x}{n\pi}\sin(n\pi x)\right]_{0}^{2} - \int_{0}^{2} \frac{1}{n\pi}\sin(n\pi x)\,dx \\
	&= \frac{1}{(n\pi)^{2}} [\cos(n\pi x)]_{0}^{2} \\
	&= \frac{1}{(n\pi)^{2}}(\cos(2n\pi)-1) \\
	&= 0
\end{align*}$$
$$\begin{align*}
	b_{n}&= \int_{0}^{2} x \sin(n\pi x)\,dx \\
	&= \frac{1}{n\pi}\left([x\cos(n\pi x)]_{0}^{2} - \int_{0}^{2} \cos(n\pi x)\, dx\right) \\
	&= - \frac{2}{n\pi}+ \left[\frac{\sin(n\pi x)}{(n\pi)^{2}}\right]_{0}^{2} \\
	&= -\frac{2}{n\pi}
\end{align*}$$
$$\therefore f(x) = 1 + \sum\limits_{n=1}^{\infty}(- \frac{2}{n\pi})\sin(n\pi x)$$
## Q2
- $f(x)= \cos(\alpha x); \; x \in [-\pi,\pi),\; \alpha\in\mathbb{R}$
- point-wise convergence
- symmetric $\implies b_{n}=0$
$$\begin{align*}
	a_{0} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\cos(\alpha x)\,dx \\
	&= \frac{2}{\pi}\int_{0}^{\pi} \cos(\alpha x)\,dx \\
	&= \frac{2}{\pi\alpha}[\sin(\alpha x)]_{0}^{\pi} \\
	&= \frac{2}{\alpha\pi} \sin(\alpha\pi)
\end{align*}$$
$$\begin{align*}
	a_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\cos(\alpha x)\cos(nx)\,dx \\
	&= \frac{2}{\pi}\int_{0}^{\pi} \frac{1}{2} \cos((\alpha+n) x)+\cos((\alpha-n)x)\,dx \\
	&= \frac{1}{\pi} \left[ \frac{\sin((\alpha+n)x)}{\alpha+n} + \frac{\sin((\alpha-n)x)}{\alpha-n}\right]_{0}^{\pi} \\
	&= \frac{1}{\pi} \left( \frac{\sin((\alpha+n)\pi)}{\alpha+n} + \frac{\sin((\alpha-n)\pi)}{\alpha-n}\right)
\end{align*}$$

## Q3
$$f(x) =\begin{cases}
 &0 & x \in [-\pi,- \frac{\pi}{2}) \\
 &1 & x \in [- \frac{\pi}{2},0) \\
 &-1 & x \in [0,\frac{\pi}{2}) \\
 &0 & x \in [\frac{\pi}{2}, \pi)
\end{cases}$$
- **sketch**: 
	![Pasted image 20240205140942.png](/img/user/pics/Pasted%20image%2020240205140942.png)
- **convergence**: point-wise
- **symmetries**: anti-symmetric
- **coefficients and series**:
	$$b_{n}= \frac{1}{\pi} \left(0+ \int_{- \frac{\pi}{2}}^{0} 1 \sin(nx)\, dx - \int_{0}^{\frac{\pi}{2}} 1 \sin(nx)\, dx + 0 \right)$$
	- let $x'=x$: 
$$\begin{align*}
b_{n} &= \frac{1}{\pi} \left( \int_{\frac{\pi}{2}}^{0} -\sin(nx')\, (-dx') - \int_{0}^{\frac{\pi}{2}} 1 \sin(nx)\, dx + 0 \right) \\
&= \frac{1}{\pi} \left(-\int_{0}^{\frac{\pi}{2}} \sin(nx)\, dx - \int_{0}^{\frac{\pi}{2}} \sin(nx)\, dx \right) \\
&= -\frac{2}{\pi}\int_{0}^{\frac{\pi}{2}}\sin(nx) \\
&= - \frac{2}{\pi} \left[- \frac{\cos(nx)}{n}\right]_{0}^{\frac{\pi}{2}} \\
&= \frac{2}{\pi n} \left[ \cos\left(\frac{n\pi}{2}\right)-1\right]_{0}^{\frac{\pi}{2}}
\end{align*}$$
$$\begin{align*}
n=1,5,9,... &: \cos\left(\frac{\pi}{2}\right)=0 & b_{n}=- \frac{2}{n\pi} \\
n=2,6,10,... &: \cos\pi=0 & b_{n}=- \frac{4}{n\pi} \\
n=3,7,11,... &: \cos\left(\frac{3\pi}{2}\right)=0 & b_{n}=- \frac{2}{n\pi} \\
n=4,8,12,... &: \cos(2\pi)=0 & b_{n}=0 \\
\end{align*}$$

## Q4
$f(x) = x$ in $[-\pi,\pi)$
- **sketch**: 
	![Pasted image 20240205141021.png](/img/user/pics/Pasted%20image%2020240205141021.png)
- **convergence**: point-wise (disconitinous at $x=-\pi$)
- **symmetries**: anti-symmetric, ie: $a_{0}=0$, $a_{n}=0$
- **coefficients and series**: $$\begin{align*}
	b_{n} &= \int_{-\pi}^{\pi} x\sin(nx)\,dx \\
	&= \frac{1}{\pi} \left[- \frac{\cos(nx)}{n}x\right]_{-\pi}^{\pi} - \frac{1}{\pi} \int_{-\pi}^{\pi}- \frac{\cos(nx)}{n}dx \\
	&= \frac{1}{\pi} \left(- \frac{\pi}{n} (-1)^{n} - \frac{\pi}{n}(-1)^{n} \right) \\&= \frac{2}{n} (-1)^{n+1}
\end{align*}$$
- fourier series: 
$$f(x) = 2\sin x - \frac{2}{2}\sin(2x) + \frac{2}{3}\sin(3x)- \frac{2}{{4}}\sin(4x)+...$$

- fourier series are useful for deriving interesting relations between numbers
## Q5
- from [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J3 - proofs and derivations#^feb2c0\|here]]: 
$$f(x) = |x| = \frac{\pi}{2}- \frac{4}{\pi}\left( \cos x + \frac{\cos{3x}}{9} + \frac{\cos{5x}}{25}+...\right)$$
- try $x=0$: 
$$\begin{align*}
	0 &= \frac{\pi}{2}- \frac{4}{\pi}\left(1 + \frac{1}{9}+ \frac{1}{25}+ ...\right) \\
	\frac{\pi^{2}}{8}&= 1+ \frac{1}{9}+ \frac{1}{25}+... \\
	\frac{\pi^{2}}{8} &= \sum\limits_{n=0}^{\infty} \frac{1}{(2n+1)^{2}}
\end{align*}$$
## Q6
- from [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J4 - periodic extensions#^2eaa23\|here]]: 
$$f(x) =x= 2\sin x - \frac{2}{2}\sin(2x) + \frac{2}{3}\sin(3x)- \frac{2}{{4}}\sin(4x)+...$$
- try $x = \frac{\pi}{2}$: 
$$\begin{align*}
	\frac{\pi}{2} &= 2\left(1- \frac{1}{3}+ \frac{1}{5}- \frac{1}{7}+ \frac{1}{9}+...\right)\\
	&= \sum\limits_{n={0}}^{\infty} \frac{(-1)^{n}}{2n+1}
\end{align*}$$