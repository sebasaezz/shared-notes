---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/aplicacion-de-problemas-de-minimos-cuadrados-a-modelos-lineales-conflict-2025-07-11-16-15-08/","tags":["ExMAT1203"]}
---

# Concepto

Derivar una regresión lineal de un conjunto de datos por medio del [[Problema de mínimos cuadrados\|Problema de mínimos cuadrados]].

La relación va a estar dada por una recta $y=\beta_{0}+\beta_{1}x$.

**Definiciones:**

- $(x_{j},y_{j})$: punto de datos, $y_{i}$ valor observado
- $(x_{j},\beta_{0}+\beta_{1}x_{j})$: punto sobre regresión
- $|(y_{j})-(\beta_{0}+\beta_{1}x_{j})|$ residuo o error
Se quiere minimizar el valor del residuo.
- $\beta_{0}$ y $\beta_{1}$ son los coeficientes de regresión.

**Formulación**
Para el conjunto de datos $\{ (x_{1},y_{1}),\dots,(x_{n},y_{n}) \}$.
Si los datos fuesen sacados perfectamente de la recta, se cumpliría que:
$$
\begin{bmatrix}
1 & x_{1} \\
1 & x_{2} \\
\vdots & \vdots \\
1 & x_{n-1} \\
1 & x_{n}
\end{bmatrix}
\begin{bmatrix}
\beta_{0} \\
\beta_{1}
\end{bmatrix}
=
\begin{bmatrix}
y_{1} \\
y_{2} \\
\vdots \\
y_{n-1} \\
y_{n}
\end{bmatrix}
$$

Esta ecuación se define de la forma:

$$
X\beta=y
$$

Y se quiere encontrar el $\beta$ que más se asemeje a la recta.

Para los valores reales $x$ e $y$, resulta que este sistema es inconsistente.

# Ejemplo

Para el conjunto de datos:

$\{ (2,1),(5,2),(7,3),(8,3) \}$ 

$$
X=\begin{bmatrix}
1 & 2 \\
1 & 5 \\
1 & 7 \\
1 & 8
\end{bmatrix},\beta=\begin{bmatrix}
\beta_{0} \\
\beta_{1}
\end{bmatrix},y=
\begin{bmatrix}
1 \\
2 \\
3 \\
3
\end{bmatrix}
$$

Ahora se tendrá que la $\beta$ más cercana cumplirá la siguiente ecuación normal:

$$
X^{T}y=X^{T}X\beta
$$

Ahora se resuelve $X^{T}y$ y $X^{T}X$ y se resuelve el sistema:

$$
X^{T}y=\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 5 & 7 & 8
\end{bmatrix}\begin{bmatrix}
1 \\
2 \\
3 \\
3
\end{bmatrix}=\begin{bmatrix}
9 \\
57
\end{bmatrix}
$$
$$
X^{T}X=\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 5 & 7 & 8
\end{bmatrix}\begin{bmatrix}
1 & 2 \\
1 & 5 \\
1 & 7 \\
1 & 8
\end{bmatrix}=\begin{bmatrix}
4&22\\22&142
\end{bmatrix}
$$

