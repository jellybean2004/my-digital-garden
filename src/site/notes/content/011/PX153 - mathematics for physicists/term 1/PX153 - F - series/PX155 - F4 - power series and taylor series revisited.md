---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-f-series/px-155-f4-power-series-and-taylor-series-revisited/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:28.403+00:00"}
---

\- ***taylor's theorem***: if $f(x)$ is a continuous, single-valued function of $x$ with continuous derivatives $f'(x), f''(x)... f^{(n)}(x)$, in a given interval $a \leq x \leq b$, and if $f^{(n+1)}(x)$ also exists in this interval, then: 
$$f(x) = f'(a)(x-a) + \frac{1}{2!} f''(a)(x-a)^{2} +...+  \frac{1}{n!} f^{(n)}(a)(x-a)^{n} + E_{n}(x)$$
		where, $E_{n}(x)$ is a remainder term which describes the error in the approximation of $f(x)$ by the power series of $n+1$ terms.
	- if $\lim_{n\to\infty} E_{n}(x) = 0$, then $f(x)$ can be represented by a *power series*, that is a *taylor series*
- let's look again at the convergence of a power series. let $y(x)$ be a function that can be described as a power series: 
$$y(x) = b_{0} + b_{1}x + b_{2}x^{n}+...+ b_{n}x^{n} = \sum\limits_{n=0}^{\infty} b_{n}x^{n}$$
- use ratio to determine convergence: $k = \lim_{n\to\infty} |\frac{b_{n+1}x^{n+1}}{b_{n}x^{n}}|= lim_{n\to\infty} |x| | \frac{b_{n+1}}{b_{n}}| <1$ for convergence
	$\implies |x| < \lim_{n\to\infty} | b_{n}/b_{n+1}|$    radius of convergence
	or,
	$- \lim_{n\to\infty} | \frac{b_{n}}{b_{n+1}} | < x <  \lim_{n\to\infty} | \frac{b_{n}}{b_{n+1}}|$
	