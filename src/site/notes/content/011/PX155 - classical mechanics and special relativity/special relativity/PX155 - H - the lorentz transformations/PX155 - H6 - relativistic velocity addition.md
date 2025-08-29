---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/special-relativity/px-155-h-the-lorentz-transformations/px-155-h6-relativistic-velocity-addition/","noteIcon":"1","created":"2025-08-27T13:14:05.268+01:00","updated":"2024-11-26T19:58:42.000+00:00"}
---

## derivation and examples
- light travels at $c$ in all initial frames
- what about objects moving at $v'<c$ in frame $S'$ along the x axis? what is $v$ for that object in frame $S$?
- use *LTs*: $$t=\gamma(t' + \frac{ux'}{c})$$
$$x = \gamma (x'+ ut')$$
- differentiating wrt $t'$: $$\frac{dt}{dt'} = \gamma\left(1+ \frac{u}{c^{2}} \frac{dx'}{dt'} \right) = \gamma \left(1 + \frac{uv'}{c^{2}}\right)$$
$$\frac{dx}{dt'} = \gamma \left( \frac{dx'}{dt'} + u \right) = \gamma(v'+u)$$
- we know:
$$v = \frac{dx}{dt} = \frac{dx}{dt'} \frac{dt'}{dt}= \frac{dx}{dt'} \left (\frac{dt}{dt'}\right)^{-1}$$
- the relativistic velocity addition is: $$\therefore v = \frac{v'+u}{1+ \frac{uv'}{c^{2}}}$$
$$\therefore v' = \frac{v-u}{1- \frac{uv}{c^{2}}}$$
- eg: two particles approach each other at $0.8c$ - "head on" - in the rest frame of some observer. what is the speed of one particle in the rest frame of the other?
	- let observer at rest in $S'$
	- $S'$ moves at $+v'$ in the rest frame of left-going particle. so, taking that frame as $S$ with $u=v'$
	$$v = \frac{v'+u}{1+ \frac{uv'}{c^{2}}} = \frac{v'+u'}{1+ \frac{uv'}{c^{2}}} = \frac{0.8c+0.8c}{1+0.8^{2}} \approx 0.9756c$$

- eg: two aeroplanes approach each other head on at $500 mph$. find the speed of one in the rest frame of other, as a correction to the galilean result
	- we want to find:
$$\delta v = \frac{v'+u}{1+ \frac{uv'}{c^{2}}} -(v'+u)$$  
	$$\delta v = \frac{v'+u-(1+ \frac{uv'}{c^{2}})(v'+u)}{1+ \frac{uv'}{c^{2}}} = \frac{-(v'+u)uv'}{(1+ \frac{uv'}{c^{2}})c^{2}}$$
	$$\delta v \approx \frac{-uv'}{c^{2}}(v'+u)$$
	- we have, $c=186,000 mps = 186,000\times3600 mph$
	- therefore,
$$\delta v \approx -5.6\times 10^{-10}$$
## more general motion
- what about a 3D velocity vector with components $(v_{x},v_{y}, v_{z})$?
- in $S'$: $v_{y}' = \frac{dy'}{dt'} = \frac{dy'}{dt} \left(\frac{dt'}{dt}\right)^{-1}$
- $\frac{dt'}{dt} = \gamma \left(\frac{1-u}{c^{2}}v_{x} \right)$
- since $y'=y$, $\frac{dy'}{dt} = \frac{dy}{dt} = v_{y}$
$$v_{y}' = \frac{v_{y}}{\gamma(1-\frac{uv_{x}}{c^{2}})}$$
- similarly,
$$v_{z}' = \frac{v_{z}}{\gamma(1-\frac{uv_{x}}{c^{2}})}$$
- and,
$$v_{x}' = \frac{v_{x}-u}{(1-\frac{uv_{x}}{c^{2}})}$$
aberration of light
- eg: a beam of light travels down the y-axis toward origin of frame $S$. what does $S'$ measure?
	- in $S$, beam has velocity, $(0,-c,0)$
	- in $S'$
	
$$v_{x}' = \frac{v_{x}-u}{1- \frac{uv_{x}}{c^{2}}} = -u$$
	
$$v_{y}' = \frac{v_{y}}{1- \frac{uv_{x}}{c^{2}}} = -\frac{c}{\gamma}$$
	- in frame $S'$:
$$\vec v' = (-u, -\frac{c}{\gamma}, 0)$$
	- sanity check:
$$|\vec v'|^{2} = u^{2} + \frac{c^{2}}{\gamma^{2}} = u^{2} + c^{2}\left( \frac{1- u^{2}}{c^{2}} \right)= c^{2}$$
- 