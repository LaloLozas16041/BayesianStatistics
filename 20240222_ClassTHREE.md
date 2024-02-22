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

$$ \frac{P(E_2|H,E_1) P(E_1|H)}{P(E_1)} \rightarrow \frac{P(E_2|H,E_1) P(E_1|H)P(H)}{P(E_2|E_1)P(E_1)} = \frac{P(E_2|H,E_1)P(H|E_1)}{P(E_2|E_1)} $$

Así, entonces, se tiene que la distribución posteriori está en términos de la memoria de $E_1$. Para el caso general, si $A$ es $E_1, ..., E_n$ de manera análoga:

$$ P(H|E_1, A) = \frac{P(E_1|H,A)P(H|A)}{P(E_1|A)} $$

Del teorema de Bayes, dado $ H $ es el evento de evaluación ant:

$$ P(A|H,E) = \frac{P(E|H,A)P(H)}{P(E|A)} \approx P(E|H,A)P(H) $$

Para variables aleatorias $Q$ y $X$

$$ P(Q|X) \approx P(X|Q)P(Q) $$
