---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/intervalos-de-monotonia-y-concavidad-de-una-funcion/","tags":["I3MAT1610"]}
---

# Concepto

Se identifican secciones crecientes y decrecientes de una función

# Definición y usos

> [!definition] Intervalos de monotonía de una función
> Si $f'(x)>0$ sobre $(a,b)$ entonces $f$ es creciente sobre $(a,b)$
> Si $f'(x)<0$ sobre $(a,b)$ entonces $f$ es decreciente sobre $(a,b)$

## Intervalos de monotonía para encontrar máximo y mínimos


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/minimos-y-maximos-de-una-funcion-teorema-de-fermat-teorema-de-valor-extremo-y-puntos-criticos/#0591d8" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] Prueba de la primera derivada
> Suponiendo que $x=c$ es un número crítico de $f$.
> Entonces:
> - $f'$ cambia de positiva a negativa $\implies$ $c$ es máximo local
> - $f'$ cambia de negativa a positiva $\implies$ $c$ es mínimo local
> - $f'$ no cambia se signo, entonces $f$ no tiene máximo o mínimo local en $x=c$

</div></div>
 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/minimos-y-maximos-de-una-funcion-teorema-de-fermat-teorema-de-valor-extremo-y-puntos-criticos/#42ccc9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] Prueba de la segunda derivada
> Si $f(x)$ es una función, y $f''$ es continua cerca de $c$, y $c$ es un valor crítico, entonces:
> - $f'(c)=0$ y $f''(c)>0$, entonces $f$ tiene un mínimo local en $x=c$
> - $f'(c)=0$ y $f''(c)<0$, entonces $f$ tiene un máximo local en $x=c$

</div></div>
 

## Concavidad de una función

Si en un intervalo de una función, todos los puntos del intervalos son mayores a su tangente, entonces la función es cóncava hacia arriba y viceversa.

> [!theorem] Concavidad de una función
> Para una función $f(x)$:
> - $f''(x)>0\forall x \in I \implies f$ es cóncava hacia arriba ($\cup$) en $I$
> - $f''(x)<0\forall x \in I \implies f$ es cóncava hacia abajo ($\cap$) en $I$

### Punto de inflexión

> [!definition] Punto de inflexión
> Se define al punto de inflexión de una función a los puntos donde la función cambia de dirección de concavidad, es decir $f''(x)=0$

# Ejemplo
## Ejemplo 1

Considerando $f(x)=x^3-\frac{9}{2}x^2+6x$

Se define la derivada como $f'(x)=3x^2-9x+6$

Así, para buscar el punto crítico, su busa la derivada en 0, es decir $f'(x)=0$.

$3x^2-9x+6=0$

$x^2-3x-2=0$

$x_{1}=2,x_{2}=1$

Así, estos dos puntos son los máximos y los mínimos de la función.

```desmos-graph
left=-2
right=5
top=10
---
f(x)=x^3-(9/2)x^2+6x
A=(2,f(2))
B=(1,f(1))
```

|         | $f(x)<1$ | $1<f(x)<2$ | $2<f(x)$ |
| ------- | :------: | :--------: | :------: |
| $(x-2)$ |   $-$    |    $-$     |   $+$    |
| $(x-1)$ |   $-$    |    $+$     |   $+$    |
| $f'(x)$ |   $+$    |    $-$     |   $+$    |

Así, se interpreta que la función sube ($+$), despues baja ($-$) y despues sube ($+$), el punto $+\infty$ se puede inferir ya que es el opuesto a el último punto crítico

## Ejemplo 2

para $f(x)=3x^{4}-4x^{3}-12x^{2}+5$

Se tiene $f'(x)=12x^{3}-12x^{2}-24x$

Entonces, se elabora la siguiente tabla de signos:

|         | $(-\infty,-1)$ | $(-1,0)$ | $(0,2)$ | $(2,+\infty)$ |
| ------- |:--------------:|:--------:|:-------:|:-------------:|
| $12x$   |      $-$       |   $-$    |   $+$   |      $+$      |
| $x-2$   |      $-$       |   $-$    |   $-$   |      $+$      |
| $x+1$   |      $-$       |   $+$    |   $+$   |      $+$      |
| $f'(x)$ |      $-$       |   $+$    |   $-$   |      $+$      |

Así, se concluye que la función $f$ es decreciente cuando $x \in (-\infty,-1)\cup(0,2)$ y creciente en $x \in (-\infty,-1)\cup(0,2)$.
