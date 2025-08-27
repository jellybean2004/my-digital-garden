---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/t-geometric-optics/px-284-t2-fermat-s-principle/","noteIcon":"1","created":"2025-08-27T13:15:28.601+01:00","updated":"2025-05-03T14:23:34.000+01:00"}
---


![PX284 - T2 - fermat's principle.png|500](/img/user/pics/PX284%20-%20T2%20-%20fermat's%20principle.png)

- considering light travelling from point $A$ to $B$

>[!note] fermat's principle
the path taken by the light ray is that which extremizes the optical path

- more generally, light takes the path that minimizes the time, which neglects the other extrema

- for a given path, the phase change from $A$ to $B$ is:
$$\Delta\phi_{AB} = \int_{A}^{B} k\, dl = \int_{A}^{B} \frac{\omega}{v}\, dl = \int_{A}^{B} \frac{\omega}{c} n\,dl$$
	where, $k$ is the wave number, $\omega$ the angular frequency, $v = c/n$ the phase velocity, and $n$ the refractive index
- since $\omega$ and $c$ are constants:
$$\Delta \phi_{AB} = k_{0}\int_{A}^{B} n\,dl$$
	where, $k_{0} = \omega/c$
- the integral is called the '**optical path**':
$$\tau = \int_{A}^{B}n\,dl$$
- the time taken for light to travel is:
$$\Delta t =\int_{A}^{B} \frac{dl}{v} = \frac{1}{c}\int_{A}^{B}n\,dl$$
$$\therefore \Delta t = \frac{\tau}{c}$$
- by destructive interference:
$$\sum\limits_{\text{all paths}} \exp(i\Delta\phi_{AB}) \to 0$$
- except where $\Delta\phi_{AB}$ is extremized when small changes in the path do not change $\Delta\phi_{AB}$, and therefore, interfere constructively

## examples
- considering $n =$ constant $\implies \tau = n\int_{A}^{B}dl$, therefore, light takes a straight line path

![PX284 - T2 - fermat's principle-1.png|500](/img/user/pics/PX284%20-%20T2%20-%20fermat's%20principle-1.png)

- now considering media with $n_1$ and $n_2$
$$\begin{gather}
x_{2} = x - x_{1} \\
\tau = n_{1} (x_{1}^{2} + y_{1}^{2})^{1/2} + n_{2} ((x-x_{1})^{2} + y_{2}^{2})^{1/2}
\end{gather}$$
- extremizing with respect to $x:$
$$\frac{\partial \tau}{\partial x_{1}} = \frac{n_{1}x_{1}}{(x_{1}^{2}+y_{1}^{2})^{1/2}} + \frac{n_2(x-x_{1})}{((x-x_{1})^{2}+y_{2}^{2})^{1/2}}$$
- this leads to [[content/012/PX284 - SMETO/part 2 - electromagnetic theory/S - EM waves at boundaries/PX284 - S1 - snell's law\|snell's law]]:
$$n_{1}\sin i = n_{2}\sin t$$
