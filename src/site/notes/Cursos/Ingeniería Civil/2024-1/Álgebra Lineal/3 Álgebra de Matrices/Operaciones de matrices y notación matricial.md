---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/3-algebra-de-matrices/operaciones-de-matrices-y-notacion-matricial/"}
---



# Notación

Notación matricial: $A=[A_{ij}]$

$$
\begin{bmatrix}
a_{11} & \dots & a_{1j} & \dots & a_{1n} \\
\vdots &  & \vdots & &  \vdots \\
a_{i1} & \dots & a_{ij} & \dots & a_{in} \\
\vdots &  & \vdots & &  \vdots \\
a_{m1} & \dots & a_{mj} & \dots & a_{mn}
\end{bmatrix}
$$
# Aritmética de matrices
## Suma y resta de matrices

Se suma entrada por entrada. no se pueden sumar matrices con números de filas y columnas distintas

## Ponderación de matrices

Una matriz multiplicada por un escalar, se multiplica cada una de las entradas.

## Multiplicación

Escomo sacar el producto matriz vectores de varios vectores.

$A=[a_{1},a_{2},a_{3}]$

$B=[b_{1},b_{2},b_{3}]$

$AB=[Ab_{1},Ab_{2},Ab_{3}]$

Una matriz $A\in\mathbb{R}^{m \times n}$ y $B \in \mathbb{R}^{m_{1} \times n_{1}}$

Solo se pueden multiplicar si $n=m_{1}$, y la matriz resultantes será en $\mathbb{R}^{m \times n_{1}}$

### Regla de fila columna

Dadas las siguientes matrices:

$A\in\mathbb{R}^{m\times n}$

$B\in\mathbb{R}^{n\times p}$

Entonces: $(AB)_{ij}=a_{i1}b_{1j}+a_{i 2}b_{2j}+\dots+a_{in}b_{nj}$

### Considerar
$$
AB\neq BA
$$
$$
AB=AC \not\implies B=C
$$
$$
AB=0 \not\implies A=0 \lor B=0
$$
# Transposición

Se define a la transpuesta de $A\in\mathbb{R}^{m\times n}$ como $A^{T}\in\mathbb{R}^{n\times m}$ donde las filas de $A^{T}$ son las columnas de $A$ y las columnas de $A^{T}$ son las filas de $A$.

Si:

$$
A=\begin{bmatrix}
a & b \\
c & d
\end{bmatrix} \implies A^{T}=\begin{bmatrix}
a & c \\
b & d
\end{bmatrix}
$$

Se de denomina matriz simétrica a la matriz que su transposición es idéntica a ella.

Propiedades:

- $(A^{T})^{T}=A$
- $(A+B)^{T}=A^{T}+B^{T}$
- $(cA)^{T}=cA^{T}:c\in\mathbb{R}$
- $(AB)^{T}=B^{T}A^{T}$
- $(A^{-1})^{T}=(A^{T})^{-1}$