---
dg-publish: true
---

- $1927$, werner heisenberg: if the x-component the momentum of a particle is measured with an uncertainty of $\Delta p_x$, then its x-position cannot, at the same time, be measured more accurately than $\Delta x = \frac{\hbar}{2\Delta p_x}:$  
$$\Delta x\Delta p \geq \frac{\hbar}{2}$$
	- with uncertainties defined in *RMS* sense, ie: $\Delta x = \sqrt{\langle{x^{2}}\rangle - \langle{x}\rangle}^{2}$, where $\langle{A}\rangle=$ average value of $A$
$$\begin{align*}
	\langle{A^{2}}\rangle &= \bar{A^{2}} = \langle{A}\rangle^{2}+\sigma_{A}^{2} \\
	\sigma_{A} &= \sqrt{\langle{A^{2}}\rangle - \langle{A}\rangle^{2}}
\end{align*}$$
- alternatively: 
$$\Delta E \Delta t \geq \frac{\hbar}{2}$$
- from [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C3 - wave packets\|wave packets]] and [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C5 - top-hat distribution\|top-hat distribution]]:
	- if $a(k)$ is sharply peaked, then the wave pulse is relatively broader
	- the width of $a(k)$ curve is inversely proportional to the probability distribution function, $\psi$
	- for a narrow range of $k$, corresponding to a narrow range of momentum, $p$, and a small uncertainty, $\Delta p$, is only possible for a large number of $x$, and therefore larger uncertainty, $\Delta x$

- eg: consider a ball of mass, $\sim200\,g$. measure its position, $\sim\pm 10\,\mu m$
	$\Delta x\Delta p \geq \frac{\hbar}{2}$
	$\Delta p \sim \frac{\hbar}{\Delta x} \sim \frac{10^{-34}}{10^{-5}} \sim 10^{-29}\,kgms^{-2}$ 
	$\Delta v = \frac{\Delta p}{m} \sim \frac{10^{-25}}{0.2} \sim 5\times10^{-29}\,ms^{-1}$

- eg: consider a hydrogen atom
	- using [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - B - atomic stucture/PX156 - B1 - atoms and atomic spectra#bohr's model\|bohr's model]]: $r_{n}=n^{2}a_{0}$
	- taking $n=1:$ 
	$$a_{0} = \frac{\epsilon_{0}h^{2}}{\pi me^{2}} \approx 0.54 \,Å$$
	- electron is localized at the scale of $2a_{0}:$ 
	$$\Delta p \geq \frac{\hbar}{2a_{0}} \sim \frac{\hbar}{a_{0}}$$
	- angular momentum: 
$$\begin{align*}
	L &= mva_{0}=\hbar \\
	|p| &= mv = \frac{\hbar}{a_{0}} 
\end{align*}$$
$$\frac{\Delta p}{|p|} = \frac{\frac{\hbar}{a_{0}}}{\frac{\hbar}{a_{0}}} = 1$$

- eg: showing that it can be shown that an electron is bound in an atom
	- in a 1D region $\sim 0.5\,Å$
	- $\Delta p \sim p \sim \frac{\hbar}{a_{0}} \sim \frac{10^{-34}}{10^{-10}} \sim 10^{-24}\,kgms^{-1}$
	$$KE = \frac{p^{2}}{2m} \sim \frac{(10^{-24})^{2}}{2\times9.11\times10^{-31}} \sim 5\times10^{-19}\,J \approx 3\,eV$$
	- from [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - B - atomic stucture/PX156 - B1 - atoms and atomic spectra#^dc2213\|here]]: rydberg constant $=13.6\,eV$

