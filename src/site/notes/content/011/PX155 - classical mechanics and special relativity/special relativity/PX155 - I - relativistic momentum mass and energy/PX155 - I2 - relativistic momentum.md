---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/special-relativity/px-155-i-relativistic-momentum-mass-and-energy/px-155-i2-relativistic-momentum/","noteIcon":"1","created":"2025-08-27T13:14:05.320+01:00","updated":"2024-11-26T19:59:27.000+00:00"}
---

## derivation
- $p$ is conserved for $v<<c$ , and we need a linear transformation
- try $m=f(v)m_{0}$ , where $m_{0}=$ "rest mass", $f(v)\to1$ as $v\to0$
- now, $p=mv = f(v)m_{0}u=0$

- conserve momentum and mass in the centre of mass frame, $S':$
	$$f(u)m_{0}u - f(-u)m_{0}u =0 ... [i]$$
	$$\implies f(u)=f(-u)$$
	$$f(u)m_{0} + f(-u)m_{0} = M_{0}...[ii]$$
- do the same in $S$:
	$$f(v)m_{0}v = f(u)M_{0}u...[iii]$$
	$$f(v)m_{0} + m_{0} = f(u)M_{0}...[iv]$$

- $[i]$ in $[ii]$:
$$2f(u)m_{0} = M_{0}$$
- $[iii]$ becomes:
$$f(v)m_{0}v = 2f^{2}(u)u m_{0} \implies f(v)v = 2f^{2}(u)u \;...[v]$$ 
- $[iv]$ becomes: $$f(v)m_{0} + m_{0} = 2f^{2}(u)m_{0}$$
$$or, \;f(v) +1 = 2f^{2}(u)...[vi]$$
- divide $[v]$ by $v$ and subtract from $[vi]$: $$f(v)+1-f(v)= 2f^{2}(u) - 2f^{2}(u) \frac{u}{v}$$
$$or, \;f^{2}(u) (2-2 \frac{u}{v})=1$$
- ***but*** $$v= \frac{2u}{1+ \frac{u^{2}}{c^{2}}}$$
$$or\;2 \frac{u}{v} = 1+ \frac{u^{2}}{c^{2}}$$
- therefore, $$f^{2}(u) (2-1- \frac{u^{2}}{c^{2}})=1$$
$$or, \; f(u) = \frac{1}{\sqrt\frac{1- u^{2}}{c^{2}}} = \gamma(u)$$
- so $p$ is conserved in both frames if $$m=\gamma(v)m_{0}$$
$$p=\gamma(v)m_{0}v$$
	- this gives us relativistic mass and momentum

## nothing moves faster than $c$
- as $v\to c$ , $p\to\infty$
- we have:
$$F= \frac{dp}{dt} \implies \Delta p = \int_{t_{0}}^{t_{f}}F.dt'$$
- we will need either infinite force or infinite time to accelerate a mass to $c$

## examples
- eg: a particle of rest mass, $m_{0}$, moving at $v=0.8c$, collides with an identical but stationary particle, and forms a new particle of rest mass, $M_{0}$, and speed, $w$
	- to find: $M_{0}, w$
	- for $v = \frac{4}{5}c$ , $\gamma = \frac{5}{3}$
	- conserving mass:
		- total initial mass $=\gamma(v)m_{0} + m_{0} = \frac{8}{3}m_{0}$
		- total final mass $= \gamma(w)M_{0} = \frac{8}{3}m_{0}... [i]$
	- conserving momentum:
		- total initial momentum $=\gamma(v)m_{0}v$
		- total final momentum $= \gamma(w)M_{0}w$
	
$$\gamma(v)m_{0}v = \gamma(w)M_{0}w$$
	
$$\frac{5}{3}m_{0} \frac{4}{3}c = \frac{8}{3}m_{0}w$$
	
$$\therefore w=\frac{1}{2} c$$
	
$$\gamma\left(w=\frac{c}{2}\right)= 1.1547$$
		- from $[i]$:
$$M_{0} = \frac{8}{3\times1.1547} = 2.309 \,m_{0}$$
