---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/a-introduction/px-282-a6-magnitudes-bandpasses-colours/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:33:22.979+00:00"}
---

- see: [[content/011/PX158 - astronomy/PX158 - D - fluxes and magnitudes/PX158 - D2 - brightness and magnitudes\|PX158 - D2 - brightness and magnitudes]]
## magnitude
- astronomy uses magnitude to measure the brightness
- it is on a logarithmic scale
- originally, it was designed to mimic human eye response
## apparent magnitude
- it is the magnitude as seen from a distance, $d$
- for two stars with apparent magnitudes, $m_{1}$ and $m_{2}$, and fluxes, $f_{1}$ and $f_{2}:$ 
$$m_{1}- m_{2} = -2.5 \log\left(\frac{f_{1}}{f_{2}}\right) \tag{1}$$
- the scale needs a zero-point, which is taken to be vega, $m_{vega}=0 \,\forall\,\lambda$ 
- therefore, the apparent magnitude for any star is: 
$$m_{*} = -2.5\log\left(\frac{f_{*}}{f_{vega}}\right)$$
- this scale makes numbers easy to work with, eg: 
	- sirius, $m = -1.4$
	- sun, $m_\odot=-2.7$
	- proxima cententari, $m=11$

- **note:** larger the apparent magnitude, the fainter a fainter star
- $\sim5\,magnitudess \approx 100\times brightness$

- flux and magnitude are so far **bolometric***, ie. measured across all wavelengths, or formally: 
$$f = \int_{0}^{\infty} f_{\lambda}\,d\lambda$$
	where, $f_\lambda$ is the flux density $[Js^{-1}m^{-2}nm^{-1}]$

- in practice,  all wavelengths cannot be measured
- $\lambda-$ranges are selected using filters
- a filter has a transmission function, $T_A:$ 
$$\bar f_{A} = \frac{\int_{0}^{\infty} T_{\lambda}f_{\lambda}\,d\lambda}{\int_{0}^{\infty} T_{\lambda}\,d\lambda}$$
- eg:
	- $90\%$ at $\lambda$

### colours and temperature
![Pasted image 20241008101726.png](/img/user/pics/Pasted%20image%2020241008101726.png)

- $m$  in a bandpass: ${} m_{B},m_{U},m_{V}$
	- $U-B \text{ colour}= m_{U}-m_{B}$
	- $B-V \text{ colour}= m_B-m_V$
- $B$ has shorter $\lambda$ than $V$, so a star with a $B-V<0$, has $m_{B}<m_{V}$, is 'bluer' than vega ($m_{vega}=0$ in all bands)

- colour is a strong function of temperature
## absolute magnitude
- it says how bright would a star would be if it were at a distance of $10\,pc$, ie: the magnitude of a star at a distance of $10\,pc$
- therefore, $M=m(\text{at 10\,pc})$
- flux has an inverse square relation with the distance, ie: $\frac{f(10\,pc)}{f_{d}} = \left(\frac{d}{10\,pc}\right)^{2}$
- using equation $(1):$ 
$$\begin{align*}
	M-m &= -2.5\log\left(\frac{f(10\,pc)}{f_{d}}\right) \\
	&= -2.5\log\left(\frac{d}{10\,pc}\right)^{2} \\
	\therefore M-m &= -5\log\left(\frac{d}{10\,pc}\right)
\end{align*}$$
- if $L \uparrow$ then $M\downarrow$ (brighter)