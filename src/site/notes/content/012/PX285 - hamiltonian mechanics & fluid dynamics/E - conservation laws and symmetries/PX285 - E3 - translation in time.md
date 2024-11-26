---
dg-publish: true
---

- taking a small translation in time, $t \to t + \delta t$
- so, the lagrangian: $L \to L + \delta L$, with $\delta L = 0$ due to the time invariance of lagrangian
- consider a general lagrangian: $L(q_{i},\dot q_{i})$, where $i = 1,\dots d$
- the total time derivative of $L$ is: 
$$\frac{dL}{dt} = \sum\limits_{i} \left(\frac{\partial L}{\partial q_{i}} \frac{\partial q_{i}}{\partial t} + \frac{\partial L}{\partial \dot q_{i}} \frac{\partial \dot q_{i}}{\partial t} \right) + \frac{\partial L}{\partial t} = \sum\limits_{i} \left(\frac{\partial L}{\partial q_{i}} \frac{\partial q_{i}}{\partial t} + \frac{\partial L}{\partial \dot q_{i}} \frac{\partial \dot q_{i}}{\partial t} \right)$$
$$\frac{\partial L}{\partial q_{i}} = \frac{d}{dt} \frac{\partial L}{\partial \dot q_{i}} \;\forall i \in[1,d]$$
$$\begin{align*}
	\frac{dL}{dt} &= \sum\limits_{i}\left(\dot q_{i} \frac{d}{dt}\frac{\partial L}{\partial \dot q_{i}} + \frac{\partial L}{\partial \dot q_{i}} \frac{\partial q_{i}}{\partial t}\right) \\
	&= \frac{d}{dt}\sum\limits_{i}\dot q_{i}\frac{\partial L}{\partial \dot q_{i}}
\end{align*}$$
$$H = \sum\limits_{i} \dot q_{i} \frac{\partial L}{\partial \dot q_{i}} - L$$
$$\begin{align*}
	\frac{dH}{dt} &= - \frac{dL}{dt} + \frac{d}{dt}\sum\limits_{i}\dot q_{i}\frac{\partial L}{\partial \dot q_{i}} \\
	&= - \frac{dL}{dt}+ \frac{dL}{dt} \\
	&= 0
\end{align*}$$
- therefore, $H$ is a constant, independent of time, ie: it is conserved
- this is called the energy