---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-f-series/px-153-f2-convergence-of-a-series/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:25.931+00:00"}
---

- in general, a series is just a sum of terms: 
$$S = a_{1} + a_{2} + a_{3} + ... = \sum\limits_{n=1}^{N}a_{n}$$
## convergence
- some infinite series converge to a finite value, and some diverge
- eg:
	- $S_{1} = \sum\limits_{n=1}^{\infty} \frac{1}{n^{2}}= \frac{\pi^{2}}{6}$ : converges
	- $S_{2} = \sum\limits_{n=1}^{\infty} \frac{1}{n} \to\infty$ : diverges
- a series with $N$ terms, $S_{N} = \sum\limits_{n=1}^{N}a_{n}$, is convergent if $\lim_{N\to\infty}S_{N}$ exists and is finite
	- else, it is divergent
- sometimes we can determine whether a series will converge by algebraic manipulation: 
$$S_{N} = \sum\limits_{a=0}^{N} x^{n}$$
	- multiply both sides by $x$: 
	$$xS_{N} = \sum\limits_{n=1}^{N+1} x^{n} = S_{N} - 1 + x^{N+1}$$
	$$(x-1)S_{N} = x^{N+1} - 1$$
	$$\therefore S_{N}= \frac{x^{N+1}-1}{1-x}$$
	- for large $N$, this gives $S_{N}\to \frac{1}{1-x}$, provided $|x|<1$. hence, this power series converges if $-1<x<1$. this is the *interval of convergence*
	- the *radius of convergence* is half of the interval: $R = 1$, that is $|x|<1$
	- this is an example of a geometric series. more generally: 
	$$S_{N} = \sum\limits_{n=0}^{N} ar^{n}$$
	- following the same argument, this converges for $|r|<1, \; \lim{N\to\infty}r^{N}=0$ and the sum tends to $S=\frac{a}{1-r}$
## tests for convergence
- $f(x)$ must be *continuous* and *differentiable*
### preliminary test
- simple, but not conclusive
- a series, $S = \sum\limits_{n=1}^{\infty}a_{n}$, cannot converge unless $\lim_{n\to\infty}a_{n}=0$
- this is necessary, but insufficient condition for convergence
- eg: $S = \sum\limits_{n=1}^{\infty} \frac{1}{n}$ diverges despite $\lim_{n\to\infty} \frac{1}{n}=0$
### comparison test
- if $S_{1}= \sum\limits_{n-1}^{\infty} a_{n}$ is a series of positive terms, and $S_{2} = \sum\limits_{n=1}^{\infty} b_{n}$ is also a series of positive terms, then $S_1$ converges if $a_{n}\leq b_{n}$ for large $n$
- conversely, if $a_{n} \geq b_{n}$ for large $n$, and $S_2$ diverges, then $S_1$ diverges
- eg: does $S_{n} = \sum\limits_{n=1}^{\infty} \frac{1}{n(n+1)}$ converge?
	- since $\frac{1}{n(n+1)} < \frac{1}{n^{2}}$ for all $n \geq 1$, by the comparison test, $S_1$ converges
### the ratio test (d'alembert's method)
- the ratio test states that for $S_{1}= \sum\limits_{n-1}^{\infty} a_{n}$ ;  $\lim_{n\to\infty} |\frac{a_{n+1}}{a_{n}}|= k$
	- if $k<1$: converges
	- if $k>1$: diverges
	- if $k=1$: inconclusive
- proof: 
	- consider $S= \sum\limits_{n-1}^{\infty} a_{n}$
	- such that $\lim_{n\to\infty} |\frac{a_{n+1}}{a_{n}}|= k <1$
	- as $k<1$, for the $N^{th}$ term, and beyond, in the series, there is a value of $r$, where $k<r<1$ and $\frac{a_{n+1}}{a_{n}}< r$ for all $n>N$
	- the terms in the series, $a_N$, $a_{N+1}$, $a_{N+2}$, $...$, are all less than $ra_{N} + r^{2}a_{N} + r^{3}a_{N}+...$
	- this is a geometric series with $r<1$, so, it converges. 
	- by the comparison test, $S$ converges as well

- eg: does $S = \sum\limits_{n=1}^{\infty} \frac{1}{n2^{n}}$ converge?
	- preliminary test: 
	$$\lim_{n\to \infty} = 0$$
		- passed
	- ratio test: 
	$$\lim_{n\to \infty} | \frac{1}{(n+1)2^{n+1}} n2^{n} | = \lim_{n\to \infty} | \frac{n}{2(n+1)} | = \lim_{n\to \infty} | \frac{1}{2} (1 + \frac{1}{n}) |$$
	$$\lim = \frac{1}{2} = k$$
		- since $k<1$, $S$ converges
### alternating series test
- if $S= \sum\limits_{n-1}^{\infty} a_{n}$ is a series with terms alternate in sign, and if the terms are continuously diminishing, with $\lim_{n\to \infty} = 0$, then the series will converge