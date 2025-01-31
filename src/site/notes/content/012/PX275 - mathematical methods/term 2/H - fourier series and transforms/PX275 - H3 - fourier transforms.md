---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h3-fourier-transforms/","noteIcon":"1","created":"2025-01-29T13:57:02.491+00:00","updated":"2025-01-30T14:02:18.923+00:00"}
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

- eg: $f(x) = \delta(x-y)$
$$\tilde f(k) = \int_{-\infty}^{\infty} \delta(x-y) e^{-ikx}\,dx = e^{-iky}$$
- **note:** for $y = 0$, $\tilde f(x) = 1$

$$f(x) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik(x-y)} dk = \delta(x-y)$$

- this gives another way to define the [[content/012/PX275 - mathematical methods/term 2/G - partial differential equations/PX275 - G7 - dirac delta function\|dirac delta function]] as a fourier transform of a complex exponential
$$\delta (x - y) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik(x-y)}\,dk$$

$$\begin{align*}
\tilde f(x) &= \mathscr F(f(x)) \\
f(x) &= \mathscr F^{-1}(\tilde f(x)) \\
\therefore f(x) &= \mathscr F^{-1} (\mathscr F(f(x)))
\end{align*}$$
- checking:
$$\begin{align*}
f(x) &= \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde f(k) e^{ikx}\, dk \\
&= \underbrace{\frac{1}{2\pi} \int_{-\infty}^{\infty}e^{ikx}\, dk}_{\mathscr F^{-1}(\tilde f(k))} \; \underbrace{\int_{-\infty}^{\infty} f(x') e^{-ikx'} \,dx'}_{\mathscr F(f(x'))} \\
&=  \frac{1}{2\pi} \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{ik(x-x')} f(x') \, dx'\,dk \\
&= \int_{-\infty}^{\infty}  f(x') \delta(x-x')\,dx'\\
&= f(x)
\end{align*}$$

- using a different normalization:
$$\begin{gather}
\tilde f(k) = \frac{1}{a} \int_{-\infty}^{\infty} f(x) e^{-ikx} \,dx \\ 
f(x) = \frac{a}{2\pi} \int_{-\infty}^{\infty} \tilde f(x) e^{ikx}\,dk
\end{gather}$$

- $a = 1$ was chosen, but a popular choice is $a = \sqrt{2\pi}$
	$\cfrac{1}{a}= \cfrac{1}{\sqrt{2\pi}}$
	$\cfrac{a}{2\pi} = \cfrac{1}{\sqrt{2\pi}}$
- so, both the transforms have the same prefactor

$$\begin{align*}
\mathscr F(\delta(x-y)) &= e^{iky} \\ \mathscr F(\delta(x)) &= 1
\end{align*} $$

- eg: $f(x) = 1 \; \forall x$
$$\tilde f(k) = \int_{-\infty}^{\infty} e^{-ikx}\,dx$$
- from the definition of $\delta(x-y)$, and setting $x - y \to -q$, a dummy variable
$$\delta(-q) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{-ikq}\,dk = \delta(q)$$

- now, $k \to x':$
$$\begin{gather}
\delta(q) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{-iqx'} \,dx' \\
2\pi \delta(q) = \int_{-\infty}^{\infty} e^{-iqx'} \,dx'
\end{gather}$$
- finally, $q \to k:$
$$\int_{-\infty}^{\infty} e^{-ikx} \,dx = 2\pi \delta(k)$$

- eg: the step function:
$$f(x) = \begin{cases}
0 & a < x < b, \\
1 & \text{elsewhere.}
\end{cases}$$
$$\begin{align*}
\tilde f(k) &= \int_{a}^{b} e^{-ikx}\,dx \\ 
&= -\frac{1}{ik} [e^{-ikx}]_{a}^{b} \\
&= -\frac{1}{ik}( e^{-ikb} - e^{-ika}) \\
\end{align*}$$
- if $a = -b:$
$$\begin{align*}
\tilde f(k) &= \frac{1}{ik} (e^{ikb} - e^{-ikb}) \\
&= \frac{2}{k}\sin kb \\
&= 2b  \frac{\sin{kb}}{kb} \\ 
&= 2b \, \text{sinc}\,{kb}
\end{align*}$$

![[Pasted image 20250130125154.png\|500]]
*image: Georg-Johann*

