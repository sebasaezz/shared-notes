---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/1-ecuaciones-lineales-en-algebra-lineal/ecuacion-matricial-ax-b/"}
---


Sea $A\in\mathbb{R}^{m\times n}$ y $b\in\mathbb{R}^m$, con $A=[a_{1},a_{2},\dots,a_{n}]$.

Con $a_{n}$ siendo vectores columnas de A.

Entonces los siguientes tienen la misma solución a la ecuación $A\mathbf{x}=\mathbf{b}$:

- La siguiente [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Ecuación vectorial#^cb63c9\|ecuación vectorial]]:

$$
x_{1}\mathbf{a}_{1},x_{2}\mathbf{a}_{2}+\dots+x_{n}\mathbf{a}_{n}=\mathbf{b}
$$
- Sistema de ecuaciones lineales con [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Resolviendo sistemas de ecuaciones lineales con matrices aumentadas y matrices convenientes#^3430f1\|matriz aumentada]] 
$$
\left[ \begin{array}{cccc|c}
\mathbf{a}_{1} & \mathbf{a}_{2} & \cdots & \mathbf{a}_{n} & \mathbf{b}
\end{array} \right] 
$$
*Si es que todas las entradas son números ($\{ a_{1},a_{2},\dots,a_{n} \}$ es un [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Independencia y dependencia lineal#^6e8a52\|conjunto l.i.]] ), el resultado será un vector en $\mathbb{R}^m$.*
# Producto matriz-vector

> [!definition] producto matriz vector y matrices
> Si el producto de la matriz A, con el vector $x$ está definido (Nº de columnas de $A=$ Nº de entradas de $x$), entonces la $i$-ésima entrada de $Ax$ es la suma de los productos de las entradas correspondientes de la fila $i$ y del vector $x$.
> Es decir:
> $$
> \begin{bmatrix}
> a_{11} & \dots & a_{1n} \\
> \vdots & \ddots & \vdots \\
> a_{m 1} & \dots & a_{mn}
> \end{bmatrix}\begin{bmatrix}
> x_{1} \\
> \vdots \\
> x_{n}
> \end{bmatrix}=\begin{bmatrix}
> a_{11}·x_{1}+\dots+a_{1n}·x_{n} \\
> \vdots \\
> a_{m1}·x_{1} +\dots+a_{mn}·x_{n}
> \end{bmatrix}
> $$

# Ecuación matricial

> [!definition] ecuación matricial Ax=b
> Dada $A\mathbf{x}=\mathbf{b}$ con $A\in\mathbb{R}^{m\times n}$, $\mathbf{b}\in\mathbb{R}^{m}$ y $\mathbf{x}\in\mathbb{R}^{n}$:
> $$
> \begin{bmatrix}
> a_{11} & a_{12}\\
> a_{21} & a_{22}
> \end{bmatrix}\begin{bmatrix}
> x_{1} \\
> x_{2}
> \end{bmatrix}=\mathbf{b}\implies
> \left[ \begin{array}{ccc}
> a_{11}·x_{1} + a_{12}·x_{2} \\
> a_{21}·x_{1} + a_{22}·x_{2}
> \end{array} \right] 
> =\mathbf{b}
> $$
> Implicando así el sistema:
> $$
> \begin{cases}
> a_{11}x_{1}+a_{12}x_{2}=b_{1} \\
> a_{21}x_{1}+a_{22}x_{2}=b_{2}
> \end{cases}
> $$

## Ejemplos

1

$$
\begin{bmatrix}
1 & 2 & -1 \\
0 & -5 & 3
\end{bmatrix} 
\begin{bmatrix}
4 \\
3 \\
7
\end{bmatrix}
=
\begin{bmatrix}
1·4+2·3-1·7 \\
0·4-5·3+3·7
\end{bmatrix}
=
\begin{bmatrix}
3 \\
6
\end{bmatrix}
$$

2, matriz identidad

$$
\left[ 
 \begin{array}{}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array} 
 \right]\begin{bmatrix}
x_{1} \\
x_{2} \\
x_{3} \\
\end{bmatrix}
=
\begin{bmatrix}
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
$$
# Propiedades de producto matriz-vector
1. Distributiva: $A(u+v)=Au+Av$
2. Asociativa: $A(cu)=c(Au)$
# Teoremas
