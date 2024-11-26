---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/iv-circuits/px-157-b14a-circuits-kirchhoff-s-rules/","created":"2024-10-01T18:27:10.139+01:00","updated":"2024-11-26T20:09:00.160+00:00"}
---

## kirchhoff's junction rule
- current into element = current out of element:
$$
I_{in}= I_{out}
$$
- no charge accumulation
![Pasted image 20240207180441.png](/img/user/pics/Pasted%20image%2020240207180441.png)
$$\begin{align*}
	I_{1} &= \iint_{A_{1}} \vec J \cdot d\vec S \\
	I_{2} &= \iint_{A_{2}} \vec J \cdot d\vec S \\\\
	Q &= \iiint_{Vol.} \rho\,d\tau
\end{align*}$$
$$
0 = \frac{dQ}{dt} = \frac{d}{dt}\iiint_{Vol.} \rho\,d\tau = \iint_{A_{1}} \vec J \cdot d\vec S - \iint_{A_{2}} \vec J \cdot d\vec S = I_{1}-I_{2}
$$
	where, $\frac{dQ}{dt}$ is the rate of change of total charge in volume, not rate of charges passing a surface in unit time
- taking a limit of decreasing the distance between $A_{1}$ and $A_{2}:$
$$\begin{align*}
		\frac{dQ}{dt} &= I_{tot} = 0 \\\\
		I_{tot} = \sum\limits_{i} I_{i} &= \sum\limits_{i,in}I_{i} + \sum\limits_{i,out}I_{i} = 0
	\end{align*}$$
- conventionally, currents toward a circuit are positive, and away are negative
## kirchhoff's loop rule
- in a DC circuit, the potential difference of a closed path is zero
- from *[[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/II - potentials/PX157 - B8a - calculating potentials#^7d6a9f\|here]]* :
$$\begin{align*}
		V_{a}-V_{b} &= \int_{a}^{b}\vec E \cdot d\vec l \\
		\oint \vec E\cdot d\vec l = \int_{a}^{a}\vec E\cdot d\vec l &= V_a-V_{a} =0
	\end{align*}$$
- over a circuit loop, the sum of the potentials from sources balances against potential drops across all other components:
$$
\sum\limits_{i}\epsilon_{i} = \sum\limits_{j}V_{j}
$$

- eg: ![Pasted image 20240207181114.png](/img/user/pics/Pasted%20image%2020240207181114.png)
	- junction rule:
		- at junction $a:$
$$
I_{1}=I_{2}+I_{3}
$$
		- at junction $b:$
$$
I_{2}+I_{3}=I_{4}=I_{1}
$$
	- loop rule:
		- for loop $1:$
$$
\epsilon_{1} = R_{1}I_{4} + R_{2}I_{2}
$$
		- for loop $2:$
$$
\epsilon_{2}-\epsilon_{3}= -R_{2}I_{2}+R_{3}I_{3}
$$
