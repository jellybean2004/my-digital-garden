---
dg-publish: true
---
![Pasted image 20240311183857.png](/img/user/pics/Pasted%20image%2020240311183857.png)
- **step 1:**
$$
\tilde Z_{eq} = R +j\omega L + \frac{1}{j\omega C}
$$
- **step 2:**
$$
\tilde I = \frac{\tilde V_{in}}{\tilde Z_{eq}} = \frac{\tilde V_{in}}{R +j\left(\omega L - \frac{1}{\omega C}\right)}
$$
- **step 3:**
$$\begin{align*}
	\tilde V_{out} &= (\tilde Z_{L}+\tilde Z_{C})\tilde I \\
	&= \left(j\omega L + \frac{1}{j\omega C}\right)\tilde I \\
	&= \frac{j\left(\omega L + \frac{1}{j\omega C}\right)}{R+j\left(\omega L - \frac{1}{\omega C}\right)} \tilde V_{in}
\end{align*}$$
- **step 4:**
$$
\frac{|\tilde V_{out}|}{|\tilde V_{in}|} = \frac{\left|\omega^{2}LC - 1\right|}{\sqrt{\omega^{2}R^{2}C^{2}+(\omega^{2}LC-1)^{2}}}
$$
- **step 5:**
$$
\phi = \arctan\left(\frac{\omega L - \frac{1}{\omega C}}{R}\right)
$$
- $\tilde V_{in}$ leads $\tilde I$ by a phase, $\phi$
![Pasted image 20240311185106.png](/img/user/pics/Pasted%20image%2020240311185106.png)
- this circuit acts as a *notch filter*
![Pasted image 20240311185143.png](/img/user/pics/Pasted%20image%2020240311185143.png)
- since $\tilde V_{in}= \tilde V_{out}+ \tilde V_{R}$, the voltage drop over the resistor makes a *bandpass filter*
