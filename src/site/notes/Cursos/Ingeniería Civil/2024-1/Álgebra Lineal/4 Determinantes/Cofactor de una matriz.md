---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/4-determinantes/cofactor-de-una-matriz/","tags":["I2MAT1203"]}
---

# Concepto

El cofactor en la posición $ij$ ($C_{ij}$) es la determinante de la submatriz $ij$, pero tiene signo designado si su posición es par o impar, es decir, su signo es $(-1)^{i+j}$.

# Definición
$$
C_{ij}=(-1)^{i+j}Det(A_{ij})
$$
## Teorema para cálculo de determinantes

el determinante de una matriz $A$ de $n\times n$, se puede calcular mediante un desarrollo por cofactores a lo largo de cualquier fila o columna. El desarrollo a lo largo de la $i$-ésima fila con los cofactores $C_{ij}$ es:

$$
Det(A)=a_{i1}c_{i1}+a_{i2}c_{i2}+\dots+a_{in}c_{_{in}}:n\in\mathbb{N}
$$

Así, también se puede hacer lo mismo en la $j$-ésima columna:

$$
Det(A)=a_{1j}c_{1j}+a_{2j}c_{2j}+\dots+a_{nj}c_{_{nj}}:n\in\mathbb{N}
$$

Así se obtiene, de forma más formal al definición vista en [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Determinante de una matriz\|Determinante de una matriz]].

## Teorema de matrices triangulares

Si $A$ es una matriz triangular, entonces el determinantes de $A$ es el producto de las entradas sobre la diagonal.

# Ejemplo
