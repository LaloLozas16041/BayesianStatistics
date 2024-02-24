# Proceso de Aprendizaje

## Teorema de Bayes

Siendo los eventos $H$ (Hipótesis) y $E$ (Evidencia), entonces:

$$P(H|E) = \frac{P(E|H)P(H)}{P(E)}$$

El teorema representa un proceso de aprendizaje:

$$P(H) \rightarrow P(H|E) = \frac{P(E|H)P(H)}{P(E)}$$

donde:

- $P(H)$: Probabilidad A priori
- $P(H|E)$: Probabilidad Posteriori
- $P(E)$: Predictiva
- $P(E|H)$: Verosimilitud

El teorema de Bayes tiene la propiedad de memoria que para dos eventos $E_1$ y $E_2$, entonces:

$$P(H|E_1,E_2) = \frac{P(E_2,E_1|H)P(H)}{P(E_2,E_1)} = \frac{P(E_2|H,E_1)P(E_1|H)P(H)}{P(E_2|E_1)P(E_1)} $$

$$ = \frac{P(E_2|H,E_1)P(H|E_1)}{P(E_2|E_1)} $$

Así, entonces, se tiene que la distribución posteriori está en términos de la memoria de $E_1$. Para el caso general, si $A$ es $E_1, ..., E_n$ de manera análoga:

$$ P(H|E_n, A) = \frac{P(E_1|H,A)P(H|A)}{P(E_n|A)} $$

Del teorema de Bayes, dado que $H$ es el evento de evaluación, entonces:

$$ P(H|E) = \frac{P(E|H)P(H)}{P(E)} \propto P(E|H)P(H) $$

Para variables aleatorias $\theta$ y $X$

$$ P(\theta|X) \propto P(X|\theta)P(\theta) $$

Por lo que para $P(\theta|X) = k P(X|\theta)P(\theta)$, donde $k \in R$ es tal que:

$$\int_{\Theta} k P(X|\Theta)P(\Theta)d\Theta = 1$$

ó

$$\sum_{i \in J} k P(X|\Theta_i)P(\Theta_i)d\Theta = 1$$

Ejemplo: Si $X|\theta \sim \text{Bernoulli}(\theta)$, $\theta \sim \text{Beta}(\alpha, \beta)$, entonces:

$$P(\theta|X) \propto P(X|\theta)P(\theta) \propto \theta^X(1-\theta)^{1-X} \frac{\Gamma(\alpha + \beta)}{\Gamma(\alpha)\Gamma(\beta)} \theta^{\alpha-1}(1-\theta)^{\beta-1}$$

$$\propto \theta^{X+\alpha-1}(1-\theta)^{\beta-X+\beta-1}$$

$$\therefore \theta|X \sim \text{Beta}(X+\alpha, \beta-X+\beta)$$

## Distribución Dirichlet

## Distribución Multinomial
