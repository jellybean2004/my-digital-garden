---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-282-stars-and-the-solar-system/c-stellar-atmosphere/c1-boltzmann-and-saha-equations/px-282-c2a-the-boltzmann-equation/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:38:13.548+00:00"}
---

- the boltzmann equation gives how many electrons are in each state: $$\frac{N_{B}}{N_{A}} = \frac{g_{B}}{g_{A}}\exp\left(- \frac{E_{B}-E_{A}}{k_{B}T}\right)$$
## derivation
- from statistical mechanics, the probability that an electron is in state 1 , requiring an energy, $E_{1}$, over state 2, with an energy, $E_{2}$, for $E_{1}>E_{2}$, is given by: $$\frac{P_{1}}{P_{2}} = \frac{e^{-\frac{E_{1}}{k_{B}T}}}{e^{-\frac{E_{2}}{k_{B}T}}} = \exp\left({- \frac{E_{1}-E_{2}}{k_{B}T}}\right)$$
- if the temperature is low, $k_{B}T\to 0 \implies \frac{P_{1}}{P_{2}}\to0:$ the electrons go to the lowest state
- if the temperature is high, $k_{B}T\to\infty \implies \frac{P_{1}}{P_{2}}\to1 :$ with infinite energy, all states are equally accessible
- these are quantum states, defined by:
	$n:$ energy
	$l=n-1:$ angular momentum
	$m_{l}\in[-l,+l],\mathbb{Z}:$ alignment
	$m_{s}=\pm \frac{1}{2}:$ spin

- consider quantum numbers for $H:$
	- at ground state: 
		- $n=1$
		- $l = n-1 = 0$
		- $m_{l} = -l\to+l = 0$
		- $m_{s} = \pm \frac{1}{2}$
		- there are two energy states
	- at $n=2:$
		- $l= 0,1$
		- $m_{0}=0$, $m_{1}=-1,0,+1$
		- $m_{s}= \pm \frac{1}{2}$
		- there are 8 energy states

- states with the same $n$ have the same energy
- all possible states need to be included
- this gets done using '*statistical weights*', $g$, such that $g_{A}$ is the  number of states with the energy, $E_{A}$
- $\frac{P_{1}}{P_{2}}$ is for a given energy, not a given state, so accounting for states, the probability ratio becomes: 
$$\frac{P_{1}}{P_{2}} = \frac{g_{1}}{g_{2}}\exp\left(- \frac{E_{1}-E_{2}}{k_{B}T}\right)$$
- a stellar atmosphere has a large number of atoms, $N$
- the probability ratio is equivalent to the number ratios of atoms in each state, therefore, **the boltzmann equation** is obtained: 
$$\boxed{\frac{N_{B}}{N_{A}} = \frac{g_{B}}{g_{A}}\exp\left(- \frac{E_{B}-E_{A}}{k_{B}T}\right)}$$
- considering the atoms of a single element in a specified state of ionization with number of electrons, $N_x$, at an energy level, $E_x$
