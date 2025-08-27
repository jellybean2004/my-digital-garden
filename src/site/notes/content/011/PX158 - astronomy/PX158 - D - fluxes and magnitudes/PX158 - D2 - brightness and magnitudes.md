---
{"dg-publish":true,"permalink":"/content/011/px-158-astronomy/px-158-d-fluxes-and-magnitudes/px-158-d2-brightness-and-magnitudes/","noteIcon":"1","created":"2025-08-27T13:14:04.986+01:00","updated":"2024-11-26T23:13:34.000+00:00"}
---

## apparent magnitude (m)
- circa $150 \, BCE$, hipparchus of nicaea catalogued the night sky using a system in which the brightest stars is a *magnitude $1$*, and the faintest stars is a *magnitude $6$*
- in the $1850s$, norman robert pogson worked out that the eye is a logarithmic detector, and that $\Delta magnitude$ is $\times 100$ in flux
- consider two stars, star 1 and star 2, with fluxes, $f_{1}$ and $f_{2}$, and magnitudes, $m_{1}$ and $m_{2}$
$$\begin{align*}
	\frac{f_{2}}{f_{1}} &= \left(\frac{1}{100}\right)^{\frac{m_{2}-m_{1}}{5}} \\
	\; \log_{10} \left(\frac{f_{2}}{f_{1}}\right) &= -\frac{2}{5}(m_{2}-m_{1}) \\
	\therefore (m_{2}-m_{1}) &= -2.5 \log_{10}\left(\frac{f_{2}}{f_{1}}\right)
\end{align*}$$
- pogson selected vega as a reference star due to its brightness: 
$$m_{vega} = 0$$
- magnitudes of other stars can be determined by: 
$$\therefore m = -2.5\log_{10}\left(\frac{f}{f_{vega}}\right)$$
- these are *apparent magnitudes* - depends upon where the observer is
## absolute magnitude (M)
- the apparent magnitude if the object was located at a distance of $10\,pc$
$$\begin{align*}
	M-m &= -2.5 \log_{10}\left(\frac{\frac{L}{4\pi (10\,pc)^{2}}}{\frac{L}{4\pi d^{2}}}\right) \\
	&= -2.5 \log_{10}\left(\frac{d}{10\,pc}\right)^{2} \\
	\therefore m-M &= 5 \log_{10}\left(\frac{d}{10\,pc} \right)
\end{align*}$$
- eg: how far away could the sun be seen with a naked eye?
		$m=6$
		$M_{\odot} = +4.8$
$$\therefore d \approx 1.4\,pc $$
- eg: what is the absolute magnitude of a $100\,W$ light bulb and how far away can it be seen with a naked eye?
	- $L_{\odot} = 3.82 \times10^{26}\,W$, $M_{\odot} = +4.8$
$$\begin{align*}
	M_{b}-M_{\odot} &= -2.5 \log_{10}\left(\frac{f_{b}}{f_{\odot}}\right) \\
	M_{b} &= +4.8 -2.5 \log_{10}\left(\frac{L_{b}}{L_{\odot}}\right) \\
	&= +4.8 -2.5 \log_{10}\left(\frac{100}{3.82\times10^{26}}\right) \\
	\therefore M_{b} &\approx +66
\end{align*}$$
	- for bulb to be seen by a naked eye in a dark sky, $m = 6$
$$\begin{align*}
	m-M &= 5\log_{10} \left(\frac{d}{10\,pc}\right) \\
	\frac{6-66}{5} &= \log_{10}\left(\frac{d}{10\,pc}\right) \\
	10^{-12} &= \frac{d}{10\,pc} \\
	\therefore d &= 10^{-11}\times 3.09\times10^{16}\,m \\
	&\approx 300km
\end{align*}$$

