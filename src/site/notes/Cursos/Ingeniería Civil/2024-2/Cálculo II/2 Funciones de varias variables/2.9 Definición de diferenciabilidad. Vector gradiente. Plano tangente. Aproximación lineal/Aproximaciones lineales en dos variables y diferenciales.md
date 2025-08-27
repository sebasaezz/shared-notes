---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-9-definicion-de-diferenciabilidad-vector-gradiente-plano-tangente-aproximacion-lineal/aproximaciones-lineales-en-dos-variables-y-diferenciales/","tags":["I3MAT1620"]}
---

# Concepto
Lo mismo de [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Aproximaciones lineales y diferenciales\|Aproximaciones lineales y diferenciales]] pero con planos.
# Definición

## Aproximación
Se se define un plano en $(a,b)$ como:
$$
P(x,y)=f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)+f(a,b)
$$
se cumplirá que:
$$
P(x,y) \approx f(x,y) :\text{para } (x,y) \text{ cercanos a }(a,b)
$$
# Diferenciales
Muy similar a lo visto en [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Aproximaciones lineales y diferenciales\|Aproximaciones lineales y diferenciales]], se tiene que:
$$
dz=f_{x}dx+f_{y}dy
$$
De aquí, si se elije una aproximación con $\Delta x=(x-a)$ y $\Delta y=(y-b)$, la aproximación estará dada por:
$$
f(x,y)=f(a,b)+dz:dz=f_{x}(x-a)+f_{y}(y-b)
$$
# Ejemplo
## Ejemplo 1
a) Si $z = f (x, y) = x^2 + 3xy - y^2$, determine la diferencial $dz$. 
Dado lo dicho anteriormente, la diferencia $dz$ estará dada simplemente por:
$$
dz=(2x+3y)dx+(3x-2y)dy
$$


b) Si x cambia de $2$ a $2.05$ y $y$ pasa de $3$ a $2.96$, compare los valores de $\Delta z$ y $dz$.
El enunciado dice que se está haciendo una aproximación en $(x,y)=(2.05,2.96)$ con puntos base $(a,b)=(2,3)$, de aquí que:
$$
\begin{align}
dx & =\Delta x=x-a=2.05-2=0.05 \\
dy & =\Delta y=y-b= 2.96-3=0.04
\end{align}
$$
De aquí que:
$$
dz=(2·2+3·3)·0.05+(3·2-2·3)·0.04=0.65
$$
Mientras que el valor de $\Delta z$ es:
$$
\Delta z=z-f(a,b)=f(2,3)-f(2.05,2.96)=13-13.6449=-0.6449
$$
