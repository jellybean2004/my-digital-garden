---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e2-two-level-system-revisited/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-23T22:43:28.438+00:00"}
---

- the energy levels are: 
$$\begin{align*}
&\_\_\_\_\_\_\_\_\_\_\;& +\frac{\Delta}{2}  \\ 
\uparrow E \hspace{2em}  &\bigg\updownarrow \Delta \\
&\_\_\_\_\_\_\_\_\_\_\;&- \frac{\Delta}{2}
\end{align*}$$
- the partition function: 
$$\begin{align*}
	Z &= \sum\limits_{i} \exp(-\beta E_{i}) \\
	&= \exp\left(\beta \frac{\Delta}{2}\right)+ \exp\left(-\beta \frac{\Delta}{2}\right) \\
	&= 2\cosh\left(\beta \frac{\Delta}{2}\right) \\\\ 
	\implies \ln Z &= \ln\left[2\cosh\left(\beta \frac{\Delta}{2}\right)\right]
\end{align*}$$
- the internal energy: 
$$U = - \frac{d\ln{Z}}{d\beta} = - \frac{\Delta}{2} \frac{2\sinh\left(\beta \frac{\Delta}{2}\right)}{2\cosh \left(\beta \frac{\Delta}{2}\right)} = - \frac{\Delta}{2} \tanh\left(\beta \frac{\Delta}{2}\right)$$

![tanh function.png|500](/img/user/pics/tanh%20function.png)
*image: wolfram*

- at very low temperatures, $\left(\beta \frac{\Delta}{2}\right)$ is very large $\implies U \to - \frac{\Delta}{2}$
- at very high temperatures, $\left(\beta \frac{\Delta}{2}\right)$ is very small $\implies U \to 0$

- also, the helmholtz free energy:
$$F = - k_{B}T \ln Z = - k_{B}T \ln \left(2\cosh\left(\beta \frac{\Delta}{2}\right)\right)$$
- the entropy: 
$$S = \frac{U-F}{T} = - \frac{\Delta}{2T} \tanh\left(\beta \frac{\Delta}{2}\right) + k_{B}T\ln\left[2\cosh\left(\beta \frac{\Delta}{2}\right)\right]$$
- so, at very low temperatures, $\left(\beta \frac{\Delta}{2}\right)$ is large: 
$$\ln\left(2\cosh\left(\beta \frac{\Delta}{2}\right)\right) = \ln\bigg[\exp\left(\beta \frac{\Delta}{2}\right) + \underbrace{\exp\left(-\beta \frac{\Delta}{2}\right)}_{tiny} \bigg] \to \left(\beta \frac{\Delta}{2}\right)$$
$$\therefore S = -\frac{\Delta}{2T} + k_{B} \beta \frac{\Delta}{2} = 0$$
- at very high temperatures, $\left(\beta \frac{\Delta}{2}\right)$ is very small: $S \to k_{B} \ln 2$
- this agrees with the third law of thermodynamics, ie: entropy of an isolated system approaches a constant value at thermal equilibrium

- finally, 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V} = k_{B}\left(\beta \frac{\Delta}{2}\right)^{2} \text{sech}^{2}\left(\beta \frac{\Delta}{2}\right)$$
- this has a peak at approximately $\frac{k_{B}T}{\Delta} \sim 0.42$
- this peak is called the **schottky anomaly**

![Pasted image 20241122105447.png](/img/user/pics/Pasted%20image%2020241122105447.png)
