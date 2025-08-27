---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/1-ecuaciones-lineales-en-algebra-lineal/combinaciones-lineales-y-espacio-generado/"}
---

> [!definition] combinación lineal
> Se va a multiplicar por un arreglo de escalares a un arreglo de vectores determinado.
> Dados los vectores $v=\{ v_{1}, v_{2}, \dots v_{n} \}\in\mathbb{R}^n$ y los coeficientes escalares, o pesos $c=\{ c_{1}, c_{2},\dots,c_{n} \}\in\mathbb{R}$. Entonces el vector:
> $$
> y=c_{1}v_{1}+c_{2}v_{2}+\dots+c_{n}v_{n}\in\mathbb{R}^n
> $$
> Es combinación lineal de $v$. Es decir, es [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Independencia y dependencia lineal#^8a3fb0\|linealmente dependiente]]. 
{ #71df8b}


## Definición

Si tengo $v_{1}, v_{2}, \dots v_{n}\in\mathbb{R}^n$, entonces el conjunto de todas las combinaciones lineales de denomina:

$$
\boxed{Gen\{ v_{1}, v_{2}, \dots v_{n} \}}\in \mathbb{R}^n 
$$
### Ejemplo 

Sea:

$$
a_{1}=\begin{bmatrix}
1 \\
-2 \\
3
\end{bmatrix}, a_{2}=
\begin{bmatrix}
5 \\
-13 \\
3
\end{bmatrix}
,
b=
\begin{bmatrix}
-3 \\
8 \\
1
\end{bmatrix}
$$

Entonces:

$$
Gen\{ a_{1},a_{2} \}=\{ v\in\mathbb{R}^3 :v=\alpha \begin{bmatrix}
1 \\
-2 \\
3
\end{bmatrix}+\beta \begin{bmatrix}
5 \\
-13 \\
-3
\end{bmatrix}:\alpha,\beta \in\mathbb{R} \}
$$

Pregunta: ¿$b\in Gen\{ a_{1},a_{2} \}$?
