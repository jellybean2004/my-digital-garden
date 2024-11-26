---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-a-dimensional-analysis/px-154-a3-applying-dimensional-analysis/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:49:12.153+00:00"}
---

- two more concepts required:
	- dimensionless groups
	- fundamental independent quantities
## dimensionless groups
- for our pendulum, we had 
$$\Pi = T\sqrt\frac{g}{l}$$
	- $T\sqrt\frac{g}{l}$ is a dimensionless group
- more generally, if we have several variables, we may form more than one dimensionless group
	- instead of $\Pi$, we have $\Pi_1, \Pi_2, \Pi_3,...$
		- for our variables: $Q_1=f(Q_2,Q_3,Q_4,...)$
		- we would write: $\Pi =\phi(\Pi_1,\Pi_2,\Pi_3,...)$
	-  eg: gravity waves on water might need inclusion of depth (L) and wavelength(L)
- the number of dimensionless groups is called $\tilde N$
	- in general, we would need to know $\tilde N$ in order to proceed: it can be determined by "[buckingham's pi method]([[content/011/PX154 - physics foundations/PX154 - A - dimensional analysis/PX154 - A2 - dimensions#^5abdae\|PX154 - A2 - dimensions#^5abdae]])."
	$$\tilde N = N -m$$
			$m =$ number of "fundamental independent quantities"
## fundamental independent quantities
- to find $m$:
	- for our pendulum:

| variables | dimensions |
| --------- | ---------- |
| T         | $T$          |
| l         | $L$          |
| g         | $LT^{-2}$  |
| m         | $M$          |
- 
	-  firstly, $T$ can depend on other variables $\implies$ NOT independent
	- so, discard $T$ and consider remaining variables
		$\implies$ in this example, there is no way to express any of these as a function of the others
	- hence, the number of independent variables is $3$ and so, $m=3$
	- hence, $\tilde N = N-m = 4-3$
			 $\therefore \tilde N = 1$
		- we would stick with $\tilde N$ in an exam
		- check moodle handout for more examples
## the procedure
- 
	- **step 1**: make a list of variables that that we think may be needed
	- **step 2**: use [buckingham's pi method]([[content/011/PX154 - physics foundations/PX154 - A - dimensional analysis/PX154 - A2 - dimensions#^5abdae\|PX154 - A2 - dimensions#^5abdae]]) to determine $\tilde N$
	- **step 3**: consider the exponents of the function that relates them
- eg:
	- speed of waves on water, for deep water:
		- we assume that the depth ($h$) is much greater than the wavelength ($\lambda$)
			- ie: $h >>> \lambda$
		- **step 1**: variables:
			- speed $[V] =LT^{-1}$
			- wavelength $[\lambda] = L$
			- gravity $[g] =LT^{-2}$
			- density $[\rho]=ML^{-3}$
			- we anticipate $v=f(\lambda, g, \rho)$
		- **step 2**: find $\tilde N$
			 $N=4$
			 $m = 3$
			 $\therefore \tilde N = 1$
		- **step 3**: considering the exponents
			- dimensionless group 
				$\Pi = v^{\alpha}g^{\beta}\lambda ^{\gamma} \rho ^{\delta}$
				$[\Pi] = {[LT^{-1}]}^{\alpha}[LT^{-2}]^{\beta}[L] ^{\gamma} [ML^{-3}] ^{\delta}$
			- exponents: 
				$L: 0 = \alpha + \beta + \gamma - 3\delta$
				$T : 0 = -\alpha -2\beta$
				$M:0=-3\delta$
			- taking $\alpha=1$:
				$\beta = -\frac{1}{2}$
				$\delta = 0$
				$\gamma = -1/2$
			- finally,
				$[\Pi] = {[LT^{-1}]}^{1}[LT^{-2}]^{- \frac{1}{2}}[L] ^{- \frac{1}{2}} [ML^{-3}] ^{0}$
				$\implies \Pi =v.g^{- \frac{1}{2}}.\lambda ^{- \frac{1}{2}}$
				$or,\; v= \Pi\sqrt{g\lambda}$
				$\therefore v \propto \sqrt{g\lambda}$
- PDFs on moodle: shallow and intermediate water


 
