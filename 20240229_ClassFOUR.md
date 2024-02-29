## Distribución Dirichlet

Sea el vector aleatorio $x = (x_1, ..., x_k)$ que se distribuye Dirichlet con parámetros $\alpha = (\alpha_1, ..., \alpha_k)$, $\alpha_i > 0$, $k > 1$ y $\sum_{i=1}^{k} x_i = 1$, si la densidad es de la forma

$$ f(x|\alpha) = \frac{\Gamma(\alpha_1 + ... + \alpha_k)}{\Gamma(\alpha_1) \cdots \Gamma(\alpha_k)} x_1^{\alpha_1 - 1} \cdots x_k^{\alpha_k - 1} $$

## Distribución Multinomial

Sea el vector aleatorio $X = (x_1, ..., x_k)$ con $x_i$ el número de veces que se da el resultado $k$-ésimo en $N$ sucesos, entonces

$$ P(X_1 = x_1, ..., X_k = x_k) = \frac{N!}{x_1!...x_k!} \theta_1^{x_1}... \theta_k^{x_k} \text{  donde  } \sum_{i=1}^{k} x_i = N $$

Si $x|N, \theta_1, ..., \theta_k$ siguen una distribución multinomial y $(\theta_1, ..., \theta_k)$ siguen una distribución Dirichlet con parámetros $(\alpha_1, ..., \alpha_k)$, $\alpha_i > 0$, entonces para la observación $x = (x_1, ..., x_k)$:

$$\theta | \x_1...x_k \propto \frac{N!}{x_1!...x_k!} \theta_1^{x_1}... \theta_k^{x_k} \frac{\Gamma(\alpha_1 + ... + \alpha_k)}{\Gamma(\alpha_1)...\Gamma(\alpha_k)} \theta_1^{\alpha_1 - 1}... \theta_k^{\alpha_k - 1}$$

$$\propto \theta_1^{x_1 + \alpha_1 - 1}... \theta_k^{x_k + \alpha_k - 1}$$

$$\therefore \theta | x_1 ... x_k \sim \text{Dirichlet con parámetros} (x_1 + \alpha_1, ..., x_k + \alpha_k)$$
