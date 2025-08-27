---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-5-criterios-de-convergencia-raiz-cociente-integral-comparacion/prueba-de-la-razon-para-evaluar-convergencia-de-series/","tags":["I1MAT1620"]}
---


> [!theorem] prueba de la razón (series)
> 1. Si $\lim_{ n \to \infty } \left\lvert  \frac{a_{n+1}}{a_{n}}  \right\rvert=L<1$. Entonces la serie  $\sum a_{n}$ es [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.5 Criterios de convergencia (raíz, cociente, integral, comparación)/Serie absoluta y condicionalmente convergente y propiedades#^357ae8\|absolutamente convergente]] (y por lo tanto converge).
> 2. Si $\lim_{ n \to \infty }  \rvert \frac{a_{n+1}}{a_{n}} \rvert=L>1 \lor \lim_{ n \to \infty }  \rvert \frac{a_{n+1}}{a_{n}} \rvert\to \infty$ entonces la serie $\sum a_{n}$ diverge.
> 3. Si $\lim_{ n \to \infty } \left\lvert  \frac{a_{n+1}}{a_{n}}  \right\rvert=1$ entonces la prueba es inconclusa.
{ #041960}


# Ejemplo

Sea $\sum_{n=1}^{\infty}(-1)^{n} \frac{n^{3}}{3^{n}}$

$$
\left\lvert  \frac{a_{n+1}}{a_{n}}  \right\rvert= \left\lvert  \left( \frac{n+1}{n} \right)^{3} · \frac{1}{3} \right\rvert   
$$

Ahora este límite converge a $\frac{1}{3}<1$, $\therefore$ converge.