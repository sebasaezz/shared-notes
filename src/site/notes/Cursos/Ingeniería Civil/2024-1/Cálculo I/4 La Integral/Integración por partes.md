---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/integracion-por-partes/","tags":["ExMAT1610","Técnicas-de-integración"]}
---

# Concepto

Se quiere integrar una integral que tiene en el integrando una función $f$ que se puede escribir de la forma $f(x)=u(x)v(x)$ (es una multiplicación de funciones)

# Integración por partes

Considerando la función $f(x)=u(x)v(x)$

Se tendrá:

$$
\begin{align}
 &  & [u(x)v(x)]' & =v(x)u'(x)+v'(x)u(x) &  & \\
 & \implies & \int [u(x)v(x)]' \, dx & =\int v(x)u'(x) \, dx  +\int v'(x)u(x) \, dx  &  &   \\
 & \implies &u(x)v(x) & =\int v(x)u'(x) \, dx+\int v'(x)u(x) \, dx    \\
 &  \implies&\int u(x)v'(x) \, dx  & =u(x)v(x)-\int u(x)v'(x) \, dx  
\end{align}
$$

> [!theorem] integración por partes
> $$
> \int u(x)\underbrace{v'(x) \, dx}_{dv} =u(x)v(x)-\int v(x)\underbrace{u'(x) \, dx}_{du} 
> $$
> pero se tiene que $v'(x)=\frac{d}{dx}v(x)\implies v'(x)dx=dv$
> Y lo mismo para $u'(x)dx$, así se tiene:
> $$
> \int u \, dv=uv-\int v \, du  
> $$
> ¿Cuál es $u$ y cuál es $v$?
> Se cumplirá que el orden de $u$ a $v$ está dado por:
> 1. Funciones inversas
> 2. Logarítmicas
> 3. Polinomios
> 4. Trigonométricas
> 5. Exponenciales

## Demostración
## Integración por partes de una integral definida

Se cumplirá lo siguiente:

$$\int_{a}^{b}\!u(x)v^{\prime}(x)d x=[u(x)v(x)]{\Big\vert}_{a}^{b}-\int_{a}^{b}\!v(x)u^{\prime}(x)d x$$

# Ejemplo
## Ejemplo 1, integral indefinida

Integrando:

$$
\int x^{2}\ln x \, dx 
$$

Primero se busca $u$ y $v$.

Por el orden dicho anteriormente, los logaritmos ($\ln x$) van antes de los polinomios $x^{2}$.

Entonces se define $u(x)=\ln x$ y $v'(x)=x^{2}\implies v(x)=\frac{1}{3}x^{3}$ 

Ahora se tendrá:

$$
\begin{align}
\int x^{2}\ln x \, dx  & =\ln x· \frac{1}{3}x^{3}-\int \frac{1}{3}x^{3}· \frac{1}{x} \, dx \\
 & =\frac{x^{3}}{3}\ln x- \frac{1}{3}\int x^{2} \, dx \\
 & =\frac{x^{3}}{3}\ln x-\frac{1}{3}· \frac{1}{3}x^{3} \\
 & =\frac{x^{3}}{9}\left( 3\ln x-1 \right) 
\end{align} 
$$
## Ejemplo 2, integral definida

Determine:

$$
\int_{0}^{1} \arctan x \, dx 
$$

Utilizando integración por partes.

Se elige $u(x)=\arctan x \implies u'(x)=\frac{1}{1+x^{2}}$

y $v'(x)=1\implies v(x)=1$ (se añadirá la constante al final)

Así:

$$
\begin{align}
\int_{0}^{1} \arctan x·1 \, dx  & =[\arctan (x)x]{\Big\vert}_{0}^{1}-\int_{0}^{1} x· \frac{1}{1+x^{2}}\, dx   \\
\text{Sea}:k & =1+x^{2}\implies dx=\frac{dk}{2x}\\
 & =[\arctan(1)-0]- \frac{1}{2}\int_{1}^{2} \frac{1}{k} \, dk \\
 & =\frac{\pi}{4}- \frac{1}{2}(\ln 2-\ln 1)  \\
 & =\frac{\pi}{4}- \frac{\ln2}{2}
\end{align}
$$
