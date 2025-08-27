---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/t-geometric-optics/px-284-t3b-spherical-surface-using-intersecting-cords-theorem/","noteIcon":"1","created":"2025-08-27T13:15:28.610+01:00","updated":"2025-05-03T12:18:39.000+01:00"}
---


![PX284 - T3 - imaging-1.png|500](/img/user/pics/PX284%20-%20T3%20-%20imaging-1.png)

- considering a spherical surface using '*real is positive*' convention ($u$ and $v>0$)
- the optical path length $APB:$
$$\tau = n_{1}((u+x)^{2} + y^{2})^{1/2} + n_{2} ((v-x)^{2} + y^{2})^{1/2}$$

>[!note] intersecting cord theorem
>when any two cords on a circle cross, the products of the length of the two pieces of each cord are equal

$$\begin{gather}
y^{2} = (2R - x)x \implies x^{2}+y^{2} = 2Rx \\
\implies \tau(x) = n_1\sqrt{u^{2} + 2(R+u)x} + n_{2}\sqrt{v^{2} + (R-v)x}
\end{gather}$$
- from fermat's principle:
$$\frac{d\tau}{dx} = 0 = \frac{n_{1}(R+u)}{\sqrt{u^{2} + 2(R+u)x}} + \frac{n_{2}(R-u)}{\sqrt{v^{2} + (R-v)x}}$$
- limiting to '**paraxial rays**', where the rays lie at small angles to the axis, so ${} x$ is small, AKA **gaussian optics**:
$$\frac{n_{1}(R+u)}{u} + \frac{n_{2}(R-u)}{v} = 0$$
$$\therefore \frac{n_{1}}{u}+ \frac{n_{2}}{v} = \frac{n_{2}-n_{1}}{R}$$

- if the spherical surface curved the other way, $x \to -x:$
$$\therefore \frac{n_{1}}{u}+ \frac{n_{2}}{v} =  - \frac{n_{2}-n_{1}}{R}$$
- this is equivalent to setting $1/R\to-1/R$, referred to as **'negative radius of curvature'**
