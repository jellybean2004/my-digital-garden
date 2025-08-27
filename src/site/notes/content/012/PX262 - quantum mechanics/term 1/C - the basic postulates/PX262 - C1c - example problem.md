---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/c-the-basic-postulates/px-262-c1c-example-problem/","noteIcon":"1","created":"2025-08-27T13:14:15.822+01:00","updated":"2024-11-26T01:07:04.000+00:00"}
---

- **consider a quantum harmonic oscillator in the ground state to calculate probability of finding the particle displaced beyond its classical limit**

- working out the classical limit: 
$$\begin{gather}
\frac{1}{2}M\omega^{2} x_{max}^{2} = E_{0}= \frac{1}{2}\hbar \omega \\
x_{max}= \sqrt{\frac{\hbar}{M\omega}} = x_{0}
\end{gather}$$
- the probability of the oscillator being beyond $|x_{0}|:$ 
  $$P = \int_{-\infty}^{x_{0}} |\phi_{0}(x)|^{2}\,dx + \int_{x_{0}}^{\infty} |\phi_{0}|^{2}\,dx$$
- the wavefunction: 
  $$\phi_{0}= \left(\frac{M\omega}{\hbar\pi}\right)^{\frac{1}{4}} \exp\left(- \frac{M\omega x^{2}}{2\hbar}\right) = \left(\frac{1}{\pi x_{0}}\right)^{\frac{1}{2}} \exp\left(- \frac{x^{2}}{2x_{0}^{2}}\right)$$
- let $t = \frac{x}{x_{0}} \implies dt = \frac{dx}{x_{0}}:$ 
  $$P = 2 \int_{1}^{\infty} \frac{1}{\sqrt{\pi}} e^{-t^{2}} \,dt = 0.045$$
- using $\int_{1}^{\infty} e^{-x^{2}} \,dx \simeq 0.16\sqrt{2\pi}$
