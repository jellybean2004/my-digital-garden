---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/special-relativity/px-155-i-relativistic-momentum-mass-and-energy/px-155-i9-how-far-could-you-go/","noteIcon":"1","created":"2025-08-27T13:14:05.286+01:00","updated":"2024-11-26T19:59:40.000+00:00"}
---

- depart earth and accelerate with $1g$. how far can you travel in $10 \, years$?
## outline derivation:
- let $S$ be the rest frame of the earth, $S'$ be your instantaneous rest frame, which is moving at $v$ in frame $S$
- after $\delta t'$ in $S'$, you are moving at speed, $\delta v'$, in $S'$, which is no longer your rest frame
	- in $S$,
$$\delta v = \frac{v+\delta v'}{1+v  \frac{\delta v'}{c^{2}}} -v$$
	$$\delta v = \frac{1- \frac{v^{2}}{c^{2}}}{1+v  \frac{\delta v'}{c^{2}}} \delta v'$$
	- time dilation:
$$\delta t = \gamma \delta t'$$
	$$\frac{dv}{dt} = \lim_{\delta t \to 0}  \frac{\delta v}{\delta t} = \frac{1}{\gamma^{3}} \frac{dv'}{dt} = \frac{1}{\gamma^{3}}a' = \frac{g}{\gamma^{3}}$$
	- this is a velocity dependent acceleration problem, because $\gamma=\gamma(v)$:
$$\int_{0}^{v} dv = \int_{0}^{t} \frac{g}{\gamma^{3}}.dt \; ...$$
		- we get $v(t)$. rearrange for $\gamma(t)$
	- integrate $v(t)$ from $0$ to $T$ to find the distance. need $T$ in terms of $T'$, where $T'=10 \, years$:
$$\delta t = \gamma\delta t'$$
			where, $\gamma=\gamma(t)$
	$$\int_{0}^{T} \frac{1}{\gamma(t)}dt = \int_{0}^{T_{0}'} dt'$$
		- get $T(T')$
	- distance travelled in frame $S$:
$$x(T') = \int_{0}^{T(T')} v(t).dt$$
	- for $a'=9$, $T'=10/,years$, $x(T') = 14,900 \,ly$
