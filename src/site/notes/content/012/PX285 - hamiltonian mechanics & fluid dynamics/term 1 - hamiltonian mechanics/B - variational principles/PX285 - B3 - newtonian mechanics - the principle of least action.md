---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/b-variational-principles/px-285-b3-newtonian-mechanics-the-principle-of-least-action/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-09T10:41:16.759+00:00"}
---

## the principle of least action
- in newtonian mechanics, 'classical' trajectories are those that extremize the *action*, which is called *'the principle of least action'* : 
$$\begin{align*}
	A &= \int_{t_{0}}^{t_{1}} {L}\,dt \\
	\text{where, } L &= T-V
\end{align*}$$
- this can be used to rederive newton's laws, and to formulate a new, more general, statement of mechanics  
## modelling the trajectory of a particle
- a particle moving along a trajectory $(x_{0},t_{0})\to (x_{1},t_{1})$
- let, $(x_0,t_0)=(0,0)$, and $(x_{1},t_{1})= (X,\tau)$
- the particle can take multiple paths, one with a constant velocity, many with varying velocities
- parameterizing the paths using one scalar parameter, $b=constant$, an equation is formulated, which represents the 'candidate' paths: 
$$x(t)=\frac{t}{\tau}X+b(\tau-t)t$$
- checking whether the equation starts and finishes at the correct fixed points: $x(0)=0$; $x(\tau)= X$ 
- $b$ allows inclusion of acceleration

## a falling particle
- for a mass, $m$, falling under gravity from a height, ${} x$, the lagrangian is: 
$$L = T-V = \frac{1}{2}mv^{2} - mgx$$
- using the candidate paths equation: 
$$\begin{align*}
	x(t) &= \frac{t}{\tau}X+b(\tau-t)t \\
	\implies v = \dot x(t) &= \frac{X}{\tau} + b(\tau-2t)
\end{align*}$$
- using the principle of least action: 
$$\begin{gather}
	A(b) = \int_{t_{0}}^{t_{1}}\left[\frac{1}{2}m \left[\frac{X}{\tau}+b(\tau-2t)\right]^{2} - mg \left[\frac{t}{\tau}X + b(\tau-t)t\right]\right]\,dt \\
	\vdots \\
	A(b) = \frac{m}{2}\left(\frac{b^{2}\tau^{3}}{3} - \frac{bg\tau^{3}}{3}- g\tau X + \frac{X^{2}}{\tau}\right)
\end{gather}$$
- the action has an extremum (here, a minimum) when: 
$$\begin{gather}
	\frac{dA}{db} = \frac{m\tau^{3}(2b-g)}{6} = 0 \\
	\implies b = \frac{g}{2}
\end{gather}$$
- therefore, it is found that: 
$$\begin{align*}
	x(t) &= \frac{t}{\tau}X + \frac{g}{2}(\tau-t)t = v_{0}t+ \frac{1}{2} gt^{2} \\
	\implies v &= \dot x(t) = \frac{X}{\tau}+ \frac{g\tau}{2}+gt
\end{align*}$$
