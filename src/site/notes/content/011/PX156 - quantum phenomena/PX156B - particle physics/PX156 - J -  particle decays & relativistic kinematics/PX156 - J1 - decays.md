---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-b-particle-physics/px-156-j-particle-decays-and-relativistic-kinematics/px-156-j1-decays/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T20:06:00.622+00:00"}
---

## fermi's golden rule
- the transition rate from one state to another, ie: number of transitions per unit time, is proportional to the physics as drawn in the [[content/011/PX156 - quantum phenomena/PX156B - particle physics/PX156 - G - feynmann diagrams/E - feynmann diagrams\|feynmann diagrams]]: 
$$P(i\to f) \propto (amplitude)^{2}(phase\,space)$$

- measured experiment $\leftrightarrow$ calculate theory

- decays:  $1 \to n$
- collisions: $2 \to n$ 

## decays
- every particle decays, except the ones that have no lighter particles to decay to: electron, proton(?), and neutrino(?)

- usually looked at in a particle's rest frames
- otherwise, [[content/011/PX155 - classical mechanics and special reltivity/special relativity/PX155 - G - foundations of special relativity/G - foundations of special relativity\|special relativity]] needs to be used

- controlled by a decay law
- given an ensemble of $N$ particles at time, $t=0$, the number of particles left at time, $t$ is: 
$$N(t) = N(0)\exp\left({-\frac{t}{\tau}}\right)$$
	where, the parameter, $\tau\equiv$ average lifetime of a particle
- in particle physics, the decay rate, $\Gamma=\frac{1}{\tau}$, is used:  
$$ N(t) = N(0)\exp\left( -\Gamma t \right)$$
- **note**: $\Gamma$ is a transition rate $\to LHS$ of *fermi's golden rule*
### derivation
$$\begin{align*}
	N(t+\Delta t) &= N(t)-N(t)\Gamma\Delta t \\
	\frac{N(t+\Delta t) - N(t)}{\Delta t} &= -N(t)\Gamma \\
	\lim_{t\to0}: \frac{dN(t)}{dt} &= -N(t)\Gamma \\
	\ln\left(\frac{N(t)}{N(0)}\right) &= -\Gamma t \\
	\therefore N(t) &= N(0)e^{-\Gamma t}
\end{align*}$$
