---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/iii-properties/px-157-b13b-resistance/","noteIcon":"1","created":"2024-10-01T18:27:10.131+01:00","updated":"2024-11-26T20:08:53.382+00:00"}
---

## resistivity
- ohm's law:
$$
\vec E = \rho\,\vec J
$$
	where, $\rho=$ electrical resistivity
{ #9e9b04}

- units: $V\,m\,A^{-1}$ or $\ohm\,m$
- expect: $\rho \propto |\vec v_{e^{-}}-\vec v_{ion}| <\nu_{ei}>$, where $\nu_{ei}=$ collision frequency

- *electrical conductivity*: $\sigma = \frac{1}{\rho}$
	- units: $\ohm^{-1}\,m^{-1}$
![Pasted image 20240207102205.png](/img/user/pics/Pasted%20image%2020240207102205.png)
$$\begin{align*}
	\frac{V}{L} &= \rho \frac{I}{A}\\
	\therefore V &= \frac{\rho L}{A}I = RI
\end{align*}$$
	where, $R=$ resistance
![Pasted image 20240207102224.png](/img/user/pics/Pasted%20image%2020240207102224.png)
### resistors in series
![Pasted image 20240207102242.png](/img/user/pics/Pasted%20image%2020240207102242.png)
- same current, $I$, flowing though both the resistors
- potential drops across $R_{1}$ and $R_{2}$ are $V_{1}$ and $V_{2}$ respectively:
$$\begin{align*}
	V_{1} &= R_{1}I \\
	V_{2} &= R_{2}I \\\\
	V &= V_{1}+V_{2} \\
	\therefore V &= (R_{1}+R_{2}) I
\end{align*}$$
- the equivalent resistance is: $R_{eq} = R_{1}+ R_{2}$
- if both resistors have the same $\rho$ and $A:$
$$
R_{eq}= \frac{\rho}{A}(L_{1}+L_{2})
$$
### resistors in parallel

![Pasted image 20240207102309.png](/img/user/pics/Pasted%20image%2020240207102309.png)
- same potential drop, $V$, across both the resistors:
$$\begin{align*}
		I_{1}&= \frac{V}{R_{1}}\\
		I_{2}&= \frac{V}{R_{2}}
	\end{align*}$$
- total current:
$$
I = I_{1}+I_{2} = V\left(\frac{1}{R_{1}} +\frac{1}{R_{2}}\right)
$$
- the equivalent resistance is: $\frac{1}{R_{eq}} = \frac{1}{R_{1}} + \frac{1}{R_{2}}$
- if both resistors have the same $\rho$ and $L:$
$$
\frac{1}{R_{eq}}= \frac{1}{\rho L} (A_{1}+A_{2})
$$
- if both resistors are the same:
	- in series: $R_{eq}= 2R \implies I = \frac{V}{2R}$
	- in parallel:
$$
\frac{1}{R_{eq}}= \frac{2}{R}\implies \frac{2V}{R}
$$
