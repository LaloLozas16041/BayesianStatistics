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

$$ P(Q|X) \propto P(X|Q)P(Q) $$

Por lo que para $P(\theta|X) = k P(X|\theta)P(\theta)$, donde $k \in R$ es tal que:

$\int_{\Theta} k P(X|\Theta)P(\Theta)d\Theta = 1$ ó $\sum_{i \in J} k P(X|\Theta_i)P(\Theta_i)d\Theta = 1$

Ejemplo: Si $X \sim \text{Beta}(\alpha, \beta)$, entonces

$P(Q|X) \text{ o } P(X|Q)P(Q) \text{ es } \alpha^{x}\beta^{(1-x)}\frac{f(x)}{f(x|\alpha,\beta)} $

$\alpha^{x}\beta^{(1-x)} * \alpha^{*\alpha-1}\beta^{*\beta-1} $

$\therefore Q|X \sim \text{Beta}(x+\alpha, \beta+x^*) $

## Distribución Dirichlet

Sea el vector aleatorio $x = (x_1, ..., x_k) $se distribuye Dirichlet con parámetros $\alpha = (\alpha_1, ..., \alpha_k) $, $x > 0 $, $k > 1 $, $\sum x_i = 1 $, si la densidad es de la forma

$f(x|\alpha) = \frac{\Gamma(\alpha_1 + ... + \alpha_k)}{\Gamma(\alpha_1)...\Gamma(\alpha_k)}x_1^{\alpha_1-1}...x_k^{\alpha_k-1} $

## Distribución Multinomial

Sea el vector aleatorio $r = (x_1, ..., x_k) $con $x $es el número de veces que da el resultado $k $-ésimo en $n $sucesos, entonces

$P(x_1, ..., x_k|n) = \frac{n!}{x_1!...x_k!}\alpha_1^{x_1}... \alpha_k^{x_k} \text{, }\sum_{i} \alpha_i = 1, \sum_{i} x_i = n $

Si $x_i \sim $Multinomial y $(\alpha_1, ..., \alpha_k) \sim $Dirichlet con parámetros $(\alpha_1, ..., \alpha_k) $, entonces la observación $x = (x_1, ..., x_k)$

$P(x|\alpha) = \frac{n!}{x_1!...x_k!}\alpha_1^{x_1}... \alpha_k^{x_k} \frac{\Gamma(\alpha_1 + ... + \alpha_k)}{\Gamma(\alpha_1)...\Gamma(\alpha_k)} $

$\alpha_1^{x_1+\alpha_1-1}... \alpha_k^{x_k+\alpha_k-1} $

$\therefore \alpha_1:x_1, ..., \alpha_k:x_k \sim \text{Dirichlet con parámetros} (x_1+\alpha_1, ..., x_k+\alpha_k) $

