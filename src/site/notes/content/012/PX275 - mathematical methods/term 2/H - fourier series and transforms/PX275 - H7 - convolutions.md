---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h7-convolutions/","noteIcon":"1","created":"2025-02-06T17:38:21.978+00:00","updated":"2025-02-08T12:19:19.518+00:00"}
---

- the convolution of two functions, $f$ and $g$, is defined as:
$$f * g (x) = \int_{-\infty}^{\infty} f(y)\,g(x-y)\,dy$$
![convgaus.gif|500](/img/user/pics/convgaus.gif)
*image: Wolfram*

## fourier transform of a convolution
$$\mathscr{F}(f*g(x)) = \int_{-\infty}^{\infty} fg(x)e^{-ikx}\,dx = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty} f(y)*g(x-y)e^{-ikx}\,dx\,dy$$

- $g(x-y)$ can be rewritten as an inverse fourier transform:
$$g(x-y) = \frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde g(k') e^{ik'(x-y)} \,dk'$$
- substituting it into the transform:
$$\begin{align*}
\mathscr{F}(f*g(x)) &= \int_{-\infty}^{\infty} e^{-ikx} \int_{-\infty}^{\infty} f(y)\frac{1}{2\pi} \int_{-\infty}^{\infty} \tilde g(k') e^{ik'(x-y)} \,dk'\,dx\,dy \\
&= \iiint_{-\infty}^{\infty} \frac{1}{2\pi} e^{ix(k-k')} \,dx \, f(y) \tilde g(k') e^{-ik'y} \,dk'\,dy \\
&= \iint_{-\infty}^{\infty} \delta(k-k') \, f(y) \tilde g(k') e^{-ik'y} \,dk'\,dy \\
&= \int_{-\infty}^{\infty}  f(y) \tilde g(k) e^{-iky} \,dy \\
&= \tilde g(k) \int_{-\infty}^{\infty}  f(y) e^{-iky} \,dy \\
\therefore \mathscr{F}(f*g(x))&= \tilde g(k) \tilde f(k)
\end{align*}$$
