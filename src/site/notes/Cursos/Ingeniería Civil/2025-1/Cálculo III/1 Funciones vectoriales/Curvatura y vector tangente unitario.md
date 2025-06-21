---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/curvatura-y-vector-tangente-unitario/","tags":["I1MAT1630"]}
---

El vector tangente unitario de se define como:
$$
\frac{\vec{r}'(t)}{\lvert \lvert \vec{r}'(t) \rvert \rvert }
$$
Pero si se tiene una [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Cambio de variable por longitud de arco de una curva paramétrica\|normalización de una curva paramétrica]] dada por $\vec{r}(s)$, ya se sabe que su rapidez siempre será $1$, es decir:
$$
T(s)=\vec{r}'(s)
$$
Si la parametrización es en términos de longitud de arco $T(s)$ y podemos calcular:
$$
\kappa=\left\lvert  \left\lvert  \frac{d}{ds}T(s)   \right\rvert  \right\rvert 
$$
$\kappa$ es la **curvatura** de de la curva paramétrica. Observe que, como $\frac{ ds }{ dt }=\lvert \lvert \vec{r}'(t) \rvert \rvert$:
$$
\frac{ dT }{ dt } =\frac{ dT }{ ds } \frac{ ds }{ dt } =\frac{ dT }{ ds } \lvert \lvert \vec{r}'(s) \rvert \rvert \implies \kappa=\left\lvert  \left\lvert  \frac{T'(t)}{\lvert \lvert \vec{r}'(s) \rvert \rvert }  \right\rvert  \right\rvert 
$$
Nuevamente, si se tiene una normalización de la curva paramétrica, se va a simplificar como:
$$
\frac{ dT }{ ds } =\lvert \lvert \vec{r}''(s) \rvert \rvert =\kappa
$$

> [!theorem]
> $$
> \kappa=\frac{\lvert \lvert \vec{r}' \times \vec{r}'' \rvert \rvert }{\lvert \lvert \vec{r}' \rvert \rvert ^{3}}
> $$

Si es que se tiene una curva dada por $y=f(x)$, entonces se puede parametrizar como $\vec{r}=\langle x,f(x) \rangle$ y se obtiene que:
$$
\kappa=\frac{\lvert f''(x) \rvert }{(1+(f'(x))^{2})^{3/2}}
$$
