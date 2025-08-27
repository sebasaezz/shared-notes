---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/diagonalizacion-de-una-matriz-simetrica-y-descomposicion-espectral/","tags":["ExMAT1203"]}
---

# Concepto

Las [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Matrices simétricas\|Matrices simétricas]] reales tienen la factorización $PDP^{T}$

# Ejemplo introductorio
## Multiplicidad 1

Se quiere diagonalizar la siguiente matriz

$$
A=\begin{bmatrix}
6 & -2 & -1 \\
-2 & 6 & -1 \\
-1 & -1 & 5
\end{bmatrix}
$$

Calculamos los valores propios con la ecuación caracterísitca

$$
\det A-\lambda I=(6-\lambda)(8-\lambda)(3-\lambda)
$$

Así:

$$
\lambda=\begin{cases}
\lambda_{1}= 8 \\
\lambda_{2}=6 \\
\lambda_{3}=3
\end{cases}
$$

Ahora se calculan los vectores propios resolviendo las homogénas:

Para $v_{1}$

$$
v_{1}=\begin{bmatrix}
-1 \\
1 \\
0
\end{bmatrix},v_{2}=\begin{bmatrix}
-1 \\
-1 \\
2
\end{bmatrix},
v_{3}=\begin{bmatrix}
1 \\
1 \\
1 \\
\end{bmatrix}
$$

> ==¡Es una base ortogonal!==
> -Manuel Sánchez, 2024

Se pueden ortonormalizar, de $v$ a $u$:

$$
u_{1}=\begin{bmatrix}
-\frac{1}{\sqrt{ 2 }} \\
\frac{1}{\sqrt{ 2 }} \\
0
\end{bmatrix},
u_{2}=\begin{bmatrix}
-\frac{1}{\sqrt{ 6 }} \\
-\frac{1}{\sqrt{ 6 }} \\
\frac{2}{\sqrt{ 6 }} 
\end{bmatrix}
,u_{3}=\begin{bmatrix}
\frac{1}{\sqrt{ 3 }} \\
\frac{1}{\sqrt{ 3 }} \\
\frac{1}{\sqrt{ 3 }}
\end{bmatrix}
$$

Ahora se construye a $P$, y notando que para una matriz $A$ donde $\operatorname{col}A$ es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Base ortogonal y ortonormal\|base ortonormal]] entonces $A^{-1}=A^{T}$. Se construye $PDP^{-1}=PDP^{T}$

Dado que ya hemos encontrado los vectores propios [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Ortonormalidad y conjuntos ortonormales\|ortonormalizados]] $u_1, u_2, u_3$ y los valores propios correspondientes $\lambda_{1}=8, \lambda_{2}=6, \lambda_{3}=3$, podemos construir la matriz de cambio de base $P$ y la matriz diagonal $D$. 

$$
P=\begin{bmatrix}
-\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
0 & \frac{2}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }}
\end{bmatrix}
$$
$$
D=\begin{bmatrix}
8 & 0 & 0 \\
0 & 6 & 0 \\
0 & 0 & 3
\end{bmatrix}
$$
$$
\begin{bmatrix}
-\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
0 & \frac{2}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }}
\end{bmatrix}\begin{bmatrix}
8 & 0 & 0 \\
0 & 6 & 0 \\
0 & 0 & 3
\end{bmatrix}\begin{bmatrix}
-\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
\frac{1}{\sqrt{ 2 }} & -\frac{1}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }} \\
0 & \frac{2}{\sqrt{ 6 }} & \frac{1}{\sqrt{ 3 }}
\end{bmatrix}^{T}
$$
## Multiplicidad mayor a 1

Diagonalizando:

$$
A=\begin{bmatrix}
3 & -2 & 4 \\
-2 & 6 & 2 \\
4 & 2 & 3
\end{bmatrix}
$$

Llegando a $\det A=-(\lambda-7)^{2}(2+\lambda)$

Así:

$$
\lambda=\begin{cases}
\lambda_{1}=7 \\
\lambda_{2}=7 \\
\lambda_{3}=-2
\end{cases}
$$

Ahora, los vectores de $\lambda=7$ son:

$$
v_{1}=\begin{bmatrix}
1 \\
0 \\
1
\end{bmatrix},v_{2}=\begin{bmatrix}
1 \\
-2 \\
0
\end{bmatrix}
$$

Ahora, estos vectores no son ortogonales. Para ortogonalizar el espacio se puede aplicar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Proceso de Gram-Schmit\|Proceso de Gram-Schmit]].

Sea $v_{1}=z_{1}$, entonces:

