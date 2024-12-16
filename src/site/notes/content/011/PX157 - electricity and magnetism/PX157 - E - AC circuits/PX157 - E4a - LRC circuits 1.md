---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-e-ac-circuits/px-157-e4a-lrc-circuits-1/","noteIcon":"1","created":"2024-10-01T18:27:10.281+01:00","updated":"2024-11-26T20:11:20.174+00:00"}
---

![Pasted image 20240311182507.png](/img/user/pics/Pasted%20image%2020240311182507.png)
- **step 1:**
$$
\tilde Z_{eq}= \tilde Z_{R}+ \tilde Z_{C} = R + \frac{1}{j\omega C}
$$
- **step 2:**
$$
\tilde V_{in} = \tilde Z_{eq}\tilde I \implies \tilde I = \frac{\tilde V_{in}}{R+ \frac{1}{j\omega C}}
$$
- **step 3:**
$$
\tilde V_{out}= \tilde Z_{C}\tilde I = \frac{1}{j\omega C}\frac{\tilde V_{in}}{R+ \frac{1}{j\omega C}} = \frac{\tilde V_{in}}{j\omega RC +1}
$$
- **step 4:**
$$
|\tilde V_{out}| = \frac{|\tilde V_{in}|}{\sqrt{\omega^{2}R^{2}C^{2}+1}} \implies \frac{|\tilde V_{out}|}{1} = \frac{|\tilde V_{in}|}{\sqrt{\omega^{2}R^{2}C^{2}+1}}
$$
- circuit acts as a *low-pass filter*
- typical relaxation time: $\tau = RC$
![Pasted image 20240311182707.png](/img/user/pics/Pasted%20image%2020240311182707.png)

- **step 5:**
$$\begin{align*}
		\tilde Z_{eq} &= Z_{0}e^{j\phi}  \\
		\phi &= \arctan\left(\frac{\mathbb{I}m \tilde Z_{eq}}{\mathbb{Re}\tilde Z_{eq}}\right) \\
		&= \arctan\left(- \frac{1}{\omega RC}\right)
	\end{align*}$$
- $\tilde V_{in}=\tilde Z_{eq}\tilde I = Z_{0}e^{i\phi}\tilde I$ $\tilde V$ leads $\tilde I$ by a phase, $\phi$ 
- since $\phi<0$, $\tilde V_{in}$ lags behind $\tilde I$
