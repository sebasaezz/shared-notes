---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/vectores-propios-valores-propios-y-espacio-propio/","tags":["I3MAT1203"]}
---

# Concepto

Dada una transformación $x \to Ax$

Esta transformación mueve vectores en cualquier dirección, pero existen ciertos vectores que se mueven de forma más simple, con una ponderación por una constante.

# Valores y vectores propios

> [!definition] Valores y vectores propios reales
> Un vector propio de una matriz $A_{n\times n}$ es un vector distinto de cero $x$ tal que:
> $$
> Ax=\lambda x:\lambda \in\mathbb{R}
> $$
> Se define a $\lambda$ como el valor propio
{ #1a33f2}


_Nota: $0$ puede ser valor propio_

## Valores propios en una matriz triangular

> [!theorem] Valores propios de una matriz triangular
> Los valores propios de una matriz triangular son las entradas de su diagonal principal
{ #fa3dee}


# Espacio propio

> [!theorem] Espacio propio como espacio nulo
> Si se buscan los vectores propios de $A$, se cumple que:
> $$
> Ax=\lambda x \iff(A-\lambda I)x=0
> $$
> Entonces:
> $$
> \boxed{\text{Espacio propio de }A \text{ correspondiente a }\lambda =\text{Nul}(A-\lambda I)\text{ con }\lambda \in\mathbb{R}:Ax=\lambda x} 
> $$
> Es decir, buscar los vectores propios de $A$, es buscar el espacio nulo de la matriz $A-\lambda I$ para un cierto $\lambda$.
> $\lambda$ es valor propio de $A$ $\iff$ la ecuación anterior tiene solución no trivial. De esto se desprende el concepto de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Ecuación característica y polinomio característico\|Ecuación característica y polinomio característico]].

Ver [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Vectores propios, valores propios y espacio propio#Ejemplo 1\|Ejemplo 1]]:

![Pasted image 20240520102711.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/6%20Valores%20y%20Vectores%20Propios%20de%20Matrices%20Simetricas/attachments/Pasted%20image%2020240520102711.png)

# Independencia lineal de vectores propios

Un conjunto de vectores propios siempre va a ser linealmente independiente

> [!theorem] Independencia lineal de vectores propios
> Si $\{ v_{1},v_{2},\dots,v_{n} \}$ son vectores propios correspondientes a valores propios $\{ \lambda_{1},\lambda_{2},\dots,\lambda_{n} \}$ de una matriz $A_{n\times n}$ entonces el conjunto es vectores $v$ es linealmente independiente.

# Ejemplo
## Ejemplo 1

Sea:

$$
A= \begin{bmatrix}
1 & 6 \\
5 & 2
\end{bmatrix}
,u=\begin{bmatrix}
6 \\
-5
\end{bmatrix},v=\begin{bmatrix}
3 \\
-2
\end{bmatrix}$$
$u$ es un vector propio, y su valor propio es $-4$, eso es que dado que:
$$

\begin{bmatrix}

1 & 6 \\

5 & 2

\end{bmatrix}\begin{bmatrix}

6 \\

-5

\end{bmatrix}=-4\begin{bmatrix}

6 \\

-5

\end{bmatrix}

$$
$v$ no es vector propio, ya que:
$$

\begin{bmatrix}

1 & 6 \\

5 & 2

\end{bmatrix}

\begin{bmatrix}

3 \\

-2

\end{bmatrix}=

\begin{bmatrix}

-9 \\

11

\end{bmatrix} \implies 

\not \exists \lambda \in\mathbb{R}:

\begin{bmatrix}

-9 \\

11

\end{bmatrix}=\lambda \begin{bmatrix}

3 \\

-2

\end{bmatrix}

$$
Ahora, demostrar que $7$ es valor propio de $A$
$$

Ax=7x \iff \begin{bmatrix}

1 & 6 \\

5 & 2

\end{bmatrix}

\begin{bmatrix}

a \\

b

\end{bmatrix}=7\begin{bmatrix}

a \\

b

\end{bmatrix}

$$
$$\implies
\begin{cases}
a & + & 6b & = & 7a \\
5a & + & 2b & = & 7b
\end{cases}\implies
\begin{cases}
-6a & + & 6b & = & 0 \\
5a & - & 5b & = & 0
\end{cases}\implies a=b
$$
$$
x= \left\{ b\begin{bmatrix}
1 \\
1
\end{bmatrix}:b\in \mathbb{R}- \{ 0 \} \right\}
$$

¿Por qué $b \neq 0$?

Por definición, un vector propio no puede ser $\vec{0}$.