---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/u-wave-optics/px-284-u3-fabry-perot-interferometry/","noteIcon":"1","created":"2025-05-15T14:05:54.807+01:00","updated":"2025-05-15T14:17:15.047+01:00"}
---


![PX284 - U3 - fabry-perot interferometry-2.png|500](/img/user/pics/PX284%20-%20U3%20-%20fabry-perot%20interferometry-2.png)

- phase difference: $2\phi = 2dk_{2}\cos t$
-  transmitted wave:
$$t_{total} = tt' ( 1 + r^{2}e^{i2\phi} + (r^{2}e^{i2\phi})^{2} + \dots)$$
- this is a geometric progression:
$$t_{total} = \frac{tt'}{1-r^{2}e^{i2\phi}}$$
- transmitted power: $T = |t_{total}|^{2}$
- assuming $tt'$ and $r$ are real:
$$\begin{align*}
T &= \frac{t^{2}t'^{2}}{(1-r^{2}e^{i2\phi})(1-r^{2}e^{-i2\phi})} \\
&= \frac{t^{2}t'^{2}}{1+r^{4}-2r^{2}\cos2\phi} \\
&= \frac{t^{2}t'^{2}}{(1-r^{2})^{2} 2r^{2}(1-2\sin^{2}\phi)} \\
&= \frac{t^{2}t'^{2}/(1-r^{2})^2}{1+F\sin^{2}\phi}
\end{align*}$$
	where, $F = 2r^{2}/(1-r^2)^2$ is called "**finesse**"

- if no losses:
$$t^{2} = t'^{2} = (1-r^{2}) = 1-R \implies T = \frac{1}{1+F\sin^{2}\phi}$$
![PX284 - U3 - fabry-perot interferometry-3.png|500](/img/user/pics/PX284%20-%20U3%20-%20fabry-perot%20interferometry-3.png)

$$F = \frac{4r^{2}}{(1-r^{2})^{2}} = \frac{4R}{(1-R)^{2}}$$
$$\begin{gather}
R = 0.5 \implies F = 8 \\
R = 0.9 \implies F = 360
\end{gather}$$

- fabry-perot interferometer acts as a narrow band filter
- the value of $\phi =-= k_{2}d\cos t$ can be tuned to pass specific wavelengths, $\frac{2\pi}{\lambda_{0}} n_{2}d\cos t$
