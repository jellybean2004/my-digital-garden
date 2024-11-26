---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-d-simple-harmonic-motion/px-155-d8-3-regimes-of-damping/","created":"2024-10-01T18:27:09.666+01:00","updated":"2024-11-26T19:55:58.143+00:00"}
---

- sign of determinant $(\frac{\gamma}{2})^{2}-\omega^{2}$ determines behaviour
	- $\gamma < 2\omega:p$ complex, oscillating, decaying
	- $\gamma > 2\omega:p$ real and negative, not oscillating, decaying
	- $\gamma = 2\omega:p=- \frac{\gamma}{2}$ special case
### light damping
- AKA under damping
- $\gamma<2\omega$: rewrite $p=- \frac{\gamma}{2} \pm i\sqrt{\omega^{2}-(\frac{\gamma}{2})^2}$
- let $p= - \frac{\gamma}{2}\pm i \omega'$
	$z= ae^{pt}=a \exp{(- \frac{\gamma}{2}\pm iw')t}$
	$z = a e^{\frac{-\gamma t}{2}}e^{\pm i \omega't}$
	$a=|a|e^{i\phi}$ and $A=|a|$
	$$z=|a|e^{i(\pm \omega' t + \phi)}$$
$$and \; x=\mathbb Re (z)= |a|e^{\frac{\gamma t}{2}}\cos{(\omega' t+\phi)}$$
- properties:
	- frequency reduces: $\omega \to \omega'$
	- exponentially decaying amplitude
	- amplitude decreases by a factor $\frac{1}{e}$ in time $\frac{2}{\gamma}$
	- energy decreases by a factor $\frac{1}{e}$ in time $\frac{1}{\gamma}$
### heavy damping
- AKA over damping
- if $\gamma > 2\omega$, $p$ is real and negative and can take 2 values
$$p_{1}=\frac{\gamma}{2} - \sqrt{\omega^{2}-(\frac{\gamma}{2})^{2}} \; and \; p_{1}=\frac{\gamma}{2} + \sqrt{\omega^{2}-(\frac{\gamma}{2})^{2}}$$
- more general solution:
$$z=ae^{p_{1}t}+be^{p_{2}t}$$
	- sum of two equally valid solutions 
$$x=\mathbb Re(z)$$
- no oscillations, just a decay
### critical damping
- if $\gamma = 2\omega$, $z=ae^{pt}=ae^{-\frac{\gamma}{2}t}$ 
- BUT $\ddot z + \gamma \dot z + \frac{\gamma^{2}z}{4} = 0$ has an extra solution $z=bte^{- \frac{\gamma t}{2}}$ 
- more general solution:
$$z=(a+bt)e^{\frac{-\gamma t}{2}}$$
- gives the *shortest time to return to the initial displacement* NOT heavy damping, which slows the return to zero
  ![Pasted image 20231113085521.png](/img/user/pics/Pasted%20image%2020231113085521.png)