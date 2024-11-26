---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-282-stars-and-the-solar-system/d-stellar-structure-and-interiors/px-282-d7-pp-1-fusion-chain/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:39:58.381+00:00"}
---

- considering the hydrogen-fusion reaction: 
$$4\,{}_{1}^{1}\text{H} \to {}_{2}^{4}\text{He}$$
- governed by conservation laws:
	- electric charge
	- nucleon number
	- lepton number
	- energy and momentum
- it is detailed in the *PP1 chain*, which is the most common in the sun
- starts with the formation of deuterium: 
$$2\,{}_{1}^{1} \text{H} \to {}_{1}^{2} \text{H} + e^{+} + \nu_{e}$$
- here, a proton has decayed into a neutron: 
$$p \to n + e^{+} + \nu_{e}$$
- next: 
$$\begin{gather}
	{}_{1}^{2} \text{H} + {}_{1}^{1} \text{H} \to {}_{2}^{2} \text{He} + \gamma \\\\
	 2\,{}_{2}^{3} \text{He} \to {}_{2}^{4} \text{He} + 2{}_{1}^{1} \text{H} 
\end{gather}$$
- overall: 
 $$4\,{}_{1}^{1} \text{H} \to {}_{2}^{4} \text{He} + 2e^{+} + 2\nu_{e} + 2\gamma$$
## energy released
- the reaction rates are set by the slowest process
- for PP1, the initial decay of $p\to n$ requires the weak nuclear force and collisions, and it takes $10^{10}$ years for a given proton

![Pasted image 20241114104722.png](/img/user/pics/Pasted%20image%2020241114104722.png)

- energy is needed to overcome the strong nuclear force and escape the coulomb potential well
- comparing the thermal and the coulomb energy: 
$$\frac{3}{2}k_{B}T = \frac{Z_{1}Z_{2}e^{2}}{4\pi\epsilon_{0}r}$$
- the required temperature for this case would be: $T\approx 1.1\times10^{10}\,K$, this is too high, and it can be concluded that the thermal energy is not enough

- the only way this can happen is due to [[content/012/PX262 - quantum mechanics/B - introduction/PX262 - B5 - quantum tunnelling\|quantum tunnelling]] 
- according to [[content/012/PX262 - quantum mechanics/A - recap/PX262 - A7 - the uncertainty principle\|the uncertainty principle]] 
$$\Delta p \, \Delta x > \hbar$$
- $\Delta x$ can be large enough to 'cross the gap'
- reaction ratios: 
$$R_{1,2} = n_{1}n_{2}\sigma v$$
	where, $n_{1}$ and $n_{2}$ are number densities; $\sigma$ is the cross-section for collisions; $v$ is the relative velocity
- the probability of tunnelling: 
$$P \propto \exp\left(- \frac{2\pi^{2}U}{E}\right)$$
- the velocity: 
$$v \propto \exp\left(- \frac{E}{k_{B}T}\right)$$
![Pasted image 20241114104423.png](/img/user/pics/Pasted%20image%2020241114104423.png)

- expanding the exponentials: 
$$R_{pp}\propto \rho^{2}X_{H}^{2}T^{4}$$
	where, $\rho=$ general mass density; $X=$ mass fraction of hydrogen
- the energy generation rate per unit mass: 
$$\epsilon_{pp}= \rho X_H ^{2} T^4$$
## other reactions
- **CNO cycle** 
	- ${} \text{H}\to \text{He} : \epsilon_{CNO} \propto \rho X_{H} X_{CNO} T^{20} {}$ for $T\sim 10^{8}\,K$
	- the core gets denser as the reaction progresses, causing it to shrink and get hotter
	- at high enough temperature, $He$ can fuse
- **triple $\alpha$ reaction**: 
$$3 \, {}_{2}^{4} \text{He} \to {}_{6}^{12} \text{C} + \gamma$$
	- $\epsilon_{3\alpha} \propto \rho^{2} Y^{3} T^{40}$ for $T>\sim10^8\,K$

![Pasted image 20241114105332.png](/img/user/pics/Pasted%20image%2020241114105332.png)
- the energy gets progressively lower, thus less time is taken for subsequent fusions into heavier nuclei