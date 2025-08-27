---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-5-criterios-de-convergencia-raiz-cociente-integral-comparacion/criterios-para-convergencia-de-una-serie/","tags":["I1MAT1620"]}
---

## Criterio por límite interior

> [!theorem] prueba de la divergencia (de una serie calculando límite interior)
> Si la serie $\sum_{n=1}^{\infty}a_{n}$ es convergente, entonces $\lim_{ n \to \infty } a_{{n}}=0$
> Así también, si $\lim_{ n \to \infty } a_{n}$ diverge o es $\neq 0$, entonces $\sum_{n=1}^{\infty}a_{n}$ diverge.
{ #6bb31a}


`\begin{proof}`

Por intuición, se debe evaluar como que la única forma de que una suma sea convergente es que lo que se le sume sea cada vez menor.

Sea $\sum_{n=1}^{\infty}a_{n}=\lim_{ n \to \infty } s_{n}=L$ convergente

$L=\lim_{ n \to \infty } s_{n+1}$

Ahora se debe cumplir que:

$s_{n+1}-s_{n}=a_{n+1}$

Aplicando el límite:

$\lim_{ n \to \infty } s_{n+1}-s_{n}=\lim_{ n \to \infty } a_{n+1}=\lim_{ n \to \infty } a_{n}$

$L-L=\lim_{ n \to \infty } a_{n}=0$

`\end{proof}`

## Criterio por integrales

> [!theorem] prueba de la integral
> Sea $f$ una función positiva, continua y decreciente sobre $[1,\infty)$, entonces se cumplirá que:
> 1. $\int_{1}^{\infty} f(x) \, dx$ converge $\implies \sum_{n=1}^{\infty}a_{n}$ converge.
> 2. $\int_{1}^{\infty} f(x) \, dx$ diverge $\implies \sum_{n=1}^{\infty}a_{n}$ diverge.
> 
> Se puede considerar como una [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Suma de Riemann\|Suma de Riemann]].
{ #0a37f4}


### Estimación del error o residuo para el criterio de integrales

> [!theorem] estimación del error de una para la prueba de integral
> Considerando la suma:
> $$
> S=\sum_{i=1}^{\infty}a_{i}=\underbrace{ a_{1}+a_{2}+\dots+a_{n} }_{ S_{n} }+\underbrace{ a_{n+1}+a_{n+2}+\dots }_{ \text{error}=R_{n} }
> $$
> Si se considera la suma hasta el término $n$, $\sum_{i=1}^{n}a_{i}$, entonces el error será lo que queda y se cumplirá que:
> $$
> \int_{n+1}^{\infty} f(x) \, dx \leq R_{n}\leq \int_{n}^{\infty} f(x) \, dx 
> $$
> Con
> $$R_{n}=\lvert S-S_{n} \rvert $$
{ #c4ad6c}


## Convergencia al límite

Se cumple un teorema muy similar al siguiente:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-1-integrales-impropias-criterios-de-comparacion/teorema-de-comparacion-y-teorema-de-comparacion-al-limite/#8e05c2" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] test de comparación al límite
> Sea $f$ y $g$ funciones continuas y positivas en $(a,\infty)$:
> Dado que $\lim_{ x \to \infty } \frac{f(x)}{g(x)}=P$, Se cumplirá que:
> - Si $P>0$, entonces se cumple que $\int_{a}^{\infty} g(x) \, dx$ converge o diverge $\iff \int_{a}^{\infty} g(x) \, dx$ converge o diverge. 
> - Si $P=0$, entonces se cumple que $\int_{a}^{\infty} g(x) \, dx$ converge $\implies \int_{a}^{\infty} f(x) \, dx$ converge.
> - Si $P \to \infty$, entonces se cumple que si $\int_{a}^{\infty} g(x) \, dx$ diverge $\implies$ $\int_{a}^{\infty} f(x) \, dx$ diverge.
> 
> Lo mismo se cumple para [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.4 Series. Definición de sumas parciales. Convergencia de series. Convergencia absoluta/Series y sumas parciales\|Series y sumas parciales]]

</div></div>
 


# Criterio $P$

Se cumple de la misma forma que con integrales, desde $1$ hasta $\infty$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-1-integrales-impropias-criterios-de-comparacion/criterio-p/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




> [!theorem]
> Dada la integral el la forma $\int \frac{1}{x^{p}} \, dx$, se cumplirán las siguiente propiedades de [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.1 Integrales impropias. Criterios de comparación/Convergencia o divergencia de una integral\|Convergencia o divergencia de una integral]].
> 
> $
> \int_{0}^{1} \frac{1}{x^{P}} \, dx \begin{cases}
> P\geq1\implies \text{diverge} \\
> P<1\implies \text{converge}
> \end{cases}
> $
> $
> \int_{1}^{\infty} \frac{1}{x^{P}} \, dx \implies \begin{cases}
> P>1\implies \text{converge} \\
> P\leq 1 \implies \text{diverge}
> \end{cases}
> $
> 
> Además, este criterio se cumplirá de la misma forma para [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.4 Series. Definición de sumas parciales. Convergencia de series. Convergencia absoluta/Series y sumas parciales\|Series y sumas parciales]] de la forma $\sum_{n=1}^{\infty} \frac{1}{n ^{P}}$




