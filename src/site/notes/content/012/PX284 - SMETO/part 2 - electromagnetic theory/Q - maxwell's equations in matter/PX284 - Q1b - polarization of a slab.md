---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/q-maxwell-s-equations-in-matter/px-284-q1b-polarization-of-a-slab/","noteIcon":"1","created":"2025-02-24T16:54:37.778+00:00","updated":"2025-02-24T17:11:16.538+00:00"}
---

- considering a dielectric medium between two parallel plate of opposite charges

![PX284 - Q1b - polarization of a slab.png|500](/img/user/pics/PX284%20-%20Q1b%20-%20polarization%20of%20a%20slab.png)

- applying gauss' law for a 'pill box' containing a small part of one of the sides:
$$|\vec E_{P}| \times 2A = \sigma_{P} \frac{A}{\varepsilon_{0}} = |\vec P| \frac{A}{\varepsilon_{0}}$$
- total polarization field inside the slab is the sum of those from the top and the bottom sides:
$$\vec E_{P} = - \frac{\vec P}{2\varepsilon_{0}} - \frac{\vec P}{2\varepsilon_{0}} = - \frac{\vec P}{\varepsilon_{0}}$$
- total field:
$$\begin{align*}
\vec E &= \vec E_{app} + \vec E_{P} \\
 &= \vec E_{app} - \frac{\vec{P}}{\varepsilon_{0}} \\
 &= \vec E_{app} - \chi \vec E  \\
\implies \vec E &= \frac{\vec{E}_{app}}{1+\chi} = \frac{\vec E_{app}}{\varepsilon_{r}}
\end{align*}$$
- reduction of $\vec E_{app}$ to $\vec E$ is called 'screening' 
- $\vec E_{P}$ is also called a 'depolarization field', but it means the same as polarization field
- for geometries other than a slab (cuboid), eg: an ellipsoid:
$$\vec E_{P} = - \alpha \frac{\vec P}{\varepsilon_{0}}$$

	where, $\alpha$ is called the depolarization factor
- for the slab, $\alpha = 1$

$$\begin{gather}
\vec P = \frac{\varepsilon_{0}\chi}{1+\alpha\chi} \vec E_{app} \\
\vec E = \frac{1}{1+\alpha\chi} \vec E_{app}
\end{gather}$$
- 
