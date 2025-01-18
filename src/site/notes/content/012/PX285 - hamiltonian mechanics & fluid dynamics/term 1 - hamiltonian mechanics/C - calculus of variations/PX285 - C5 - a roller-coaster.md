---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/c-calculus-of-variations/px-285-c5-a-roller-coaster/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-09T11:21:51.844+00:00"}
---

- the arc-length coordinate, $s$, is used to describe the motion of a roller coaster, which represented the distance moved along the track from an arbitrary starting point
- the height of the track at any point, $s$, is given by $h(s)$
- the lagrangian is: 
$$L = \frac{1}{2}m\dot s^{2} -mgh(s)$$
- using the euler-lagrange equation: 
$$\begin{gather*}
	mg \frac{dh}{ds}-m\ddot s = 0 \\
	\ddot s = -g \frac{dh}{ds}
\end{gather*}$$
## solutions
- the above differential equation can always be solved by adopting some numerical approach, eg: finite difference approach - discretize $s$ and $t$

- it can also be solved analytically
- eg: $h(s)=\alpha s$: 
$$\ddot s = -\alpha g$$
	- integrating both sides: 
	$$\dot s = - \alpha gt + v_{0}$$
	- integrating again: 
	$$s = - \frac{1}{2} \alpha gt^{2}+ v_{0}t + s_{0}$$

- also, for $h(s) = \frac{1}{2}cs^{2}:$ 
$$h'(s) = cs$$
	- the $h(s)-s$ graph is not a parabola - it is a *cycloid*
	$$\ddot s = -gcs = -\omega^{2} s$$
		where, the equation is in simple harmonic motion, and $\omega = \sqrt{gs}$ is the angular frequency
	- this is a 'perfect' SHM for all amplitudes, not necessarily small, neglecting friction
