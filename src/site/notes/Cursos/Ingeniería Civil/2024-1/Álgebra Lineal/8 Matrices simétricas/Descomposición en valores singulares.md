---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/descomposicion-en-valores-singulares/","tags":["ExMAT1203"]}
---

# Concepto

Efectuar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Diagonalización de una matriz\|Diagonalización de una matriz]] $PDP^{-1}$ en $\mathbb{R}^{m\times n}$. Como es imposible, se usará una nueva factorización $QDP^{-1}$ 

Se parte con una propiedad que presenta la diagonalización normal, y es que los vectores propios nos dicen cuando se estira un vector propio $\mathbf{x}$, entonces si dicho vector es unitario ($\lvert \lvert \mathbf{x} \rvert \rvert=1$):

$$
\lvert \lvert A\mathbf{x} \rvert \rvert =\lvert \lvert \lambda \mathbf{x} \rvert \rvert =|\lambda|\lvert \lvert \mathbf{x} \rvert \rvert =|\lambda|
$$

Así se cumplirá que los $\lambda$ dirán la longitud de estiramiento en las direcciones de sus vectores propios de la forma que tenga la transformación. Así, al tener un $\lambda_{1}$ de mayor magnitud, entonces el vector propio asociado $\mathbf{v}_{1}$ indicará la dirección en la que la transformación amplíe más la norma de el vector que transforma. Es decir, si $\mathbf{x}=\mathbf{v}_{1}\implies \lvert \lvert A\mathbf{x} \rvert \rvert>\lvert \lvert A\mathbf{x}_{1} \rvert \rvert :\mathbf{x}_{1}$ siendo cualquier otro vector con la misma norma que $\mathbf{x}$.

## Ejemplo introductorio

A continuación se verá como lo dicho nos puede acercar a una diagonalización de matrices rectangulares.

Sea:

$$
A=\begin{bmatrix}
4 & 11 & 14  \\
8 & 7 & -2
\end{bmatrix}
$$

Entonces, al analizar el mapeo de la esfera unitaria $\{ \mathbf{x}\in\mathbb{R}^{3}:\lvert \lvert \mathbf{x} \rvert \rvert=1 \}$ se da que es sobre una elipse en $\mathbb{R}^{2}$.

![Pasted image 20240707011229.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/8%20Matrices%20sim%C3%A9tricas/attachments/Pasted%20image%2020240707011229.png)

Encontrar el vector unitario $\mathbf{x}$ tal que se maximice la longitud de $A\mathbf{x}$.

### Solución

Notar que $\lvert \lvert A\mathbf{x} \rvert \rvert^{2}$ se maximiza de la misma forma que $\lvert \lvert A\mathbf{x} \rvert \rvert$. Por la definición de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Producto punto o interior y propiedades#^7997eb\|producto interior]], se tiene que $\lvert \lvert A\mathbf{x} \rvert \rvert^{2}=(A\mathbf{x})^{T}Ax=\underbrace{ \mathbf{x}^{T}(A^{T}A)\mathbf{x} }_{ \text{forma cuadrática} }$.

Ahora, $A^{T}A$ siempre será una matriz cuadrada simétrica, ya que $(A^{T}A)^{T}=A^{T}A$. ¡Se tiene una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas\|forma cuadrática]]! y está restringida para $\lvert \lvert \mathbf{x} \rvert \rvert=1$. Entonces se puede usar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas#^28e8d9\|este teorema]] que dice que el valor menor y mayor serán los valores propios, y el $\mathbf{x}$ unitario asociado serán los vectores propios (normalizados si es que no salen unitarios).

$$
\begin{array}{}
 & A^{T}A=\begin{bmatrix}
4 & 8 \\
11 & 7 \\
14 & -2
\end{bmatrix}\begin{bmatrix}
4 &11 & 4  \\
8 & 7 & -2
\end{bmatrix}= \begin{bmatrix}
 80 & 100 & 40 \\
100 & 170 & 140 \\
40 & 140 & 200
\end{bmatrix}
\implies
\begin{cases}
\lambda_{1}=360 \\
\lambda_{2}=90 \\
\lambda_{3}=0
\end{cases}   & \\
\implies & \mathbf{v}_{1}=\begin{bmatrix}
\frac{1}{3}   \\
\frac{2}{3} \\
\frac{2}{3}
\end{bmatrix},\mathbf{v}_{2}=\begin{bmatrix}
-\frac{2}{3} \\
-\frac{1}{3} \\
\frac{2}{2} 
\end{bmatrix},\mathbf{v}_{3}=\begin{bmatrix}
\frac{2}{3} \\
-\frac{2}{3} \\
\frac{1}{3}
\end{bmatrix}
\end{array}
$$

