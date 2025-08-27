---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/ecuacion-caracteristica-y-polinomio-caracteristico/","tags":["I3MAT1203"]}
---


Para que el sistema $(A-\lambda I)x=0$ tenga soluciones no triviales, entonces la matriz no puede ser invertible, es decir |$\det(A-\lambda I)=0$. 

> [!definition] Polinomio característico
> Se define como polinomio característico para una matriz $A$, donde $\lambda$ don valores propios, al polinomio resultante de $\det(A-\lambda I)$
> Los resultados de igualar este polinomio a $0$ son los valores $\lambda$ para $A$
{ #7bf0cd}


# Definición

> [!definition] Ecuación característica
> Para una matriz $A$, donde $\lambda$ es un valor propio, la ecuación característica está dada por $$Det(A-\lambda I)=0$$
{ #729b96}


# Ejemplo

Para la matriz:

$$
A=\begin{bmatrix}
2 & 3 \\
3 & -6
\end{bmatrix}
$$

Se debe tener que:

$$
0=Det \left( \begin{bmatrix}
2-\lambda  & 3 \\
3 & -6-\lambda 
\end{bmatrix} \right)=
(2-\lambda)(-6-\lambda)-9 =(\lambda-3)(\lambda+7)
\begin{cases}
\lambda_{1}=3 \\
\lambda_{2}=-7
\end{cases}
$$