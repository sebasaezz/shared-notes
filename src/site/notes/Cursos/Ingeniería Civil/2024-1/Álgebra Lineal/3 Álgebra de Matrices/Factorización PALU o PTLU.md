---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/3-algebra-de-matrices/factorizacion-palu-o-ptlu/","tags":["I2MAT1203"]}
---

# Concepto

Si se tiene una matriz que no se puede factorizar mediante [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/3 Álgebra de Matrices/Factorización LU\|Factorización LU]], entonces se recurre a una matriz permutación para lograr la factorización

# Matriz permutación

> [!definition] Matriz Permutación
> Se define a una matriz permutación $P_{n\times n}$ como una matriz que tiene como orden la permutación (intercambio) de ciertas filas de una matriz.
> e.g.
> $$
> P=\begin{bmatrix}
> 0 & 1 & 0 \\
> 1 & 0 & 0 \\
> 0 & 0 & 1
> \end{bmatrix}
> $$
> Así, en este ejemplo, para una matriz $A_{3\times 3}$ la matriz $PA$ es la matriz $A$ con una permutación de su primera y segunda fila.

## Teorema de inversa

> [!theorem] Inversa y transpuesta de una matriz permutación
> Si $P$ es una matriz permutación, entonces $P^{-1}=P^{T}$

## Factorización $PALU$

> [!definition] Factorización PALU
> Para una matriz $A$, se define la matriz permutación $P$ tal que mediante $PA$ se pueda lograr una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/3 Álgebra de Matrices/Factorización LU#^490a6d\|Factorización LU]], entonces si se tiene $PA=LU$, se logra la factorización:
> $$
> A=P^{T}LU=P^{-1}LU
> $$

# Ejemplo