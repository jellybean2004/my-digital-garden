---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-f-series/px-153-f1-taylor-series/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:24.073+00:00"}
---

- taylor's theorem gives a way of expressing functions as a power series
- it uses the derivatives of a function to approximate its value around a point
$$\frac{df}{dx}|_{x=a}\simeq \frac{f(a+\Delta x)-f(a)}{\Delta x}$$
- for small $\Delta x$: 
$$f(a+\Delta x) \simeq f(a) + \frac{df}{dx}|_{x=a} \Delta x$$
- make a more accurate approximation by adding higher order derivatives. let's assume that we can approximate the function as a power series, a polynomial in $(x-a)$, that will be valid for some interval around $x=a$, ie: 
$$f(x=a)\simeq A_{0} + A_{1(x-a)} + A_{2}(x-a)^{2}+ A_{3}(x-a)^{3}+...$$
$$f(x=a)\simeq A_{0}+ \sum\limits _{n=1}^{N} A_{n}(x-a)^{n}$$ where $A_{0}$, $A_{1}$, $A_{2}...A_{n}$ are constants we must find
$$\frac{df}{dx}= A_{1}+ 2A_{2}(x-a) + 3A_{3}(x-a^{2})+...$$
$$\frac{d^{2}f}{dx^{2}} = 2A_{2} + 3.2.A_{3}(x-a)+ 4.3.A_{4}(x-a)^{2}+...$$
- evaluate these at $x=a$, allows us to find $A_{0}$, $A_{1}$, $A_{2}$, etc
$$f(x) \simeq f(a) + f'|_{x=a}(x-a) + \frac{1}{2!} f''|_{x=a}(x-a)^{2}+...+ \frac{1}{n!} f^{n'}|_{x=a}(x-a)^{n}$$
$$f(x)\simeq f(a) + \sum\limits_{n=1}^{\infty}\frac{1}{n!} f^{n'}|_{x=a}(x-a)^{n}$$ 
- $\frac{1}{n!} f^{n'}|_{x=a} = A_{n}$ is just a number 
- this is the *taylor expansion* of $f(x)$
- if $a=0$, this is the *maclaurin expansion*

- eg: find the firs 3 non-zero terms of the taylor expansion of $f(x)=\sin x$ about $x=0$ (ie: maclaurin expansion)
		$$f(x) = \sin x \simeq \sin 0 + \sum\limits_{n=1}^{\infty}\frac{1}{n!} f^{n'}|_{x=a}(x)^{n}$$
			$f(0) = \sin 0 = 0$
			$f'(0) = \cos(0) = 1$
			$f''(0)= -\sin(0) = 0$
			$f'''(0)= -\cos(0) = -1$
			$f'''(0)= -\cos(0) = -1$
			$f^{4'}(0)= \sin(0) = 0$
			$f^{5'}(0)= \cos(0) = 1$
	$$\implies \sin x = x - \frac{1}{3!} x^{3}+ \frac{1}{5!}x^{3}+...$$
	- $\sin x$ is an *odd function*, so, we only have odd powers of $x$
	- **note**: $x$ is in $radians$

- eg: estimate the value of $\cos 62\degree$ by expanding $\cos x$ around $60\degree$
	- switch to radians: $60\degree = \frac{\pi}{3}$, $62\degree - 60\degree = 2\degree = \frac{\pi}{90}$
		$$\cos\left(\frac{\pi}{3} + \frac{\pi}{90}\right) \simeq \cos (\frac{\pi}{3}) + \sum\limits_{n=1}^{\infty}\frac{1}{n!} f^{n'}|_{\frac{\pi}{3}}(\frac{\pi}{90})^{n}$$
		$\cos(\frac{\pi}{3})=\frac{1}{2}$
		$f'(\frac{\pi}{3}) = \frac{-\sqrt{3}}{2}$
		$f''(\frac{\pi}{3}) = \frac{-1}{2}$
		$f'''(\frac{\pi}{3}) = \frac{\sqrt{3}}{2}$
	$$\cos62\degree \simeq \frac{1}{2}- \frac{\sqrt{3}}{2}\left(\frac{\pi}{90}\right)- \frac{1}{2!} \frac{1}{2} (\frac{\pi}{90})^{2}+...$$
		$$\cos 62\degree \simeq  0.5-0.302-00003+... \simeq 0.4695$$
		(accurate to 4 sf)

- a useful trick is the relationship the derivative/integral of the taylor series is equal to the derivative/integral of the function
- if the expansion is around $0$, you can find the expansion of a power of the independent variable (eg: $x^{3}$), by substituting it into the taylor expansion of the function of $x$
- eg: if you want to find the expansion of $\sin x^{3}$ about $x=0$, find the expansion for $\sin x$ and replace $x$ with $x^3$ 
$$\implies \sin x^{3} = x^{3} + \frac{x^{9}}{3!} + \frac{x^{15}}{5!}+...$$
## non analytical function
- every differential is zero