Ahora, se considerará a $\lambda_{1}=360$ que será el máximo de $\lvert \lvert A\mathbf{x} \rvert \rvert^{2}$, así para $\lvert \lvert \mathbf{x} \rvert \rvert=1$ el valor máximo de $\lvert \lvert A\mathbf{x} \rvert \rvert$ es $\lvert \lvert A\mathbf{v}_{1} \rvert \rvert=\sqrt{ 360 }=6\sqrt{ 10 }=\sigma_{1}$ este valor se le denominará valor singular.

## Los valore singulares de una matriz

Sea $A_{m\times n}$. Entonces $A^{T}A$ se podrá diagonalizar ortogonalmente con $\{ \mathbf{v}_{1},\mathbf{v}_{2},\dots,\mathbf{v}_{n} \}$ como base ortonormal consistente en los vectores propios de $A^{T}A$. Entonces, para $1\leq \lambda_{i}\leq\lambda_{n}$:

$$
\begin{align}
\lvert \lvert A\mathbf{v}_{i} \rvert \rvert ^{2} & =(A\mathbf{v}_{i})^{T}A\mathbf{v}_{i}=\mathbf{v}_{i}^{T}(A^{T}A)\mathbf{v}_{i} \\
 & =\mathbf{v}_{i}^{T}(\lambda_{i}\mathbf{v}_{i})  & \lvert \lvert \mathbf{v}_{i} \rvert \rvert =1\\
 & =\lambda_{i}
\end{align}
$$

Ahora, se ordenan en orden decreciente los valores propios:

$$
\lambda_{1} \geq \lambda_{2} \geq\dots \geq\lambda_{n}\geq 0
$$

Notar que siempre serán positivos los valores propios. ¿Por qué?

Los valores singulares serán la raíces de estos valores propios en orden decreciente, esto es $\sigma_{i}=\sqrt{ \lambda_{i} }=\lvert \lvert A\mathbf{v}_{i} \rvert \rvert$.

> [!theorem] ortogonalidad imagen de vectores propios para valores singulares
> Sea $\{ \mathbf{v}_{1},\dots,\mathbf{v}_{n} \}$ una base de $\mathbb{R}^{n}$ consistende de vectores propios de una matriz $A^{T}A$ acomodados con sus valores propios en orden descendiente. Suponiendo que $A$ tiene $r$ valore singulares distintos de $0$, entonces $\{ A\mathbf{v}_{1},\dots,A\mathbf{v}_{r} \}$ será una base ortogonal de $\operatorname{Col}A$. Además será el **rango** de la matriz.

# La descomposición en valores singulares

Efectuar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Diagonalización de una matriz\|Diagonalización de una matriz]] $A=PDP^{-1}$ para $A\in\mathbb{R}^{m\times n}$. Como es imposible, se usará una nueva factorización $U\Sigma V^{T}$.

La matriz $\Sigma_{m\times n}$ es una matriz "diagonal", de la siguiente forma:

$$
\Sigma=
\underbrace{ \begin{bmatrix}
D_{r\times r} & 0 \\
0 & 0
\end{bmatrix} }_{ n-r \text{ col de 0} }  \Big\} \tiny{m-r\text{ filas de ceros}} \tag{1}
$$
{ #5bf698}


Donde $D$ es una matriz de $r\times r$ donde $r\leq m \land r\leq n$. Si es igual a uno, entonces no hay filas o columnas de ceros.

> [!theorem] Descomposición en valores singulares
> Sea $A$ una matriz de $m\times n$ de **rango** $r$, entonces existirá una matriz $\Sigma$ de la forma vista en [[#^5bf698|(1)]], para la que $D$ es diagonal con los primeros $r$ valores singulares $\sigma$ de $A$ en orden decreciente. Existirá una matriz $U$ ortogonal de $m\times m$ y una matriz $V$ ortogonal de $n\times n$ tales que:
> $$
> A=U\Sigma V^{T}
> $$
> - A las columnas de $U$ se le llaman vectores singulares izquierdos de $A$
> - A las columnas de $V$ se le llaman vectores singulares derechos de $A$

## Cómo diagonalizar (ejemplo anterior)

Volviendo al ejemplo anterior, ya se tiene a $A^{T}A$ y a sus valores propios. De los valores propios se pueden calcular los valores singulares:

$$
\sigma_{1}=6\sqrt{ 10 },\sigma_{2}=\sqrt{ 90 }=3\sqrt{ 10 },\sigma_{3}=0
$$

# Definición
# Ejemplo