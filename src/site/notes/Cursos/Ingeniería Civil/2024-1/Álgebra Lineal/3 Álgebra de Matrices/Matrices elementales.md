---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/3-algebra-de-matrices/matrices-elementales/"}
---

Una matriz elemental es una matriz que se obtiene al hacer una única operación por fila en una matriz identidad.

Multiplicar una matriz $A$ por una matriz elemental $E_{1}$ que se le aplicó la operación $F$, es lo mismo que aplicarle la operación $F$ a $A$.

![Pasted image 20240401100142.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/3%20%C3%81lgebra%20de%20Matrices/attachments/Pasted%20image%2020240401100142.png)

Todas las matrices elementales son inversibles. La inversa de una elemental es la elemental que representa la operación inversa a la operación que se le aplicó a la elemental.

La inversa es aplicarle a la identidad la operación que aplica la elemental.

# Ejemplo

![Pasted image 20240401101354.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/3%20%C3%81lgebra%20de%20Matrices/attachments/Pasted%20image%2020240401101354.png)

# Un algoritmo para determinar la inversa

Se quiere obtener $A^{-1}$

Se crea la matriz aumentada $[AI]$

SI $A$ es equivalente en filas a $I$, entonces tenemos: $[AI] =[IA^{-1}]$

Si no se da, entonces $A$ no es invertible

## Ejemplo

Encontrar la inversa de $A$:

![Pasted image 20240401102201.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/3%20%C3%81lgebra%20de%20Matrices/attachments/Pasted%20image%2020240401102201.png)

Entonces, dado que $[AI]=[IA^{-1}]$:

$$
A^{-1}= \begin{bmatrix}
-\frac{9}{2} & 7 & -\frac{3}{2} \\
-2 & 4 & -1 \\
\frac{3}{2} & -2 & \frac{1}{2}
\end{bmatrix}
$$