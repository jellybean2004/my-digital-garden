---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/d-the-hamiltonian/px-285-d4-roller-coaster-revisited/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:08.168+00:00"}
---

- revisiting [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/C - calculus of variations/PX285 - C5 - a roller-coaster\|the roller-coaster problem]]
- the lagrangian: 
$$L = \frac{1}{2}m\dot s ^{2}- mgh(s)$$
- the hamiltonian: 
$$H = \dot s \frac{\partial L}{\partial \dot s} - L =\frac{1}{2}m\dot s^{2} + mgh(s) = E$$
- seeking an equation for the trajectory, ie, an ODE for $\dot s:$ 
$$\begin{gather}
	\dot s^{2} = \frac{2}{m}(E -mgh(s)) \\
	\frac{ds}{dt} = \pm\sqrt{\frac{2}{m}} \sqrt{E-mgh(s)} \\\\
	\pm \sqrt{\frac{m}{s}} \int_{s_{0}}^{s_{1}} \frac{ds'}{\sqrt{E - mgh(s)}} = \int_{0}^{t} dt' \\\\
	\implies f(s) = t
\end{gather}$$
- therefore, $t$ as a function of $s$ is obtained, which can then be used to obtain $s$ as a function of $t:$ 
$$s = f^{-1}(t)$$
- consider a promising particular case, a cycloid: 
$$h(s) = \frac{1}{2}cs^{2}$$
$$t = \pm \sqrt{\frac{m}{s}} \int_{s_{0}}^{s_{1}} \frac{ds'}{\sqrt{E - mg \left(\frac{1}{2}cs^{2}\right)}}$$
- try: $s = \sqrt{\frac{2E}{mgc}} \sin\theta$ 
	$\implies ds' = \sqrt{\frac{2E}{mgc}} \cos\theta\,d\theta$
$$\frac{mgc}{2} s'^{2} = \frac{mgc}{2} \frac{2E}{mgc}\sin^{2}\theta = E\sin^{2}\theta$$
$$\begin{align*}
	t &= \pm\sqrt{\frac{m}{2}} \int_{\theta(s_{0})}^{\theta(s)} \frac{\sqrt{\frac{2E}{mgc}}\cos\theta\,d\theta}{\sqrt{E(1-\sin^{2}\theta)}} \\
	&= \pm \sqrt{\frac{m}{2}} \sqrt{\frac{2}{mgc}} \int_{\theta(s_{0})}^{\theta(s)} d\theta \\
	&= \pm\sqrt{\frac{1}{gc}} \; [\theta(s_{0}) - \theta(s) ]
\end{align*}$$
- define $\omega^{2}=gc:$ 
$$\begin{gather*}
	\omega t = \pm(\theta(s) - \theta(s_{0})) \\
	\omega t \pm \theta(s_{0}) = \pm \theta(s)  \\
	\sin(\omega t + \phi) = \sin\theta = s \sqrt{\frac{mgc}{2E}} \\\\
	\therefore s = \sqrt{\frac{2E}{mgc}}\sin(\omega t + \phi)
\end{gather*}$$
- this is an equation of simple harmonic motion
- at maximum height: 
$$s(0) = \sqrt{\frac{2E}{mgc}} \sin\phi = s_{0}$$
