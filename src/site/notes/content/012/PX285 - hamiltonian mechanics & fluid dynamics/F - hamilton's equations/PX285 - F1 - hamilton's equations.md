---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/f-hamilton-s-equations/px-285-f1-hamilton-s-equations/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T12:59:34.136+00:00"}
---

considering variations in the lagrangian: 
$$\begin{align*}
	dL (q_{i}, \dot q_{i}) &= \sum\limits_{i} \frac{\partial L}{\partial \dot q_{i}} d\dot q_{i} + \sum\limits_{i}\frac{\partial L}{\partial q_{i}} dq_{i} \\
	\therefore dL &= \sum\limits_{i} p_{i}\, d\dot q_{i} + \sum\limits_{i} \dot p_{i} \, dq_{i} \tag{1}
\end{align*}$$
	where, $p_{i} = \frac{\partial L}{\partial \dot q_{i}}$, and $\dot p_{i} = \frac{\partial L}{\partial q_{i}}$
- for $a = fg:$ 
$$\frac{da}{dt}= f \frac{dg}{dt}+ g \frac{df}{dt} \implies da = f\,dg + g\, df$$
- similarly, for equation $(1):$ 
$$\begin{align*}
	d\left(\sum_{i}p_{i}\dot q_{i}\right) = \sum\limits_{i}p_{i} \, d\dot q_{i} + \sum\limits_{i}\dot q_{i}\,dp_{i} \\
	\sum\limits_{i}p_{i} \, d\dot q_{i}  = d\left(\sum_{i}p_{i}\dot q_{i}\right) - \sum\limits_{i}\dot q_{i}\,dp_{i}
\end{align*}$$
- substituting into equation $(1)$ and rearranging: 
$$d\left(\sum\limits_{i}p_{i}\dot q_{i} - L \right) =  - \sum\limits_{i}\dot p_{i}\, dq_{i} + \sum\limits \dot q_{i}\,dp_{i} \tag{2}$$
- the argument of the differential on the $LHS$  of equation $(2)$ is defined to be the hamiltonian: 
$$H(p,q,t) = \sum\limits p_{i}\dot q_{i}- L$$
- therefore, equation $(2)$ can be re written as: 
$$dH =  - \sum\limits_{i}\dot p_{i}\, dq_{i} + \sum\limits \dot q_{i}\,dp_{i} \tag{3}$$
- also: 
$$dH = \sum\limits_{i} \frac{\partial H}{\partial q_{i}} dq_{i} + \sum\limits_{i}\frac{\partial H}{\partial p_{i}} dp_{i} \tag{4}$$
- comparing equations $(3)$ and $(4)$, the canonical hamilton's equations are obtained:  
$$\begin{gather}
	\dot q_{i}= \frac{\partial H}{\partial p_{i}} \\
	\dot p_{i}= - \frac{\partial H}{\partial q_{i}} 
\end{gather}$$
