---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-7-series-de-potencias-definicion-intervalo-y-radio-de-convergencia/series-de-potencias/","tags":["I2MAT1620"]}
---

Se tiene una función en al forma:
$$
f(x)=\sum_{n=0}^{\infty} c_{n}x^{n}=c_{0}+c_{1}x^{1}+c_{2}x^{2}\dots
$$
Encontrar los $x$ para los que la serie converge, es equivalente a encontrar $\operatorname{Dom}f$.
Se puede encontrar por medio de la [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.5 Criterios de convergencia (raíz, cociente, integral, comparación)/Prueba de la razón para evaluar convergencia de series\|prueba de la razón]]. Es decir:
$$
\lim_{ n \to \infty } \frac{c_{n+1}x^{n+1}}{c_{n}x^{n}} <1
$$
Los extremos del intervalo encontrado se deben evaluar reemplazando en $x$.
# Series de potiencias centradas en $a$
Cuando se tiene una serie de potencia en la forma:
$$
\sum_{n=0}^{\infty}c_{n}(x-a)^{n}
$$
> [!theorem] teroema de las series de potencias centradas en $a$
> Dada una sere de potencias centrada en $a$, es decir:
>$$
>\sum_{n=0}^{\infty}c_{n}(x-a)^{n}
>$$
> Entonces se cumplirá que la serie (casos):
> 1. Converge a cuando $x=a$
> 2. Converge para toda $x$
> 3. Existe un número $R$ (radio de convergencia) tal que la serie converge si $\lvert x-a \rvert<R$ y divergente si $\lvert x-a \rvert>R$
{ #6f7717}


# Ejemplo