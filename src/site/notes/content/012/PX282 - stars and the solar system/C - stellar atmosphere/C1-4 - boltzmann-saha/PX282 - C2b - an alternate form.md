---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-the-solar-system/c-stellar-atmosphere/c1-4-boltzmann-saha/px-282-c2b-an-alternate-form/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-28T18:02:10.790+00:00"}
---

- [[content/012/PX282 - stars and the solar system/C - stellar atmosphere/C1-4 - boltzmann-saha/PX282 - C2a - the boltzmann equation\|the boltzmann equation]] can be written in an alternate form to get $\frac{N_{A}}{N}$ 
- $N$ is the total number of electrons: 
$$N = \sum\limits_{m=1}^{\infty}N_{m}$$
- using the boltzmann equation: 
$$\begin{gather}
	\frac{N_{m}}{N_{1}} = \frac{g_{m}}{g_{1}}\exp\left(- \frac{E_{m}-E_{1}}{k_{B}T}\right) \\
	\implies N = \frac{N_{1}}{g_{1}} \sum\limits_{m=1}^{\infty} g_{m}\exp\left(- \frac{E_{m}-E_{1}}{k_{B}T}\right)
\end{gather}$$
- defining the *partition function*: 
$$U(T) = \sum\limits_{m=1}^{\infty} g_{m}\exp\left(- \frac{E_{m}-E_{1}}{k_{B}T}\right)$$
- therefore, the fraction of electrons in state 1 is: 
$$\begin{gather}
	\implies \frac{N_{1}}{N}= \frac{g_{1}}{U(T)} \\
	\therefore \frac{N_{m}}{N}= \frac{g_{m}}{U(T)}\exp\left(- \frac{E_{m}-E_{1}}{k_{B}T}\right)
\end{gather}$$
	

- eg: what $T$ is needed to get $N_{2}=N_{1}$?
		$\implies \frac{N_{2}}{N_{1}} = 1$
	- known:
		$g_{2}= 8$, $g_{1}=2$
		$E_{1}= -13.6\,eV$, $E_{2} = -3.4\,eV$
	- using the botzmann equation: 
	$$- \frac{E_{1}-E_{2}}{k_{B}T} = ln\left(\frac{g_{1}}{g_{2}}\right)\implies T=85\,300\,K$$
## example
- calculating the temperature to get $N_{2}=N_{1}$
- using the boltzmann equation: 
$$\frac{N_{2}}{N_{1}} = \frac{g_{2}}{g_{1}} \exp\left(- \frac{E_{2}-E_{1}}{k_{B}T}\right) =1$$
- here, $g_{2}=8$ and $g_{1}=2$, and $E_{2}=-3.4\,eV$ and $E_{1}=-13.6\,eV$
- rearranging the equation: 
$$T = \frac{E_{2}-E_{1}}{k_{B}\log(\frac{g_{2}}{g_{1}})} \approx 85300\,K$$
- **balmer lines** require lots of electrons in the $n=2$ state, and they get weaker for $T>\sim9000\,K$ due to ionization
- there exists a 'de-ionized' form of hydrogen, $H^{-}$, with two electrons, which is useful in case of the sun
- $He\,I: 2p\,2n\,2e$ ; $He\,II: 2p\,2n\,1e$