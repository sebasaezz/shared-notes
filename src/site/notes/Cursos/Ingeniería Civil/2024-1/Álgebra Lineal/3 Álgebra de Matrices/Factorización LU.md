---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/3-algebra-de-matrices/factorizacion-lu/","tags":["I2MAT1203"]}
---


Se representa una matriz como el producto de dos o más matrices, en la forma:

$$
A=LU
$$

El proceso de reducción por filas, induce a una factorización de forma natural, si se considera a las operaciones por fila, como una matriz elemental, entonces se está haciendo una factorización.

$$
(E_{1}E_{2}\dots E_{n})A=U \iff A=U(E_{1}^{-1}E_{2}^{-1}\dots E_{n}^{-1})
$$

Esto implica que A se puede reducir a escalonada sin hacer intercambio de filas

> [!definition] Matriz triangular unitaria
> Se define a una matriz triangular unitaria como una matriz cuadrada triangular donde las entradas pertenecientes a la diagonal son todas $1$. Así, la siguiente matriz $A$, es una matriz triangular inferior:
> $$A=
> \begin{bmatrix}
> 1 & 0 & \dots & 0 \\
> a_{21} & 1 & \dots &0 \\
> \vdots &\vdots & \ddots & \vdots \\
> a_{n 1} & a_{n 2} & \dots & 1  
> \end{bmatrix}
> $$
{ #2741b2}


# Definición

> [!definition] Factorización LU de una matriz
> Se defina a $U_{m\times n}$ como una matriz triangular inferior  y a $L_{m\times m}$ como una matriz triangular [[#^2741b2]] inferior, entonces la factorización $LU$ es la representación de una matriz $A_{m\times n}$ invertible de la siguiente forma:
> $$
> A=LU
> $$
{ #490a6d}


## Método de cálculo de L

dada una matriz $A_{m\times n}$, se debe lograr la matriz $U_{m\times n}$ escalonando la matriz (sin hacer cambios de fila ni ponderar filas). Esto se hace con pivoteo. Ahora, cada columna en su estado antes de pivotear pertenece a la columna en $L_{m\times m}$ desde el pivote hacia abajp, solo que se debe dividir por el pivote para que sea uno, es decir:

Por ejemplo, dada:

$$
A=\begin{bmatrix}
2 & 4 & -1 & 5 & -2 \\
-4 & -5 & 3 & -8 & 1 \\
2 & -5 & -4 & 1 & 8 \\
-6 & 0 & 7 & -3 & 1 \\

\end{bmatrix}
$$

Entonces, se pivotea de la siguiente forma:

![Pasted image 20240509143506.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/3%20%C3%81lgebra%20de%20Matrices/attachments/Pasted%20image%2020240509143506.png)

Finalmente y dado lo dicho anteriormente, se considera a $L$ de la siguiente forma:

![Pasted image 20240509143536.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/3%20%C3%81lgebra%20de%20Matrices/attachments/Pasted%20image%2020240509143536.png)

# Teorema

> [!theorem] Existencia de factorización LU
> Si $A$ es una matriz cuadrada que puede reducirse a forma escalonada sin usar intercambios de filas, entonces A tiene una [[#^490a6d|factorización LU]].

# Teorema

> [!theorem] Unicidad de factorización LU
> Si $A$ es invertible, solo van a existir una $L$ y una tales que sigan una [[#^490a6d]].

# Resolución con LU

> [!theorem] Resolución de un sisstema con factorización LU
> Dado el sistema $Ax=b$, se cumple que, utilizando la [[#^490a6d]]:
> $$
> Ax=b \iff L\underbrace{Ux}_{y}=b\leftrightarrow \begin{cases}
> Ly & = & b \\
> Ux & = & y
> \end{cases}
> $$
> A $y$ se le denomina una variable auxiliar, y se debe resolver con los siguientes pasos:
> 1. Se resuelve a $y$ en $Ly=b$ mediante sustitución.
> 2. Se resuelve $x$ en $Ux=y$ usando la $y$ ya descubierta.

# Ejemplos
## Ejemplo 1

Encontrar la descomposición LU de la matriz

$$
A=\begin{bmatrix}
1 & 0 & 1  \\
a & a & a \\
b & b & a
\end{bmatrix}
$$

cuando exista.

Para qué números reales $a$ y $b$ existe la descomposición?

$$
A \sim \begin{bmatrix}
1 & 0 & 1 \\
a-a & a & a-a \\
b-b & b & a-b
\end{bmatrix} \sim \begin{bmatrix}
1 & 0 & 1 \\
0 & a & 0 \\
0 & b & a-b
\end{bmatrix} \sim \begin{bmatrix}
1 & 0 &  1\\
0 & a & 0 \\
0 & 0 & a-b
\end{bmatrix}=U
$$
$$
\implies L=\begin{bmatrix}
1  & 0 & 0\\
a  & 1 & 0\\
b & \frac{b}{a} & 1
\end{bmatrix}
$$

Notar que el tercer paso no se pudo haber hecho si es que $a=0$, se hubiera tenido que hacer una permutación, y se está haciendo una descomposición $LU$, no una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/3 Álgebra de Matrices/Factorización PALU o PTLU\|Factorización PALU o PTLU]]. De la misma forma (y por la misma razón), la entrada $l_{32}=\frac{b}{a}$ sería indefinida si $a=0$. 

Finalmente $a\in\mathbb{R}-\{ 0 \} \land b\in\mathbb{R}$.f