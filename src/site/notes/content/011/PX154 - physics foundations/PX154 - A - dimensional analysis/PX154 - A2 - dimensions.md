---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-a-dimensional-analysis/px-154-a2-dimensions/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T23:13:24.134+00:00"}
---

*we use dimensions to mean quantities from the [SI system](https://www.npl.co.uk/si-units)* 
## quantities

| quantities         | units | dimension |
| ------------------ | ----- | --------- |
| length             | m     | L         |
| mass               | kg    | M         |
| time               | s     | T         |
| temperature        | K     | $\theta$  |
| current            | A     | I         |
| amount             | mol   | n         |
| luminous intensity | Cd    | C, J      |

*luminous intensity is "visual effect of radiation"*
- from these seven, we can derive all others
	- eg:
		- area - $m^2$ - $L^2$
		- density - $kg m^{-3}$ - $M L^{-3}$
		- kinetic energy - $kg m^{2}s^{-2} / joules$ - $M(L T^{-2})$
			- potential energy must be the same
		- charge - $C$ - $IT$ 
- ### homogeneity
	- total energy = kinetic energy + potential energy
	-  $M(L T^{-2}) = M(L T^{-2}) + M(L T^{-2})$
	- all additive terms must have the same dimensions
- ### units of other quantities
#### angles
- using units of radians
	- $\phi = \frac{l}{r} =$ no unit : use radians
	- *"dimension of..."* $= [\phi]$
	- ***angles have no dimensions***
#### trigonometry
- $sin{\phi} = \frac{opp}{hyp}$
	$\frac{[opp]}{[hyp]} = \frac{L}{L} = 1 \implies$  no dimensions
#### exponentials
- $e^x,\;exp(x)$
- $x$ has no dimensions
- eg: radioactive decay:
	- intensity of radiation emitted by a radioisotope 
	$$I(t) = I_0e^{-\lambda t}$$
	$t = time(s), \lambda = decay \; constant (s^{-1})$
	So, $[t \lambda] = TT^{-1} = 1 \implies$ no dimensions
	-> *argument for exponentials and logs has no dimensions*
- eg: natural log: 

$$ln \left(\frac{I}{I_{0}}\right)=-\lambda t$$
might write this as:
$$ln(I) = -\lambda t + ln(I_0)$$
- ideal gas law:  $PV = nRT$
	- to find : dimensions of R
	$[P] = M.L^{-1}T^{-2}$
	$[V]=L^3$
	$[n]=mol$
	$[T]=\theta$
	so, $M.L^2T^{-2}=mol.\theta.[R]$
	$\implies[R]=M.L^2T^{-2}mol^{-1}\theta^{-1}$
	$\therefore[R]=ML^2T^{-2}mol^{-1}\theta^{-1}$

- use homogeneity to show that $sin(x)$ or $exp(x)$ has no dimensions
	- hint: taking series expansions
	$$\sin{x}=x-\frac{x^3}{3!}+\frac{x^5}{5!}-...$$
	- in the RHS, various degrees of x are added.
	- if x had a unit, this would not be possible
	- $\therefore \sin{x}$ has no units 
	$$e^{x}= 1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+...$$
	
	-  in the RHS, various degrees of x are added.
	- if x had a unit, this would not be possible
	- $\therefore e^{x}$ has no units 
## dimensional analysis
- let's be a little more rigorous:
- for our pendulum, we had 4 variables:

| T   | l   | g   | m   | N=4 |
| --- | --- | --- | --- | --- |
| $Q_1$ | $Q_2$ | $Q_3$ | $Q_4$ | -   |
- so we should have set of variables $Q_{1...N}$
	- we also said: $T = f(l,g,m)$
		- we can write: $Q_{1}= f(Q_2,Q_3,Q_4)$
			- if we were interested in g: $Q_3= f(Q_1,Q_2,Q_4)$
- we wrote our answer for the pendulum: 
$$constant = T \sqrt{\frac{g}{l}} = Tg^{\frac{1}{2}}l^{\frac{-1}{2}}$$
- now we can write: 
$$constant = \Pi = Q_1^\alpha Q_2^\beta Q_3^\gamma Q_4^\delta$$
	- *\*$\Pi \neq3.1415...$* but a convention to denote constants
	- dimensions: 
	$$[\Pi] = [Q_1]^\alpha [Q_2]^\beta [Q_3]^\gamma [Q_4]^\delta$$
	- for the pendulum:  
	$$[\Pi] = [T]^\alpha [l]^\beta [g]^\gamma [m]^\delta$$
	$$[\Pi] = T^\alpha L^\beta {(LT^{-2})}^\gamma M^\delta$$
	- LHS is dimensionless $\therefore$ RHS is dimensionless too
	$$= T^\alpha L^\beta L^{\gamma}T^{-2\gamma} M^\delta$$
		- $T$: $0 = \alpha - 2\gamma$
		- $L$: $0 = \beta + \gamma$
		- $M$: $0 = \delta$
		- we have simultaneous equations for the exponents
		- we can choose a value for one of the unknowns:
			let $\alpha = 1$
				$\implies \gamma = \frac{+1}{2}$
				$\implies \beta = \frac{-1}{2}$
				$\implies [\pi] = T^1 L^\frac{-1}{2}{(LT^{-2})}^\frac{1}{2} M^0$
				$\therefore\pi = Tg^{\frac{1}{2}}l^{\frac{-1}{2}} = T \sqrt{\frac{g}{l}}$
			$$[\Pi] = T^\alpha L^\beta {(LT^{-2})}^\gamma M^\delta$$
				- $T$: $0 = \alpha - 2\gamma$
				- $L$: $0 = \beta + \gamma$
				- $M$: $0 = \delta$
			- let $\alpha = 2$
			$\implies \gamma = 1$
			$\implies \beta = -1$
			$\implies [\pi] = T^2 L^{-1}{(LT^{-2})}^1 M^0$
			$\implies [\pi]^\frac{1}{2} = T^1 L^{-\frac{1}{2}}{(LT^{-2})}^\frac{1}{2} M^0$
			$\therefore\sqrt{\pi} = Tg^{\frac{1}{2}}l^{\frac{-1}{2}} = T \sqrt{\frac{g}{l}}$

