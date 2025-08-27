---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/factorizacion-de-cholesky/","tags":["ExMAT1203"]}
---

# Concepto

> "No es más que la continuación de la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/3 Álgebra de Matrices/Factorización LU\|Factorización LU]]"
> -Zegarra

Si $A$ es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas#^da1c7f\|Formas cuadráticas#^da1c7f]], entonces se cumplirá que siempre existirá una matriz $B$ tal que:

$$
A=B^{T}B
$$

Esto ya que $A=PDP^{T}$, todos los valores propios de $A$ son positivos. Entonces si se define a $C=\sqrt{ D }$, (como es diagonal es la matriz diagonal de todos los valores propios )

# Definición

> [!definition] factorización de cholesky
> Sea $A$ una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas#^da1c7f\|matriz positiva definida]], entonces:
> $$
> A=R^{T}R
> $$
> Con $R$ una matriz triangular superior con todas las entradas positivas

# Algoritmo para determinar una factorización

Pivotar la matriz hasta llegar a triangular superior $U_{1}$, sin cambiar filas. Es decir, solo operaciones tipo $F_{i}+kF_{j}=F_{i}$.

Ahora determinar $R$ dividiendo a cada fila de $U_{1}$ por la raiz de su pivote.

## Ejemplo

$$A=\left[{\begin{array}{r r r}{9}&{6}&{-3}\\ {6}&{5}&{-1}\\ {-3}&{-1}&{6}\end{array}}\right]\sim\cdot\cdot\cdot\sim\left[{\begin{array}{r r r}{9}&{6}&{-3}\\ {0}&{1}&{1}\\ {0}&{0}&{4}\end{array}}\right]=U_{1}$$

Ahora dividiendo la primera fila de $U_{1}$ por $\sqrt{ 9 }=3$, la segunda por $\sqrt{ 1 }=1$ y la tercera por $\sqrt{ 4 }=2$:

$$R={\left[\begin{array}{l l l}{3}&{2}&{-1}\\ {0}&{1}&{1}\\ {0}&{0}&{2}\end{array}\right]}$$

Se cumplirá que $R^{T}R=A$
