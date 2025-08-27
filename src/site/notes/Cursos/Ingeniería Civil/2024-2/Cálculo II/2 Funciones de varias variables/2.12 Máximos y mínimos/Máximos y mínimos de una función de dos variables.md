---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-12-maximos-y-minimos/maximos-y-minimos-de-una-funcion-de-dos-variables/","tags":["I3MAT1620"]}
---

# Concepto
# Definición

> [!definition] máximos locales y mínimos locales
> Una función de dos variables $f$ tiene un máximo local en $(a,b)$ si $f(x,y)\leq f(a,b)$ cuando en puntos cercanos (un disco de centro $(a,b)$).
> El mínimo local es lo mismo pero para $f(x,y)\geq f(a,b)$. 

Se hereda el mismo concepto de [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Mínimos y máximos de una función, teorema de Fermat, teorema de valor extremo y puntos críticos\|puntos críticos]] en Cálculo I, pero ahora las derivadas parciales tienen que ser cero.

Si $f$ tiene un máximo local o un mínimo local en $(a,b)$ y las derivadas parciales de primero orden existe, entonces serán cero.

## Prueba de la segunda derivada
Recordando a Cálculo I:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/minimos-y-maximos-de-una-funcion-teorema-de-fermat-teorema-de-valor-extremo-y-puntos-criticos/#42ccc9" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] Prueba de la segunda derivada
> Si $f(x)$ es una función, y $f''$ es continua cerca de $c$, y $c$ es un valor crítico, entonces:
> - $f'(c)=0$ y $f''(c)>0$, entonces $f$ tiene un mínimo local en $x=c$
> - $f'(c)=0$ y $f''(c)<0$, entonces $f$ tiene un máximo local en $x=c$

</div></div>
 


Ahora se debe tomar en consdieración a los signos de una variable $D$ que es el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Determinante de una matriz\|Determinante de una matriz]] formada por las derivadas
> [!theorem] prueba de la segunda derivada en dos variables y punto silla
> Siendo continuas las segundas derivadas de $f$ en una región que encierre al punto $(a,b)$. Y se evalúan en cero. Se tiene lo siguiente:
> $$
> D=\det \begin{bmatrix} f_{xx}(a,b) & f_{xy}(a,b)\\ 
>f_{yx}(a,b) & f_{yy} (a,b)
>
>\end{bmatrix}=D(a,b)=f_{xx}(a,b)f_{yy}(a,b)-[f_{xy}(a,b)]^2 
> $$
> De este valor $D$ se infiere que:
> - Si $D>0$ y $f_{xx}(a,b)>0$: Hay un mínimo local en $(a,b)$.
> - Si $D>0$ y $f_{xx}(a,b)<0$: Hay un máximo local en $(a,b)$.
> - Si $D<0$: no hay un máximo ni un mínimo. Hay un **punto silla**.

- [x] Revisar antes de la prueba  [scheduled:: 2024-12-01]  [due:: 2024-12-02]  [completion:: 2025-03-12]
# Ejemplo