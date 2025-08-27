---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/1-ecuaciones-lineales-en-algebra-lineal/ecuacion-vectorial/","tags":["I2MAT1620"]}
---


Dada una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Combinaciones lineales y espacio generado\|combinación lineal]], se puede establecer una ecuación, la cual se representa en una matriz **expandida**. Donde cada columna es un vector.

Ejemplo:

$$
a\begin{bmatrix}
1 \\
2
\end{bmatrix}+b\begin{bmatrix}
3 \\
4
\end{bmatrix}=\begin{bmatrix}
5 \\
8
\end{bmatrix}
$$

Se representa como:

$$
\left[ \begin{array}{cc|c}
1 & 3 & 5 \\
2 & 4 & 8
\end{array}  \right] 
$$

Así como también con la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Ecuación matricial Ax=b\|Ecuación matricial Ax=b]]:

$$
\begin{bmatrix}
1 & 3 \\
2 & 4
\end{bmatrix}x=\begin{bmatrix}
5 \\
8
\end{bmatrix}
$$

Finalmente, una ecuación vectorial tiene la siguiente definición.

> [!definition] ecuación vectorial
> Una ecuación dada por una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Combinaciones lineales y espacio generado#^71df8b\|combinación lineal]] para resolver un vector $\mathbf{x}\in\mathbb{R}^{m}=\begin{bmatrix}x_{1}\\x_{2}\\\vdots\\ x_{n}\end{bmatrix}$ dado un conjunto de vectores $a=\{ \mathbf{a}_{1},\mathbf{a}_{2},\dots,\mathbf{a}_{n} \}$ todos en $\mathbb{R}^{m}$ y un vector resultante de la combinación $\mathbf{b}\in\mathbb{R}^{m}$. Es decir:
> $$
> x_{1}\mathbf{a}_{1}+x_{2}\mathbf{a}_{2}+\dots+x_{n}\mathbf{a}_{n}=\mathbf{b}
> $$
> Esto es equivalente a hablar de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Ecuación matricial Ax=b\|Ecuación matricial Ax=b]] con la matriz $A_{m\times n}=\begin{bmatrix}\mathbf{a}_{1}&\mathbf{a}_{2}&\cdots&\mathbf{a}_{n}\end{bmatrix}$ 

^cb63c9