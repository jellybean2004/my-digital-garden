---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-b-particle-physics/px-156-k-accelerators-and-detectors/px-156-k5-detectors/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T20:06:34.359+00:00"}
---

- collider detectors are onion-like with different types of sub detectors with different types of subdetectors doing different things to 'reconstruct' particles coming from a collision
## tracker 
- detects and tracks charged particles close to the interaction point
- many type of trackers
- all are built in layers around the beam pipe to trace particles coming out

![Pasted image 20240515122943.png](/img/user/pics/Pasted%20image%2020240515122943.png)

## calorimeter
- energy measurement
### electromagnetic calorimeter (ECAL) 
- measures electron and photon energies from how they move through material
- electrons: in a field of an atom in a material, it scatters, radiating in a photon
- photons: pair-production
- in a detector, an electromagnetic shower of $e^{-}/e^{+}/\gamma$ is created
- $\gamma$ can be detected in light detectors
### hadronic calorimeters (HCAL)
- same thing a ECAL for hadrons
- instead of just $e^{-}/e^{+}/\gamma$, there are also other hadrons in the shower

## probability of survival 
- calorimeters are designed around specific length scales that define the shower development
- EM showers: probability that an electron or photon survives to a distance, $x$, inside a material as: 
$$P_{e}(x) = \exp\left(- \frac{x}{x_{0}}\right)$$
	where, $x_{0}=$ reiteration length, property of a material 
- hadronic showers: probability of a hadron to survive a distance, $x$, inside a material as: 
$$P_{h}(x) = \exp\left(- \frac{x}{\lambda_{I}}\right)$$
	where, $\lambda_{x}=$ 'nuclear reiteration length', material dependent

| material | $x_{0}(cm)$ | $\lambda_{I}(cm)$ |
| :------: | :---------: | :---------------: |
|  water   |    $3.6$    |       $83$        |
|   iron   |    $1.8$    |       $17$        |
|   lead   |    $0.5$    |       $17$        |
