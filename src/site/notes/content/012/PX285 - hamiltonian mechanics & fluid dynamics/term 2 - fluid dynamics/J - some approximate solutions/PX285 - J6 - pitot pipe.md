---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/j-some-approximate-solutions/px-285-j6-pitot-pipe/","noteIcon":"1","created":"2025-01-31T12:31:25.825+00:00","updated":"2025-02-01T15:45:15.821+00:00"}
---

![PX285 - J6 - pitot pipe.png|500](/img/user/pics/PX285%20-%20J6%20-%20pitot%20pipe.png)

- applying bernoulli's principle for the stream line:
$$\begin{gather}
P_{f} + \rho_{f} \frac{u_{f}^{2}}{2} + \rho_{f} g z_{0} = P_{0} + \rho_{f} g z_{0} \\
P_{0} - P_{f} = \rho_{f} \frac{u_{f}^{2}}{2} \\
\therefore u_{f} = \sqrt{\frac{2(P_{0}- P_{f})}{\rho_{f}}} \tag{1}
\end{gather}$$

![PX285 - J6 - pitot pipe-1.png|500](/img/user/pics/PX285%20-%20J6%20-%20pitot%20pipe-1.png)

- applying bernoulli's principle in the tube:
$$\begin{gather}
P_{A} = P_{f} + \rho_{f} g z' + \rho_{m}g \Delta z \\
P_{B}= P_{0} + \rho_{f}g (z' + \Delta z)
\end{gather}$$
- if $P_{A}= P_{B}$, there is no flow, $\vec u = 0$
$$\begin{align*}
P_{0} - P_{f} &= \rho_{f} g z' + \rho_{m}g \Delta z - \rho_{f} g z' + \rho_{f} g \Delta z \\
&= g \Delta z (\rho_{m} - \rho_{f})
\end{align*}$$
- substituting into equation $(1):$
$$\therefore u_{f} = \sqrt{2g\Delta z \left(\frac{\rho_{m}}{\rho_{f}}-1\right)} \approx \sqrt{2g\Delta z \left(\frac{\rho_{m}}{\rho_{f}}\right)}$$
	where, the approximation is for $\rho_{m}\gg \rho_{f}$
