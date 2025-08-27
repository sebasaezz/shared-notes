---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-14-maximos-y-minimos-para-regiones-acotadas/minimos-y-maximos-para-regiones-acotadas-en-funciones-de-varias-variables/","tags":["I3MAT1620"]}
---

# Concepto
# Definición
## Teorema de valor extremo
Se asemeja al teorema de valor extremo visto en Cálculo I.

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/minimos-y-maximos-de-una-funcion-teorema-de-fermat-teorema-de-valor-extremo-y-puntos-criticos/#ff8c4a" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] Teorema de valor extremo
> Si $f$ es continua en $[a,b]$ entonces tienen que existir $c$ y $d$ en tal intervalo, tales que $f(c)$ es el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Mínimos y máximos de una función, teorema de Fermat, teorema de valor extremo y puntos críticos\|máximo global]] y $f(d)$ el mínimo global.
> Este teorema requiere de las siguientes hipótesis:
> - Que $f$ sea continua en el intervalo $[a,b]$
> - Que es mínimo o un [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Mínimos y máximos de una función, teorema de Fermat, teorema de valor extremo y puntos críticos\|máximo local]] en $c$ y $f'(c)$ existe, entonces $f'(c)=0$. En otras palabras, $f'(c)$ es un punto crítico de $f$.

</div></div>
 


> [!theorem] Teorema de valor extremos para dos variables
> Si $f$ es continua sobre un conjunto de $\mathbb{R}^{2}$ $D$, cerrado y acotado. $f$ alcanza un valor máximo absoluto $f(x_{1},y_{1})$ y un valor mínimo $f(x_{2},y_{2})$ en algunos puntos $(x_{1},y_{1})$ y $(x_{2},y_{2})$ en $D$.

## Puntos en la frontera
Para un conjunto cerrado, los máximos y mínimos pueden estar en la frontera.
# Ejemplo 
Determinar los valores máximos y mínimos absolutos de:
$$
f(x,y)=x^{2}-2xy+2y
$$
En $D=\{ (x,y):0\leq x\leq 3 \land 0\leq y\leq 2 \}$
Este intervalo se interpreta como un rectángulo en $\mathbb{R}^{2}$.
**Primero se analizan los puntos críticos.**
Se sabe que $(1,1)$ es un punto crítico. 

**Análisis de frontera**
Para $x=0$, se tienen los puntos $(0,y):0\leq y\leq 2$
Se sabe que $f(0,y)=2y:0\leq y\leq 2$
Se define una función análoga de una variables $g(y)=2y\implies g'(y)=2$.
$g$ alcanza su máximo para $y=2$.

<iframe width='500' height='500' src='https://www.wolframcloud.com/obj/179f263f-9099-451a-b37b-7b1550674c5d' frameborder='0'></iframe>