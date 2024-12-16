---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/c-entropy-and-temperature/px-284-c1-entropy/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T23:41:45.320+00:00"}
---

## the boltzmann entropy formula
- the entropy associated with a macrostate of an isolated system in an equilibrium is given by the **boltzmann entropy formula**: 
$$\boxed{S = k_{B} \ln\Omega}$$
	where, $\Omega$ is the number of equally likely microstates associated with this macrostate
- consequently, the more **microstates accessible, the less defined is the system**, and the greater the entropy, thus **entropy is related to disorder**
## combining systems
- **in thermodynamics**, if two systems with entropies, $S_{1}$ and $S_{2}$, the total entropy: 
$$S_{tot} = S_{1} + S_{2}$$
- **in statistical mechanics**, $\Omega_{tot} = \Omega_{1}\times\Omega_{2}:$ 
$$S_{tot} = k_{B} \ln(\Omega_{1}\times\Omega_{2}) = k_{B}\ln\Omega_{1} + k_{B}\ln\Omega_{2} = S_{1} + S_{2}$$
## isothermal expansion
- consider that two systems of equal volume, $V_0$,  are connected with a pipe with a tap
- **in thermodynamics**: 
$$\Delta S = \int_{i}^{f}dS = \int_{V_{0}}^{2V_{0}} \frac{p}{T}dV = \int_{V_{0}}^{2V_{0}} \frac{Nk_{B}}{V} dV = Nk_{B}\ln 2$$
- **in statistical mechanics**, each molecule now has two choices: $LHS$ or $RHS$
$$\Omega_{tot} = \Omega_{0} \times 2^{N}$$
	where, $\Omega_{0}$ is the number of original microstates
- so: 
$$\Delta S = k_{B}\ln(2^{N}\Omega_{0}) - k_{B}\ln\Omega_{0} = Nk_{B}\ln(2)$$
## the second law
- **in thermodynamics**, an isolated state in equilibrium is a state of maximum entropy
- **in statistical mechanics**, an isolated system in equilibrium will adopt the state with the highest number of microstates