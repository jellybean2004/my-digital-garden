---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g1-functions-of-a-single-variable/","noteIcon":"1","created":"2025-08-27T13:15:23.634+01:00","updated":"2025-01-07T19:31:39.000+00:00"}
---

## derivative
- for a function of one variable, the derivative is defined as:
$$\frac{df}{dx} = \frac{f(x+\Delta x) - f(x)}{\Delta x}$$
## ordinary differential equations (ODEs)
[[content/011/PX153 - mathematics for physicists/term 1/PX153 - C - first order ODEs/C - first order ODEs\|C - first order ODEs]]
[[content/011/PX153 - mathematics for physicists/term 1/PX153 - D - second order ODEs/D - second order ODEs\|D - second order ODEs]]
[[content/011/PX153 - mathematics for physicists/term 1/PX153 - D - second order ODEs/D - second order ODEs\|D - second order ODEs]]

- considering an ODE:
  $$\frac{df}{dx} = ax \implies f = ax^{2}+c$$
- $c$ is a constant of integration, and its value can be determined using an initial condition: $f(0) = c$
- a physics example: decay of a radioactive sample:
$$\frac{dN(t)}{dt} = - \lambda N(t)$$
	where, $N(t)$ is the number of undecayed nuclei at time, $t$
-  **note:** 
	- if $\cfrac{df}{dt} \propto a\, f(t) \implies f \propto e^{at}$
	- similarly, if $\cfrac{df}{dt} \propto -a\, f(t) \implies f \propto e^{-at}$ 

- therefore, the ODE can be solved giving:
$$N(t) = N_{0} e^{-\lambda t}$$
	where, $N_{0} = N(t=0)$

- now, considering a second-order ODE:
$$\frac{d^{2}f}{dx^{2}} \propto a^{2}f$$
- the solution will be exponential
- eg: if $f = e^{ax} + e^{-ax}:$
$$\begin{gather}
\frac{df}{dx} = ae^{ax} - ae^{-ax} \\
\frac{d^{2}f}{dx^{2}} = a^{2}e^{ax} + a^{2}e^{-ax} = a^{2}f
\end{gather}$$

- considering another second-order ODE:
$$\frac{d^{2}f}{dx^{2}} \propto -a^{2}f$$
- the solution will be a linear combination of $\cos$ and $\sin$
- eg: if $f = \cos ax + \sin ax$
$$\begin{gather}
\frac{df}{dx} = - a\sin ax + a \cos ax \\ 
\frac{d^{2}f}{dx^{2}} = - a^{2}\cos ax - a^{2} \sin ax  = -a^{2}f
\end{gather}$$
\1\n\2\n