---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s2a-fresnel-relations/","noteIcon":"1","created":"2025-08-27T13:15:28.818+01:00","updated":"2025-03-14T06:27:14.000+00:00"}
---

- **fresnel conditions**:
$$\begin{gather}
\hat n \times (\vec E_{2} - \vec E_{1}) = 0 \\
\hat n \times (\vec H_{2} - \vec H_{1}) = 0 \\
(\vec j_{f} = 0 \text{ in dielectrics})
\end{gather}$$
- considering the two polarisation states of light:

![PX284 - S1 --2.png|500](/img/user/pics/PX284%20-%20S1%20--2.png)

- it is chosen to orient $\vec E$ such that $\vec E_i$, $\vec E_r$ and $\vec E_t$ point in the same direction where $i = r = t$, so for the first figure, $\vec E$ always points outwards, and for the second, it points to the right
- these are called the **s**- and the **p-components**, which stand for **sentrecht** and **parallel** (perpendicular and parallel in german)
- these refer to the orientation of the electric field with respect to the plane of the paper

- for the s-component, the electric field is continuous at the boundary
$$E_{i} + E_{r} = E_{t}$$
- defining $r_{s} =E_{r}/E_{i}$, and $t_{s} = E_{t}/E_i$
$$\implies 1 + r_{s} = t_{s}$$
- looking at the magnetic field:
$$H_{i} \cos i - H_{r}\cos r = H_{t} \cos t$$
- for dielectrics ($\mu_{r} \simeq 1)$, the impedance:
$$Z = \frac{E}{H} = \frac{Z_{0}}{n}$$
$$\begin{gather}
\implies\frac{E_{i}}{Z_{0}/n_1} \cos i - \frac{E_{r}}{Z_{0}/n_{1}}\cos r = \frac{E_{t}}{Z_{0}   /n_{2}}\cos t \\
n_{1}\cos i \,(E_{i} - E_{r}) = n_{2} \cos t \,E_{t} \\
n_{1}\cos i \, (1 - r_{s}) = n_{2} \cos t\, t_{s} = n_{2}\cos t \, (1+r_{s}) \\\\
\therefore r_{s} = \frac{n_{1}\cos i - n_{2}\cos t}{n_{1}\cos i + n_{2}\cos t} \\
t_{s} = \frac{Z n_{1}\cos i}{n_{1}\cos i + n_{2}\cos t}
\end{gather}$$

- similarly, for the p-component:
$$\begin{gather}
H_{i} - H_{r} = H_{t} \\
E_{i} \cos i + E_{r}\cos r = E_{t} \cos t \\
\end{gather}$$
- defining $r_{p}= E_{r}/E_{i}$ and $t_{p} = E_{t}/E_{i}$
$$\begin{gather}
\frac{E_{i}}{Z_{1}} - \frac{E_{r}}{Z_{1}} = \frac{E_{t}}{Z_{2}}\\
\implies n_{1}(1-r_{p}) = n_{2} t_{p} \\\\
(1 + r_{p}) \cos i = t_{p} \cos t \\\\
\therefore r_{p} = \frac{n_{1}\cos t - n_{2}\cos i}{n_{1}\cos t + n_{2}\cos i} \\
t_{p} = \frac{2n_{1}\cos i}{n_{1}\cos t + n_{2}\cos i} \\

\end{gather}$$
