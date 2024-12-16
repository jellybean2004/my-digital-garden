---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-f-series/px-153-f3-estimating-the-sum-of-a-series/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:27.701+00:00"}
---

- consider the series $S= \sum\limits_{n-1}^{\infty} a_{n}$ where $a_{n}>0$
- suppose that $n>N$, we can write $a_{n}=f(n)$, where $n = N+1, N+2, ...$

- eg: for $S= \sum\limits_{n-1}^{\infty} \frac{1}{n^{2}}$, we assume that above some $N$, we can treat$f(n) = \frac{1}{n^{2}}$
	- here, $f(x)$ is a positive, decreasing, and continuous function for $N<x<\infty$
	- we then have: 
	$$S-S_{N} = \sum\limits_{n=N+1}^{\infty}f(n) \leq \int_{N}^{\infty} f(x).dx \equiv A_{N}$$
		- integral is the orange area in figure
	- similarly, we have 
	$$S-S_{N} \geq \int_{N+1}^{\infty}f(x).dx \equiv A_{N+1}$$
		- integral is the blue area in figure
		- it is translated by -1 in the x direction
	- ![Pasted image 20231114190024.png](/img/user/pics/Pasted%20image%2020231114190024.png)
	- thus, $A_{N+1} + S_{N} \leq S \leq A_{N}+S_{N}$
	$$S \approxeq S_{N} + \frac{1}{2}(A_{N}+A_{N+1})$$
- eg: estimate $S = \sum\limits_{n=1}^{\infty} \frac{1}{n^{2}}$ using the first five terms
		$S_{5} = 1 + \frac{1}{4} + \frac{1}{9} + \frac{1}{16} +\frac{1}{25}  = 1.464$
		$A_{5} = \int_{5}^{\infty} \frac{1}{x^{2}}.dx = [- \frac{1}{x}]_{5}^{\infty} = \frac{1}{5}$
		$A_{6} = \frac{1}{6}$
		$\implies 1.464 + \frac{1}{6} \leq S \leq 1.464 + \frac{1}{5}$
	- best guess: $S = 1.464 + \frac{1}{2}\left( \frac{1}{5}+ \frac{1}{6}\right)= 1.647$
	- actual value: $S = \frac{\pi^{2}}{6} = 1.645$
