---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/b-introduction/px-284-b2-microstates-and-macrostates/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-23T20:35:29.640+00:00"}
---

## microstate
- any microscopic configuration of the system
- eg: specify the position, and the velocity for every molecule in $1\,l$ of gas
- this is very difficult/impossible to measure
## macrostate
- any configuration with particular measurable properties
- eg: specify internal energy ${} (U)$, pressure $(p)$, and volume $(V)$ for $1\,l$ of gas
- each macrostate can correspond to many microstates
## example
- 3 simple harmonic oscillators (SHOs) with $E=2\hbar\omega$ can be arranged in six ways, ignoring the zero point energy
$$\begin{gather*}
	\begin{matrix}
	    \boxed2  & \boxed0 & \boxed0
	\end{matrix} & E^{(1)} = 2\hbar \omega \\\\
	
    \begin{matrix}
        \boxed1 & \boxed1 & \boxed0 \\ 
        \boxed1 & \boxed0 & \boxed1 \\ 
    \end{matrix} &  E^{(2)} = \hbar \omega \\\\
    
    \begin{matrix}
        \boxed0 & \boxed1 & \boxed1 \\
        \boxed0 & \boxed0 & \boxed2 \\ 
        \boxed0 & \boxed2 & \boxed0
    \end{matrix} & E^{(3)} = 0 \hbar \omega
\end{gather*}$$
- here, the total number of microstates: ${} \Omega=6 {}$
- if a measurement is done sensitive to:
	- $E:$ there is $1$ macrostate
	- $E^{(1)}$ (the energy of SHO 1): there are 3 macrostates: $E^{(1)} = (2\;or\;1\;or\;0)\hbar \omega$ with 1, 2, and 3 microstates respectively
