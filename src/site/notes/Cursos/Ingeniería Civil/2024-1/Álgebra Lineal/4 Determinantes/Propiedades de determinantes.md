---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/4-determinantes/propiedades-de-determinantes/","tags":["I2MAT1203"]}
---

# Propiedades

Sea $A$ una matriz cuadrada $n\times n$:

- Si un múltiplo de una fila de $A$ se suma con otra fila de $A$ para producir una matriz $B$, entonces $Det(B)=Det(A)$
- Si dos filas de $A$ se intercambian para producir $B$, entonces $Det(B)=-Det(A)$.
{ #7c7a66}

- $A$ solo es invertible si $Det(A) \neq 0$
- $Det(A^{T})=Det(A)$
- $Det(A^{-1})=(\det(A))^{-1}$
## Multiplicaciones por escalar
- Si una fila de $A$ se multiplica por $k$ para producir $B$, entonces $Det(B)=kDet(A)$ con $k\in\mathbb{R}$.
- De lo anterior, al multiplicar $A_{n\times n}$ por $k$, es lo mismo que multiplicar todas las filas por $k$,. así: $\det(kA_{n\times n})=k^{n}\det A$
## Propiedades de operaciones

Sean $A$ y $B$ matrices de $n\times n$:

- Propiedad multiplicativa: $Det(AB)=Det(A)·Det(B)$
	- Nota, esto implica que no importa del orden de $AB$. Así:
	- $Det(AB)=Det(BA)$
## Linealidad de función determinante

Sea $T(x)$ la siguiente transformación $\mathbb{R}^{n} \rightarrow\mathbb{R}$ dada una matriz $A=[a_{1},a_{2},\dots,a_{n}]$

$$
T(x)=Det([a_{1},\dots,a_{j1},x,a_{j+1},..,a_{n}])
$$

Entonces $T(x)$ es lineal

Lo que hace $T(x)$ es tomar una columna $j$ de $A$, y saca la determinante de $A$ usando el vector que representa la columna $j$ ($x$).

# Determinante 0

> [!theorem] determinante de una matriz no invertible
> Si una matriz $A$ no es invertible, entonces $Det(A)=0$, así, una matriz cuadrada con vectores linealmente dependientes, tiene determinante 0.
{ #96fe07}


# Ejemplo
