---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/iv-circuits/px-157-b14c-circuits-rc-circuit/","noteIcon":"1","created":"2025-08-27T13:14:04.804+01:00","updated":"2024-11-26T20:09:04.000+00:00"}
---


![Pasted image 20240207180739.png](/img/user/pics/Pasted%20image%2020240207180739.png)
## charging a capacitor:
- at $t=0:$ 
	- capacitor is not charged
	- the circuit is closed:
$$\begin{align*}
		I_{0} = \frac{V_{ab}}{R} &= \frac{\epsilon}{R} \\\\
		Q_{0} &= 0 
	\end{align*}$$
- at $t=t':$
	- from [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/IV - circuits/PX157 - B14a - circuits - kirchhoff's rules#kirchhoff's loop rule\|kirchhoff's loop rule]]:
$$\begin{align*}
		\epsilon &= RI + \frac{Q}{C} \;, & I &= \frac{dQ}{dt}\\
		\epsilon &= R \frac{dQ}{dt}+ \frac{Q}{C}
\end{align*}$$
	- for $t\to\infty:$ the capacitor to be fully charged:
$$
\epsilon = V_{bc} = \frac{Q_{final}}{C} \implies Q_{final}= \epsilon C
$$
	- solving a [[content/011/PX153 - mathematics for physicists/term 1/PX153 - C - first order ODEs/C - first order ODEs\|first order ODE]] : try$Q(t) = \tilde Q (t) e^{- t/RC}:$ 
	$$\tilde Q(t) = \int_{0}^{t} \frac{\epsilon}{R} e^{- \frac{t'}{RC}}\,dt' = \epsilon C (e^\frac{t}{RC}-1)$$
	
$$
\implies Q(t) = \epsilon C (1-e^{- \frac{t}{RC}})
$$
	$$I(t) = \frac{dQ}{dt}= \frac{\epsilon}{R} e^{- \frac{t}{RC}}$$
![Pasted image 20240213093241.png](/img/user/pics/Pasted%20image%2020240213093241.png)
![Pasted image 20240213093331.png](/img/user/pics/Pasted%20image%2020240213093331.png)

- typical rate of charging is given by the *time constant*, or the *relaxation time* :
$$
\tau = R\,C
$$
## discharging a capacitor
- at $t=0:$
	- the battery is disconnected 
	- $I_{0}=0$, $Q_{0}=\epsilon C$
	- [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/IV - circuits/PX157 - B14b - circuits - maxwell loops\|loop rule]]:
$$\begin{align*}
			RI + \frac{Q}{C} &= 0 \\
			R \frac{dQ}{dt} + \frac{Q}{C} &= 0
		\end{align*}$$
	- solving the [[content/011/PX153 - mathematics for physicists/term 1/PX153 - C - first order ODEs/C - first order ODEs\|C - first order ODEs]] :
$$\begin{align*}
			Q(t) &= Q_{0}e^{-\frac{t}{RC}} \\
			&= \epsilon C e^{-\frac{t}{RC}}
		\end{align*}$$
	- current:
$$
I(t) = \frac{dQ}{dt} = - \frac{\epsilon C}{RC} e^{-\frac{t}{RC}} = -\frac{\epsilon}{R} e^{-\frac{t}{RC}}
$$
![Pasted image 20240213093148.png](/img/user/pics/Pasted%20image%2020240213093148.png)
![Pasted image 20240213093204.png](/img/user/pics/Pasted%20image%2020240213093204.png)
