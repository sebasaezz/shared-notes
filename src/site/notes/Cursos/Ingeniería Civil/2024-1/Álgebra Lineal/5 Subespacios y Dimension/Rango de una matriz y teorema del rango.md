---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/rango-de-una-matriz-y-teorema-del-rango/","tags":["I3MAT1203"]}
---

# Concepto

# Definición

> [!theorem] Teorema del rango
> Dada una matriz $A_{m\times n}$, su rango, está dado por la cantidad de columnas totales, menos la dimensión de su espacio nulo (la cantidad de columnas no pivote). 
> Así, lógicamente, el rango estará dado por la cantidad de columnas pivote. Esto coincidiendo con la dimensión del espacio fila y columna.
> $$
> Rango(A_{m\times n})=n-\text{dim}(\text{nul }A)=\text{dim}(\text{col }A)=\text{dim}(\text{fil }A)
> $$
{ #7c453c}


De aquí se ve que el teorema del rango no solo sirve para identificar el rango de una matriz, sino que también cosas como la dimensión de su espacio columna o el número de columnas.

# Ejemplo
## Ejemplo 1
**Enunciado**
Calcular el rango de la siguiente matriz:
$$
A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix}
$$

> [!Respuesta]-
> El rango de la matriz $A$ es $1$, ya que la tercera fila es igual a la suma de la primera y segunda fila.
> 
> **Desarrollo:**
> Para encontrar el rango de una matriz, necesitamos reducirla a su forma escalonada por filas. Empecemos con la matriz dada:
> 
> $$
> \begin{pmatrix}
> 1 & 2 & 3 \\
> 4 & 5 & 6 \\
> 7 & 8 & 9
> \end{pmatrix}
> $$
> 
> Restamos $4$ veces la primera fila a la segunda fila y $7$ veces la primera fila a la tercera fila:
> 
> $$
> \begin{pmatrix}
> 1 & 2 & 3 \\
> 0 & -3 & -6 \\
> 0 & -6 & -12
> \end{pmatrix}
> $$
> 
> Luego sumamos $2$ veces la segunda fila a la tercera fila:
> 
> $$
> \begin{pmatrix}
> 1 & 2 & 3 \\
> 0&-3&-6\\ 
> 0&0&0 
> \end{pmatrix}
> $$
> 
> Ahora, contamos cuántas filas no nulas tenemos, que son dos. Por lo tanto, el rango de la matriz es $2$.