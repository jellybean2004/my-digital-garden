---
dg-publish: true
---

- sketch he domain, find the equations for the boundaries
- integrate over $y$ considering $x$ constant: 
$$I = \int_{a}^{b}\left( \int_{y_{1}(x)}^{y_{2}(x)} f(x,y).dy \right).dx$$
	- might have to split into two integrals if a boundary cannot be expressed as a single function
- integrate over $x$
- answer can be verified by switching the order of integration: 
$$I = \int_{c}^{d}\left( \int_{x_{1}(y)}^{x_{2}(y)} f(x,y).dx \right).dy$$
