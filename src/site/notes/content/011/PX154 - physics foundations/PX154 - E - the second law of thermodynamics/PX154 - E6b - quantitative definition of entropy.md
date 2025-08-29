---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-e-the-second-law-of-thermodynamics/px-154-e6b-quantitative-definition-of-entropy/","noteIcon":"1","created":"2025-08-27T13:14:08.593+01:00","updated":"2024-11-26T19:51:15.000+00:00"}
---

- a small change in entropy, $dS$, is given by a small amount of heat transfer, $dQ$, at a temperature, $T$: 
$$dS = \frac{dQ}{T}$$ [YF eqn 20.1]
- if a small amount of heat, $dQ$, is put into a system: 
$$dQ = dU + dW$$
	- $dU\to$ increase in internal energy $\implies$ increases randomness, and hence entropy.
	- $dW=pdV \to$ increase volume, molecules have more space to move in, and hence entropy increases

- **key notes**: 
	- the relationship given **only holds for reversible processes**
	- for an isothermal process, $T$ constant, we can write $\Delta S=\frac{Q}{T}$
	$$\begin{align*}
		Q = W &= nRT \ln{\frac{V_{2}}{V_{1}}} \\
		\Delta S &= nR\ln{\frac{V_{2}}{V_{1}}}
	\end{align*}$$
	- for an irreversible process, $\Delta S$ can still be found using a reversible process that has the same initial and final states.

- eg: heat $1kg$ water from $0\degree C \to 100\degree C$. what is the change in entropy?
	- heat capacity of water, ${} c_{mass}= 4190 JK^{-1}kg^{-1}$
	- $T$ is not constant
	$$\Delta S = \int_{state\;1}^{state\;2} \frac{dQ}{T}$$
	- heat, $Q$, is supplied to heat the water
	- $c_{mass}= \frac{1}{m} \frac{dQ}{dT}$
	- so, $dQ = m c_{mass}dT$
	$$\begin{align*}
		\Delta S &= \int_{T_{1}}^{T_{2}} \frac{m c_{mass}}{T}\,dT \\ 
		&= m c_{mass}\ln\frac{T_{2}}{T_{1}}
	\end{align*}$$
	$$\therefore \Delta S = 1.31 \times 10^{3}JK^{-1}$$
- cooling back down to $0\degree C$, $\Delta S = - 1.3 \times 10^{3}JK^{-1}$
	- ie: $\Delta S = 0$ for $0\degree C \to 100\degree C \to 0\degree C$
- this is the *entropy change of just the water*
- what about the entropy change of the universe?
	- if a reversible process is used to heat and cool the water, $0\degree C \to 100\degree C$, then, $\Delta S_{universe}=0$
	- however, if the water is heated on a bunsen burner, and cooled in a fridge the process will be *irreversible*: 
$$\begin{align*}
	\Delta S_{water} &= 0 \\ 
	\Delta S_{universe} &> 0
\end{align*}$$
- for all real processes: 
$$\Delta S_{universe}>0$$
- furthermore, for an isolated system: 
$$\Delta S \geq 0$$
- **comment**:
	- in *[[content/011/PX154 - physics foundations/PX154 - E - the second law of thermodynamics/PX154 - E4 - the carnot cycle\|the carnot cycle]]*, the cooling must be adiabatic
		- what about isochoric cooling?
			- if only the gas is considered, it can be cooled and heated between $A$ and $B$ reversibly
			- but in the engine, the "isolated system" must include the reservoir
	- what about *[[content/011/PX154 - physics foundations/PX154 - E - the second law of thermodynamics/PX154 - E5 - reversible and irreversible processes#heat transfers\|the example in the last section]]*?
		- irreversible (will not spontaneously retain)
		- can use two reversible processes: 
			- cool hot object from $100\degree C \to 50\degree C$
			- heat cold object to $50\degree C$
		- calculate $Q$ for each process (heat loss = heat gain)
		- calculate $\Delta S$ for each region and add to get the total
