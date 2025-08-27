---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-9-serie-de-taylor/serie-de-taylor/","tags":["I2MAT1620"]}
---

# Concepto
Representar una función cualquiera
# Definición
Si $f(x)$ se escribe como series de [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.7 Series de potencias. Definición. Intervalo y radio de convergencia/Series de potencias\|Series de potencias]] centrada en un punto $x=a$, con radio de convergencia $R$, entonces se podrá escribir como:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-7-series-de-potencias-definicion-intervalo-y-radio-de-convergencia/series-de-potencias/#6f7717" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] teroema de las series de potencias centradas en $a$
> Dada una sere de potencias centrada en $a$, es decir:
>$
>\sum_{n=0}^{\infty}c_{n}(x-a)^{n}
>$
> Entonces se cumplirá que la serie (casos):
> 1. Converge a cuando $x=a$
> 2. Converge para toda $x$
> 3. Existe un número $R$ (radio de convergencia) tal que la serie converge si $\lvert x-a \rvert<R$ y divergente si $\lvert x-a \rvert>R$

</div></div>
 
## Derivando y evaluando en $a$
$$
\begin{align}
f(x) &= c_{0}+c_{1}(x-a)+c_{2}(x-a)^{2}\dots \\
f'(x)  & =c_{1}+2c_{2}(x-a)+3c_{3}(x-a)^{2}+\dots+nc_{n}(x-a)^{n-1} \\
f''(x)  & =2c_{2}+2·3c_{3}(x-a)^{}+\dots+n(n-1)c_{n}(x-a)^{n-2} \\
f'''(x)  & =2·3c_{3}+2·3·4c_{4}(x-a)+\dots+n(n-1)(n-2)c_{n}(x-a)^{n-3}
 \\
f^{(n)}(a) & =n!c_{n} \\
\implies c_{n} & = \frac{f^{(n)}(a)}{n!}
\end{align}
$$
Ahora, volviendo a la función anterior, y considerando al punto $a$ como un punto que se elige para aproximar.
$$
f(x)=f(a)+f'(a)(x-a)+\frac{f''(a)}{2!}(x-a)^{2}+\frac{f'''(a)}{3!}(x-a)^{3}+\dots+\frac{f^{(n)}}{n!}(x-a)^{n}$$
Este es el polinomio de Taylor. Ahora, se podrá definir una serie:
> [!definition] Serie de Taylor y serie Maclaurin.
>  $$
> f(x)=\sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!}(x-a)^{n}
> $$
> Esta es la serie de Taylor centrada en $a$. Ahora, si se centra en $0$ se tendrá la serie de Maclauryn.



# Error
Se tendrá que $f(x)=T_{n}(x)+R_{n}(x)$.


Desigualdad de Taylor:
$$
\left\lvert  R_{n}(x) \right\rvert \leq \frac{M}{(n+1)!}\lvert x-1 \rvert^{a+1}:\lvert x-a |\rvert\leq d  
$$


`\begin{proof}`
[[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.3 Sucesiones monótonas y acotadas/Desmotración por inducción\|Desmotración por inducción]]:
Para $n=1$
Si $\lvert f''(x) \rvert \leq M$ para $\lvert x-a \rvert \leq d$
entonces: $\lvert R_{1}(x) \rvert \leq \frac{M}{2!}(x-a)^{2}$.

Gráficamente, se debe pensar a $d$ como una distancia que es mayor a la distancia que hay entre $x$ y $a$.
Ya se tiene que  $\lvert f''(x) \rvert \leq M$, en otras palabras, $-M \leq f''(x) \leq M$.
Ahora:
$$
\int_{a}^{x} -M \, dt \leq \int_{a}^{x} f''(x) \, dt |\leq \int_{a}^{x} M \, dt  
$$
Aplicando el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Teorema fundamental del cálculo (TFC) y propiedades\|TFC]]:
$$
-M(x-a) \leq f'(x)-f'(a)\leq M(x-a)
$$
$$
-M(x-a)+f'(a) \leq f'(x) \leq M(x-a)+ f'(x)
$$
$$
\int_{a}^{x} -M(x-a)+f'(a) \, dt  \leq \int_{a}^{x} f'(x) \, dt  \leq \int_{a}^{x} M(x-a)+ f'(x) \, dt 
$$
Integrando:
- [x] terminar  [completion:: 2025-04-20]


`\end{proof}`


# Ejemplo
## Ejemplo 1
Un ejemplo clásico de la serie de Taylor es la representación de la función exponencial $e^x$ alrededor del punto $a=0$ (es decir, una serie de Maclaurin):

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \cdots
$$

Esta serie converge para todo valor real de $x$, por lo que puede usarse para calcular el valor de $e^x$ con cualquier precisión deseada. 

Ahora para acotar el error:
Se tendrá $\lvert x \rvert \leq d \implies \lvert e^{x} \rvert \leq e^{d} \implies \lvert R_{n} \rvert \leq \frac{e^{d}}{(n+1)!}x^{n+1}$
Ahora, para demostrar la convergencia de la serie, se debe demostrar que el error tiende a $0$ en tanto que $n$ tiende a infinito:
$$
\lim_{ n \to \infty } \frac{e^{d} x^{n+1}}{(n+1)!}=0
$$
$$
 
$$
## Ejemplo 2
Otro ejemplo clásico es la representación de la función seno $\sin(x)$ también alrededor del punto $a=0$:

$$
\sin(x) = \sum_{n=0}^\infty (-1)^n\frac{x^{2n+1}}{(2n+1)!} = x - \frac{x^3}{3!} + \frac{x^5}{5!}-\frac{x^7}{7!}+\cdots
$$

Esta serie también converge para todo valor real de $x$.