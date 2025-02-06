---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/l-exchange-symmetry/px-284-l3-distribution-functions/","noteIcon":"1","created":"2025-01-27T10:34:01.282+00:00","updated":"2025-02-06T14:20:59.791+00:00"}
---

- considering a many-particle system with a single state at energy, $E$
- the grand partition function is a sum over all possible configurations of the system:
$$\mathscr Z = \sum\limits_{n} \exp(-n\beta (E - \mu))$$
	where, $n$ is the occupation number, ie. the number of particles in the state, and ${} \mu$ is the chemical potential

- the mean occupation:
$$\langle{n}\rangle = \sum\limits_{n}\frac{ n \exp(-n \beta (E-\mu))}{\mathscr Z} = - \frac{1}{\beta \mathscr Z} \frac{\partial \mathscr Z}{\partial E} = - \frac{1}{\beta} \frac{\partial \ln \mathscr Z}{\partial E}$$

- for fermions: $n = 0$ or $1$ because of pauli's exclusion principle
$$\begin{align*}
\therefore \mathscr Z &= 1 + \exp(-\beta(E-\mu)) \\
\ln \mathscr  Z &= \ln(1 + \exp(-\beta (E - \mu))) \\\\
\langle{n}\rangle &= \frac{\exp(-\beta (E - \mu))}{1 + \exp(-\beta (E - \mu))} \\
&= \frac{1}{\exp(\beta (E - \mu))+1}
\end{align*}$$ 

- for bosons: $n = 0, 1, 2, \dots$
$$\therefore \mathscr Z = \sum\limits_{n=0}^{\infty} \exp(-n \beta (E - \mu))$$
- this is a geometric progression with sum to infinity: 
$$\sum\limits_{0}^{\infty} ar^{n} = \frac{1}{1-r}$$
- so here,
$$\begin{align*}
\mathscr Z &= \frac{1}{1-\exp(-\beta (E - \mu))} \\
\ln \mathscr Z &= -\ln(1-\exp(-\beta (E - \mu))) \\
\langle{n}\rangle &= \frac{\exp(-\beta (E - \mu))}{1-\exp(-\beta (E - \mu))} \\
&= \frac{1}{\exp(\beta (E - \mu))-1}
\end{align*}$$
- these expression can be shown to hold for a particular single-particle state in a general multi-state system

- defining the **distribution function**, $f(E)$, as the mean occupation of a single-particle system $\langle{n}\rangle$ in such a system
- for fermions:
$$f_{FD}(E) = \frac{1}{\exp(\beta (E - \mu))+1}$$
- this is called the **fermi-dirac distribution**, which runs from $0 \to 1$

- for bosons:
$$f_{BE}(E) = \frac{1}{\exp(\beta (E - \mu))-1}$$
- this is called the **bose-einstein distribution**, which runs from $0 \to \infty$

- $f(E)$ can be used to calculate the properties
- number of particles between $E$ and $E + dE$ $= g(E)\,f(E)\,dE$
- so, the total number of particles:
$$N = \int_{0}^{\infty} g(E)\, f(E)\, dE$$
- and, the internal energy:
$$U = \int_{0}^{\infty} E\, g(E)\, f(E)\, dE$$

