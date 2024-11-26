---
dg-publish: true
---

## conditional probability
- the probability of $A$ happening given that $B$ has happened is written as: $P(A \mid B)$
## joint probability: 
- the probability that $A$ and $B$ both occur if they are independent: 
$$P(A \cap B) = P(A) \cdot P(B)$$
- if they are not independent: 
$$P(A \cap B) = P(A \mid B) \cdot P(B) = P(A \mid B) \cdot P(A)$$
## bayes' theorem
$$P(A\mid B) = \frac{P(B \mid A)\cdot P(A)}{P(B)}$$
### example
- an athlete fails a drugs test which is $95\%$ accurate. what is the likelihood that they are guilty if on average, only $1\%$ of athletes take drugs
- here, $P(D)=0.01$, so, $P(\bar D) = 0.99$
	${} P(+ve \mid D) = 0.95 {}$, 
	$P(+ve \mid \bar D) = 0.05$
	$P(-ve \mid \bar D) = 0.95$
	$P(-ve \mid D) = 0.05$
- using *bayes' theorem*: 
$$P(D \mid +ve) = \frac{{P(+ve \mid D) \, P(D)}}{P(+ve)}$$
$$P(+ve) = P(+ve \mid D) \cdot P(D) + P(+ve \mid \bar D) \cdot P(\bar D) = 0.06$$
$$P(D \mid +ve) = \frac{0.95\times0.01}{0.06} = 0.16$$
