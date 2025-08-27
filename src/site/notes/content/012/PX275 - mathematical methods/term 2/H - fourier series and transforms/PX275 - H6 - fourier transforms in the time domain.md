---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h6-fourier-transforms-in-the-time-domain/","noteIcon":"1","created":"2025-08-27T13:15:23.780+01:00","updated":"2025-02-06T18:20:46.000+00:00"}
---

- considering a time dependent function, $f(t)$
$$f(t) = \begin{cases}
0 & t<0 \\
e^{i\omega t}e^{-\gamma t} & t\geq 0
\end{cases}$$
- so, it has an oscillating term, and a damping term

![PX275 - H6 - fourier transforms in the time domain.png|500](/img/user/pics/PX275%20-%20H6%20-%20fourier%20transforms%20in%20the%20time%20domain.png)

- a useful function is the heavyside (step) function:
$$H(t) = \begin{cases}
1 & t \geq 0 \\
0 & t < 0
\end{cases}$$

![PX275 - H6 - fourier transforms in the time domain-1.png|500](/img/user/pics/PX275%20-%20H6%20-%20fourier%20transforms%20in%20the%20time%20domain-1.png)

- rewriting the amplitude as:
$$f(t) = H(t) e^{i\omega_{0}t}e^{-\gamma t}$$
- so, the total power:
$$I_{tot} = \int_{-\infty}^{\infty} |f(t)|^{2} \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty}|\tilde f(\omega)|^{2}\,d\omega$$
- this is [[content/012/PX275 - mathematical methods/term 2/H - fourier series and transforms/PX275 - H5 - parseval's theorem\|parseval's theorem]] in time domain: $f(t) \to \tilde f(\omega)$ instead of  $f(x) \to \tilde f(k)$

- similarly, the fourier transform is:
$$\tilde f(\omega) = \int_{-\infty}^ {\infty} e^{-i\omega t} f(t)\,dt$$
- so, $x$ [length] $\to k$ [length]$^{-1}$, and $t$ [time] $\to \omega$ [time]$^{-1}$, which is the frequency

- for the given case:
$$\begin{align*}
\tilde f(\omega) &= \int_{-\infty}^{\infty} e^{-i\omega t} H(t)e^{i\omega_{0}t} e^{-\gamma t}\,dt \\
&= \int_{0}^{\infty} e^{i(\omega_{0}-\omega) t -\gamma t} \,dt \\
&= \left[ \frac{e^{i(\omega_{0}-\omega)t - \gamma t}}{i(\omega_{0}-\omega) - \gamma} \right]_{0}^{\infty} \\
&= \frac{-1}{i(\omega_{0}-\omega) - \gamma}
\end{align*}$$

- now, for $|\tilde f(\omega|^{2} = \tilde f(\omega) \tilde f^{*}(\omega)$

$$\begin{align*}
\tilde f(\omega) &= \frac{-1}{i(\omega_{0}-\omega) - \gamma} \left[\frac{-\gamma-i(\omega_{0}-\omega)}{-\gamma-i(\omega_{0}-\omega)}\right] \\
&= \frac{\gamma+i(\omega_{0}-\omega)}{\gamma^{2}+(\omega_{0}-\omega)^{2}} \\\\
\implies \tilde f^{*}(\omega) &= \frac{\gamma-i(\omega_{0}-\omega)}{\gamma^{2}+(\omega_{0}-\omega)^{2}} \\\\
\therefore |f(\omega)|^{2} &= \frac{\gamma^{2} + (\omega_{0}- \omega)^{2}}{[\gamma^{2} + (\omega_{0}- \omega)^{2}]^{2}}\\
&= \frac{1}{\gamma^{2} + (\omega_{0}- \omega)^{2}}\\\\
I_{total} &= \frac{1}{2\pi} \int_{-\infty}^{\infty} \frac{1}{\gamma^{2}+(\omega_{0}-\omega)^{2}} \, d\omega
\end{align*}$$
