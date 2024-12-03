---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-f-collisions/px-155-f1-collisions-in-1-d/","created":"2024-10-01T18:27:09.731+01:00","updated":"2024-11-26T19:57:31.605+00:00"}
---

## conservation of momentum and reference frames
![Pasted image 20231114064745.png](/img/user/pics/Pasted%20image%2020231114064745.png)
- speeds are measured in "lab frame", ie: relative to some stationary equipment 
- assume: 
	- momentum is conserved (no external forces)
	- potential energy is irrelevant, ie: no long range forces

- conserve momentum: $m_{1}u_{1} + m_{2}u_{2} = m_{1}v_{1}+m_{2}v_{2}$:
$$p_{1}+p_{2}=q_{1}+q_{2}$$

- consider $v_{cm} = \dot r_{cm} = \frac{m_{1}u_{1}+m_{2}u_{2}}{m_{1}+m_{2}} = \frac{p_{1}+p_{2}}{m_{1}+m_{2}}$
	- or, $v_{cm} = \frac{q_{1}+q_{2}}{m_{1}+m_{2}} = \frac{m_{1}v_{1}+m_{2}v_{2}}{m_{1}+m_{2}}$
	- $v_{cm}$ is conserved if momentum is conserved

- consider a second observer is moving in the lab at speed $v_{cm}$. defines COM frame denoted with a dash
	- so,
		$u_{1}=u_{1}' + v_{cm} \implies u_{1}' = u_{1}-v_{cm}$ 
		$u_{2}=u_{2}' + v_{cm} \implies u_{2}' = u_{2}-v_{cm}$
		- note: $v_{cm}' = 0 = \frac{p_{1}'+p_{2}'}{m_{1}+m_{2}} = \frac{q_{1}'+q_{2}'}{m_{1}+m_{2}}$
	- total momentum $=0$ in COM frame
	- ![Pasted image 20231114070317.png](/img/user/pics/Pasted%20image%2020231114070317.png)
	- only unknown is magnitude of $q_{1}'$ and $q_{2}'$
## completely inelastic collision
- all magnitude of momenta is lost , $q_{1}'=q_{2}'=0\implies$ particles stick after collision
- in lab frame: $v_{1}=v_{2}= v_{cm}$
## elastic collision
- kinetic energy is conserved, $T = \frac{p^{2}}{2m}$
	- $\frac{(p_{1}')^{2}}{2m_{1}}+ \frac{(p_{2}')^{2}}{2m_{2}} = \frac{(q_{1}')^{2}}{2m_{1}} + \frac{(q_{2}')^{2}}{2m_{1}}$
	- let $p' = |p_{1}'| = |p_{2}'|$ and $q' = |q_{1}'| = |q_{2}'|$
	- hence, $\frac{1}{2}(\frac{1}{m_{1}} + \frac{1}{m_{2}})(p')^{2} = \frac{1}{2}(\frac{1}{m_{1}} + \frac{1}{m_{2}})(q')^{2}$
	$$\therefore (p')^{2}=(q')^{2}$$
	- the magnitudes of $p'$ and $q'$ are equal
	- so, the collision only reverses momenta, doesn't change magnitude

- eg: $m_{1}=7kg$, $m_{2}=3kg$, $u_{1}=5ms^{-1}$, $u_{2}=-5ms^{-1}$. to find: $v_{1}, \; v_{2}$ if the collision is (a) completely inelastic (b) elastic
	- $v_{cm} = 2ms^{-1}$
		(a) completely inelastic
			$v_{1}= v_{2} = 2ms^{-1}$
		(b) elastic
		- move into COM frame
			$u_{1}'=u_{1}-v_{cm} = 3ms^{-1}$
			$u_{2}'=u_{2}-v_{cm} = -7ms^{-1}$
			$v_{1}' = -3ms^{-1}$
			$v_{2}' = 7ms^{-1}$
		- back to lab frame
			$v_{1} = v_{1}' + v_{cm} = -1ms^{-1}$
			$v_{2} = v_{2}' + v_{cm} = 9ms^{-1}$
		- sanity check: $v_{cm} = \frac{m_{1}v_{1}+m_{2}v_{2}}{m_{1}+m_{2}} = 2ms^{-1}$
