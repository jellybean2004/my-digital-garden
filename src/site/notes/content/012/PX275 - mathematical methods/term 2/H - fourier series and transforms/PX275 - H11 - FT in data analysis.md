---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h11-ft-in-data-analysis/","noteIcon":"1","created":"2025-08-27T13:15:23.829+01:00","updated":"2025-02-18T12:38:39.000+00:00"}
---

- discrete set of measurements are dealt with in data analysis, rather than continuous functions
- considering $N$ measurements, $x_i$, obtained at times, $t_i$, where $i \in [1,N]$
$$x_{i}= f(t_i)$$
- defining the **discrete fourier transform (DFT):**
$$DFT = \frac{1}{\sqrt{N}} \sum\limits_{n=1}^{N} x_{n} \exp\left(-2\pi ik \left(\frac{n}{N}\right)\right)$$
- the **fast fourier transform (FFT)** is a more efficient way of achieving this
