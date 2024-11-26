---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-h-waves-at-boundaries/px-154-h2-two-strings-joined-together-transmission-and-reflection/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:52:36.985+00:00"}
---

## introduction
- string 1, and string 2 are joined at $x_{0}$
- the join is *perfect*
- mass per unit length of string 1 is $\mu_{1}$, and that for string 2 is $\mu_{2}$
- tension, $T$, and wave frequency, $\omega$, are same in both strings
- wave speed, $v=\sqrt{\frac{T}{\mu}}$ , is slower in the heavier string
- the frequency, $f$, should be the same in both the strings, otherwise the waves will go out of phase and the strings will come apart
- the wavelength, $\lambda = \frac{v}{f}$, is shorter in the heavier string as $v$ is slower, and $f$ is constant

## application
- concepts apply elsewhere: 
	- light from one medium into another, eg: air to glass
	- QM treatment of particles, eg: at potential step
	- electrical signals in electronics

- in general, expect three waves:
	- incident wave: 
	$$y_{i}(x,t) = A_{i}\cos(k_{1}x-\omega t)$$
	- reflected wave: 
	$$y_{r}(x,t) = A_{r}\cos(k_{1}x-\omega t)$$
	- transmitted wave: 
	$$y_{t}(x,t) = A_{t}\cos(k_{2}x-\omega t)$$
## what happens at the join?
- boundary conditions:
	- string is continuous (doesn't snap): 
	$$y_{string\; 1}(x_{0}) = y_{string\; 2}(x_{0}) \implies y_{i}+y_{r}= y_{t}$$
	- tension is the same in both strings
		- at the joint, the forces are equal
		- string only moves in the transition
- consider [[content/011/PX154 - physics foundations/PX154 - G - mechanical waves/PX154 - G1a - waves on a taut string\|PX154 - G1a - waves on a taut string]]  for forces on an element of the string
![Pasted image 20231129100336.png](/img/user/pics/Pasted%20image%2020231129100336.png)
- no change in gradient at the joint
- at $x_{0}$: 
$$\frac{\partial y_{i}}{\partial x} = \frac{\partial y_{r}}{\partial x} = \frac{\partial y_{t}}{\partial x}$$
- using these conditions, the reflection and transmission coefficients, $r$ and $t$ can be derived: 
$$\begin{align*}
	t = \frac{A_{t}}{A_{i}} &= \frac{2z_{1}}{z_{1}+z_{2}} \\ 
	r = \frac{A_{r}}{A_{i}} &= \frac{z_{2}-z_{1}}{z_{1}+z_{2}}
\end{align*}$$
	where, $z=\sqrt{\mu T}$ is the impedance
## observation
- for a wave approaching the join: ![Pasted image 20231129100954.png](/img/user/pics/Pasted%20image%2020231129100954.png)
- if $\mu_{1}<\mu_2$: ![Pasted image 20231129101039.png](/img/user/pics/Pasted%20image%2020231129101039.png)
- if $\mu_{1}>\mu_2$: ![Pasted image 20231129101106.png](/img/user/pics/Pasted%20image%2020231129101106.png)
- if $\mu_{1}= \mu_{2}$: ![Pasted image 20231129101212.png](/img/user/pics/Pasted%20image%2020231129101212.png)
## power transmission at the boundary
- derivation on moodle pdf

$$P_{i}= P_{r}+ P_{t}$$