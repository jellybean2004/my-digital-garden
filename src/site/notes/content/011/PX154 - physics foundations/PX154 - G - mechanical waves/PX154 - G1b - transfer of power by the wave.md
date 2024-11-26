---
dg-publish: true
---

[YF 15.5]
- we know that waves transfer energy
- more useful to consider the power transfer, ie: rate of energy transfer
	- leads to 
	$$P = -T \frac{\partial y}{\partial x} \frac{\partial y}{\partial t}$$
	- if we take $y(x,t) = A \cos(kx-\omega t)$: 
	$$P = TA^{2}k \omega \sin^{2}(kx-\omega t)$$
	- ![Pasted image 20231125160137.png](/img/user/pics/Pasted%20image%2020231125160137.png)
	- power oscillates at twice the wave's frequency: 
	$$f_{P} = 2\omega$$ 
	- let's simplify this. take $v= \frac{\omega}{k}$ and $v^{2} = \frac{T}{\mu}$: 
	$$\implies k=\omega \sqrt{\frac{\mu}{T}}$$
		$$\therefore P(x,t) = \omega^{2} A^{2} \sqrt{\mu T}\sin ^{2}(kx-\omega t)$$
			where, $z = \sqrt{\mu T}$, often called '*impedance*'
	- the average power transmitted over a wave cycle: 
	$$P_{av} = \frac{1}{2}\omega^{2} A^{2} z$$
	- $P$ is proportional to $z$, and the squares of $A$ and $\omega$ of the wave
		- this is true for mechanical waves
		- however, for EM waves, we will see later