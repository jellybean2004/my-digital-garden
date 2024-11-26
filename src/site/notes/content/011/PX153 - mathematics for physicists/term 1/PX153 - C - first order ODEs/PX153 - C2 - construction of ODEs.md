---
dg-publish: true
---

- eg: you have  lump of radioactive material. how does the number of radioactive nuclei change over time?
	- variables:
		- independent - time($t$)
		- dependent - number of radio active nuclei ($N(t)$)
	- empirical observation:
		- rate of decay is proportional to the number of nuclei: $\frac{dN}{dt}=-\alpha N$
	- try a solution: $N(t)=Ae^{\lambda t}$
			$\frac{dN}{dt}=\lambda Ae^{\lambda t}=-\alpha N$
			$\lambda =-\alpha$
	- and the general solution: $N(t)=Ae^{-\alpha t}$
	- *aside*: why $N(t)=Ae^{-\alpha t}$?
		- $e^x$ is defined by, if $y=e^x$, $y=y'$, $y(0)=1$
		- if $\frac{dN}{dt}\propto N$, solution will be an exponential
	- to find a particular solution, we need a boundary condition
		- if $N(0)=N_0$ then, the particular solution is $N(t)=N_0e^{-\alpha t}$

- eg: a large tank of water with cross-section $A$, and a small opening on the side, at the bottom, with cross-section $a$. find the ODE that described the height of the water
{ #a397d9}

	- ![Pasted image 20231023144607.png](/img/user/pics/Pasted%20image%2020231023144607.png)
	- variables:
		- independent - $t$
		- dependent - $h(t)$
	- the water exits the opening at speed $v(h)$ 
		- in a time $\Delta t$, the volume of water leaving is $\Delta V = a \;v(h) \Delta t$
			- corresponds to a change in height: 
			$$\Delta h = h(t +\Delta t)-h(t) =  \frac{\Delta v}{A}= \frac{-av(h)\Delta t}{A}$$
			- to find $v(h)$, we use bernaulli's equation of energy conservation in fluid flow: 
			$$p_{0} + \rho g h + \frac{1}{2}\rho v^{2}= constant$$
				- basically $E = KE + PE$
			$$\implies \rho gh = \frac{1}{2}\rho v^{2} \implies v(h)=\sqrt{2gh}$$
			- so we have 
			$$\frac{h(t+\Delta t)-h(t)}{\Delta t} = - \frac{a}{A}\sqrt{2gh}$$
			- taking the limit $\Delta t \to 0$ gives is the derivative 
			$$\frac{dh}{dt}= - \frac{a}{A}\sqrt{2gh}$$
