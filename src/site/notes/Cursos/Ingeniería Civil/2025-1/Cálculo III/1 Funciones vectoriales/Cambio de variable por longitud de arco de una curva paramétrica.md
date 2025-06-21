---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/cambio-de-variable-por-longitud-de-arco-de-una-curva-parametrica/","tags":["I1MAT1630"]}
---

# Concepto
Una curva paramétrica en función de $t$, puede ser caracterizada por medio de la distancia que ha recorrido hasta $t$. Es decir, cada punto en la curva es identificable por medio de la longitud de arco hasta ese punto.
Entonces se puede dar una forma explícita para el valor de $t$ desde una distancia inicial.
Para cada $s$ se puede decir e $t$ que corresponde a esa longitud de arco, entonces se puede expresar $t$ es términos de $s$.
# Definición
Para una función vectorial $\vec{r}(t)$, se podrá encontrar la equivalencia:
$$
t=t(s)
$$
Entonces se va a poder hacer el cambio de variable:
$$
\vec{r}(t(s))
$$
Esta parametrización se conoce como "parametrización con respecto a la longitud de arco".
Esta parametrización se puede interpretar como un cambio de velocidad, donde la rapidez ($\lvert \lvert \vec{r}'(s) \rvert \rvert$) siempre sea $1$.

# Ejemplo
La hélice $\vec{r}(t)=\langle \sin t , \cos t, t\rangle$ cumple que $s(t)=\sqrt{ 2 }t$.
$$
\implies t=\frac{s}{\sqrt{ 2 }}
$$
Ahora se tendrá que la hélice es equivalente a:
$$
\vec{r}(s)=\left\langle  \sin \frac{s}{\sqrt{ 2 }}, \cos \frac{s}{\sqrt{ 2 }}, \frac{s}{\sqrt{ 2 }}  \right\rangle 
$$
