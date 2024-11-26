---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-e-ac-circuits/px-157-e2-complex-impedences/","created":"2024-10-01T18:27:10.275+01:00","updated":"2024-11-26T20:11:16.582+00:00"}
---

- for DC, using [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/III - properties/PX157 - B13b - resistance#^9e9b04\|ohm's law]]: $V=RI$
- for AC, generalizing [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/III - properties/PX157 - B13b - resistance#^9e9b04\|ohm's law]]:
$$
\tilde V = \tilde Z \tilde I
$$
- $\tilde Z =$ *complex impedance* (units: $\Omega$)
- $\tilde Y = \frac{1}{\tilde Z} =$ *complex admittance* (units: siemens ($S$))
### resistors
![Pasted image 20240311182237.png](/img/user/pics/Pasted%20image%2020240311182237.png)
- source:
$$
V(t) = V_{0}\cos(\omega t)
$$
- current:
$$
I(t) = \frac{V(t)}{R} = \frac{V_{0}}{R}\cos(\omega t) = I_{0}\cos(\omega t)
$$
- for the resistor:
$$
\tilde Z_{R}=R
$$
### capacitors
![Pasted image 20240311182247.png](/img/user/pics/Pasted%20image%2020240311182247.png)
- charge on capacitor: $Q=CV$
- current: $I= \frac{dQ}{dt} = C \frac{dV}{dt}$
- if $V(t) = V_{0}\cos(\omega t):$
$$
I(t) = -C\,V_{0}\,\omega\sin(\omega t)
$$
- $V(t)$ and $I(t)$ are *out of phase*

- **complex notation**:
$$\begin{align*}
		\tilde V &= V_{0}e^{j\omega t} \\
		\tilde I &= j\,\omega\,C\,\tilde V \\
		\tilde Z_{C} &= \frac{1}{j\omega C}
	\end{align*}$$
$$
\tilde I = \omega C V_{0}e^{j\omega t} e^{j \frac{\pi}{2}}
$$
- $\tilde I$ leads to $\tilde V$ by $\frac{\pi}{2}:$
$$
I(t) = \omega CV_{0}\cos(\omega t + \frac{\pi}{2})
$$
![Pasted image 20240311182301.png](/img/user/pics/Pasted%20image%2020240311182301.png)
### inductors
![Pasted image 20240311182318.png](/img/user/pics/Pasted%20image%2020240311182318.png)
- voltage across the inductor:
$$
V= L \frac{dI}{dt}
$$
- if $V(t) = V_{0}\cos(\omega t):$
$$
I(t) = \frac{V_{0}}{\omega L}\sin(\omega t)
$$
- $V(t)$ and $I(t)$ are *out of phase*

- **complex notation**:
$$\begin{align*}
		\tilde I &= I_{0}e^{j\omega t} \\\\
		\tilde V &= L \frac{d\tilde{I}}{dt} \\
		&= j\omega L \tilde I
	\end{align*}$$
- comparing with $\tilde V = \tilde Z \tilde I:$
$$
\tilde Z_{L} = j\omega L
$$
- since $I = \frac{1}{j\omega L} \tilde V:$
$$
I = \frac{-j}{\omega L}\tilde V = \frac{1}{\omega L} \tilde V e^{-j \frac{\pi}{2}}
$$
- the current lags behind the voltage by $\frac{\pi}{2}$
![Pasted image 20240311182332.png](/img/user/pics/Pasted%20image%2020240311182332.png)

- **imp note**: distinguish '$L$' from '$C$' in writing