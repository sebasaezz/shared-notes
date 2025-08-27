---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/valores-propios-complejos/","tags":["ExMAT1203"]}
---

# Concepto

Utilizando el teorema que dice que para todo polinomio de grado $n$, existen $n$ soluciones en $\mathbb{C}$.

# Definición

> [!definition] Valores propios complejos
> Un escalar complejo $\lambda \in\mathbb{C}$, satisface que $\det(A-\lambda I)=0$ si y solo si existe un vector distinto de 0 $x \in \mathbb{C}^{n}$ tal que:
> $$Ax=\lambda x$$
> Finalmente, $x$ es un vector propio [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Números, vectores y matrices complejos#^aa2db5\|complejo]]  y $\lambda$ es un valor propio [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Números, vectores y matrices complejos#^889a66\|complejo]] .

# Ejemplo
## Ejemplo

es una matriz que gira el plano a $90º$ antihorario.

Nótese que $A$ es periódica, después de 4 rotaciones se repite.

Ahora, la ecuación característica es:

$$
\lambda+1=0 \implies \lambda=\begin{cases}
\lambda_{1} & = & -\sqrt{ -1 } & = & -i \\
\lambda_{2} & = & \sqrt{ -1 } & = & i
\end{cases}
$$

Se tiene la ecuación:

$$
\begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}·x=ix \implies x=\begin{bmatrix}
1 \\
-i
\end{bmatrix}
$$
$$
\begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}·x=-ix \implies x=\begin{bmatrix}
1 \\
i
\end{bmatrix}
$$
## Ejemplo 2