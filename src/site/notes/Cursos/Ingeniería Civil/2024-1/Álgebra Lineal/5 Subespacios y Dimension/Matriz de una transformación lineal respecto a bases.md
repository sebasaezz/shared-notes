---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/matriz-de-una-transformacion-lineal-respecto-a-bases/","tags":["I3MAT1203"]}
---

# Concepto

Pasar de $x$ a $T(x)$ nos lleva a una interpretación de $[x]_{B} \to [T(x)]_{C}$ con $B$ y $C$ bases de el espacio de $x$ y de $T(x)$.

Esta interpretación se considera como una matriz tal que $[x]_{B}M=[T(x)]_{C}$.

![Pasted image 20240527100924.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/6%20Valores%20y%20Vectores%20Propios%20de%20Matrices%20Simetricas/attachments/Pasted%20image%2020240527100924.png)

# Definición
$$
M=[[T(b_{1})]_{C},\dots,[T(b_{n})]_{C}]\in\mathbb{R}^{m\times n}
$$

# Ejemplo

Suponga que $B=\{ b_{1},b_{2} \}$ es base de $V$ y $C=\{ c_{1},c_{2},c_{3} \}$ base de $W$.

Ahora $T:V\to W$ es tal que:

$T(b_{1})=3c_{1}-2c_{2}+5c_{3}$

$T(b_{2})=4c_{1}+7c_{2}-c_{3}$

Ahora determinar a $M$:

Se debe encontrar $[T(b_{1})]_{C}$ y $[T(b_{2})]_{C}$, ya que estas dos están desde $B$.

Así:

$$
[T(b_{1})]_{C}=\begin{bmatrix}
3 \\
-2 \\
5
\end{bmatrix}
;
[T(b_{2})]_{C}=\begin{bmatrix}
4 \\
7 \\
-1
\end{bmatrix}
$$

Finalmente, se concluye que:

$$
M=\begin{bmatrix}
3 & 4 \\
-2 & 7 \\
5 & -1
\end{bmatrix}
$$