</div></div>


# Ejemplo
## Ejemplo 1

$\sum_{n=1}^{\infty} \frac{\ln x}{n}$, converge o diverge????¿?¿?¿?=?¿¿?¿??¿??¿?¿?¿?¿

Sea $f(x)=\frac{\ln x}{n}$, se evalurarán las primeras hipótesis del teorema de [[#^0a37f4]] .

- $f(x)$ es continua ya que está hecha de funciones continuas en $[1,\infty)$
Para evaluar crecimiento, se considera la derivada $f'(x)= \frac{1-\ln x}{x^{2}}$.
$$
\begin{align}
\frac{1-\ln x}{x^{2}} & <0 \\
1-\ln x& <0 \\
1& <\ln x \\
e& <x
\end{align}
$$
- $f(x)$ es siempre positiva
Ahora se integra por partes:
$$
\begin{align}
\int_{1}^{\infty} \frac{\ln x}{x} \, dx 
\end{align}
$$

diverge (pura algebrita)

## Ejemplo 2

Estimar el error de la siguiente suma:

$$
\sum_{n=1}^{10} \frac{1}{n ^{3}}
$$
$$
R_{10}=\sum_{n=1}^{\infty} \left[\frac{1}{n ^{3}}\right]-\sum_{n=1}^{10} \frac{1}{n ^{3}}
$$

Por el teorema de  [[#^c4ad6c]], se cumplirá que:

$$
\int_{11}^{\infty} \frac{1}{x^{3}} \, dx \leq R_{10} \leq \int_{10}^{\infty} \frac{1}{x^{3}} \, dx 
$$

- [x] revisar error por integral para examen  [priority:: high]  [scheduled:: 2024-12-01]  [completion:: 2025-03-16]
Ahora se calcula:

$$
\lim_{ t \to \infty } \left[ -\frac{1}{2x^{2}} \right]_{11}^{t}=\frac{1}{2·11^{2}}= \frac{1}{242} \approx0.0041322
$$
$$
\lim_{ t \to \infty } \left[ -\frac{1}{2x^{2}} \right]_{10}^{t}=\frac{1}{2·10^{2}}= \frac{1}{200} =0.005
$$

También se puede calcular la sumatoria:

$$
\sum_{n=1}^{10} \frac{1}{n^{3}}\approx 1.1975
$$

Así, por el teorema se puede concluir que la diferencia entre esta suma, y su serie se encuentra en el intervalo $[0.0041322;0.005]$.

Así, el valor real de la serie debe rondar en el intervalo $| 1.2016; 1.2025|$.

El valor real de la serie es de $\approx1.20206$, cosa que cumple con el intervalo.