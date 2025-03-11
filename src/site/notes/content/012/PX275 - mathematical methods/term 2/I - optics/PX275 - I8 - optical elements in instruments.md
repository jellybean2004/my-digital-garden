---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i8-optical-elements-in-instruments/","noteIcon":"1","created":"2025-03-11T12:20:46.643+00:00","updated":"2025-03-11T12:42:08.040+00:00"}
---

- considering an optical bench, which involves a number of optical elements past aperture, before detection
- each active optical element will affect the light paths, and therefore, the image formation at the detector
- the result is the convolution of successive convolutions
- optic systems modelling is equal to convolutions
$$\mathcal F (f*g(x)) = \tilde f\, \tilde g$$
- the eventual result is source $* \text{psf}(x)$ , which is the point spread function
- this function can be very complex due to many optical elements in the light path
- the output will be the input $* \text{psf}+$noise

- **image deconvolving/deconvolution** involves working backwards from the observed image to obtain the source
- the observed image has finite resolution and signal to noise may contain artefacts and imperfections
- therefore, it can be done, but with limitations