$$
z_{2}=v_{2}-\left( \frac{v_{2}·v_{1}}{v_{1}·v_{1}} \right)v_{1}=\begin{bmatrix}
-\frac{1}{4} \\
1 \\
\frac{1}{4}
\end{bmatrix}
$$

Además se llega a que, por $\lambda_{3}$:

$$
v_{3}=\begin{bmatrix}
-1 \\
-\frac{1}{2} \\
1
\end{bmatrix}
$$

Ahora, el conjunto ortogonal será $\{ v_{1},z_{2},v_{3} \}$ y se va a cumplir que $A=PDP^{-1}=PDP^{T}$, con $P=[v_{1}\space z_{2}\space v_{3}]$.

# Definiciones

> [!theorem] ortogonalidad de vectores propios de una matriz simétrica
> Sea $A$ una matriz simétrica, **con todos sus vales propios distintos**, entonces dos vectores propios cualesquiera de la matriz serán [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Ortogonalidad entre vectores\|ortogonales]].

> [!definition] matriz diagonalizable ortogonalmente
> Una matriz $A\in\mathbb{R}^{n\times n}$ será diagonalizable ortonormalmente $\iff$ existe factorización $PDP^{-1}=PDP^{T}$.
> Esto se cumplirá para todas las [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Matrices simétricas\|Matrices simétricas]].
{ #f76dc2}


> [!theorem] matrices simétricas son diagonalizables ortogonalmente
> Dada la factorización $A=PDP^{-1}$ correspondiente a la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Diagonalización de una matriz\|Diagonalización de una matriz]], se cumplirá que:
> $$
> PDP^{-1}=PDP^{T}\iff A^{-1}=A^{T}
> $$
> Es decir, es [[#^f76dc2|diagonalizable ortogonalmente]] si y solo si es [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Matrices simétricas\|simétrica]] 

## Descomposición espectral

> [!theorem] teorema espectral para matrices simétricas
> Para $A_{n\times n}$, se le llama espectro de $A$ a los valores propios de a si se cumplen las siguientes propiedades:
> 1. $A$ tiene $n$ valores propios reales considerando multiplicidades
> 2. Las multiplicidades geométricas son iguales a las algebraicas
> 3. El conjunto de los vectores propios es ortogonal
> 4. La matriz $A$ es diagonalizable ortogonalmente
> 
> A esta matriz se le puede aplicar la descomposición espectral

Sea $A_{n\times n}=PDP^{-1}=PDP^{T}$, y $\mathbf{u}_{k}$ sus vectores propios orto**normales** entonces:

$$\begin{array}{c l l c} 
 A & =&P D P^{T}= 
\left[\begin{array}{c c c c}{{{\bf u}_{1}}}&{{\cdots}}&{{{\bf u}_{n}}}\end{array}\right]
\left[\begin{array}{c c c c}{{\lambda_{1}}}&{{}}&{{}}&{{0}}\\ {{}}&{{\ddots}}&{{}}&{{}}\\ {{0}}&{{}}&{{}}&{{\lambda_{n}}}\end{array}\right]
 
\left[\begin{array}{c}{{{\bf u}_{1}^{T}}}\\ {{\vdots}}\\ {{{\bf u}_{n}^{T}}}\end{array}\right]  \\
 & =&\begin{bmatrix}
\lambda_{1}\mathbf{u}_{1} & \cdots & \lambda_{n}\mathbf{u}_{n}
\end{bmatrix}\left[\begin{array}{c}{{{\bf u}_{1}^{T}}}\\ {{\vdots}}\\ {{{\bf u}_{n}^{T}}}\end{array}\right]
\end{array}$$
Ahora notar que esta multiplicación de matrices se puede tomar como una suma (expansión fila columna de un producto).
$$

A=\lambda_{1}\mathbf{u}_{1}\mathbf{u}_{1}^{T}+\dots+\lambda_{n}\mathbf{u}_{n}\mathbf{u}_{n}^{T} \tag{1}

$$

{ #b91294}


Cada término en [[#^b91294]] es una matriz de $n\times n$, y ==de rango 1==.

- [x] Entender esta propiedad  [completion:: 2025-04-20]
Cada una de estas matrices es una [[Matriz de proyección\|Matriz de proyección]].


> [!definition] descomposición espectral
> Sea $A_{n\times n}$ una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Matrices simétricas\|matriz simétrica]], entonces, con $\mathbf{u}_{k}$ la ortonormalización de los vectores propios de $A$, se podrá descomponer de la forma:
> $$
> A=\sum_{i=1}^{n}\lambda_{i}\mathbf{u}_{i}\mathbf{u}_{i}^{T}
> $$

 