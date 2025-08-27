---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/cambio-de-variable-de-la-forma-cuadratica/","tags":["ExMAT1203"]}
---

# Concepto

Tomar una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas\|Formas cuadráticas]] y dejarla sin factores cruzados.

# Definición

Para las [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Formas cuadráticas\|Formas cuadráticas]], se considera a $x=Py$ con $x \in \mathbb{R}^{n}$ y $P \in \mathbb{R}^{n\times n}$.

Entonces para la forma cradrática $Q(x)=x^{T}Ax$ se tiene:

$$
\begin{align}
x^{T}Ax & =(Py)^{T}A(Py) \\
 & =y^{T}(P^{T}AP)y
\end{align}
$$

Como $A$ se le puede aplicar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Diagonalización de una matriz simétrica y descomposición espectral\|Diagonalización de una matriz simétrica y descomposición espectral]]:

$$
\begin{align}
 &  & A & =PDP^{T} &  & \\
\implies &  & P^{T}AP & =P^{T}PDP^{T}P \\
 &  &  & = D 
\end{align}
$$

_Notar que $P$ es una matriz ortonormal, entonces $P^{T}P=I$_

Finalmente, se tiene que para el cambio de variable $x=Py$:

$$
x^{T}Ax=y^{T}Dy
$$

> [!theorem] teorema de los ejes principales
> Sea $A$ una matriz simétrica, entonces existe un cambio de variable ortigonal $x=Py$ que convierte la forma cuadrática $x^{T}Ax$ a $y^{T}Dy$ sin productos cruzados.

![Pasted image 20240621103830.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/8%20Matrices%20sim%C3%A9tricas/attachments/Pasted%20image%2020240621103830.png)

## Concepto gráfico del cambio de variable

Las gráficas que tienen términos cruzados, representan una rotación en torno al origen.

Por ejemplo, para $Q(x)=5x_{1}^{2}-4x_{1}x_{2}+5x_{2}^{2}$.

Se tiene:

$$
P=\begin{bmatrix}
\frac{1}{\sqrt{ 2 }} & \frac{1}{\sqrt{ 2 }} \\
-\frac{1}{\sqrt{ 2 }} & \frac{1}{\sqrt{ 2 }}
\end{bmatrix}\implies x=\begin{bmatrix}
\frac{1}{\sqrt{ 2 }} & \frac{1}{\sqrt{ 2 }} \\
-\frac{1}{\sqrt{ 2 }} & \frac{1}{\sqrt{ 2 }}
\end{bmatrix}^{-1}y
$$

Y la factorización $Q(y)=3y_{1}^{2}+7y_{2}^{2}$.

La gráfica de $Q(x)$ es la siguiente:

# Ejemplo

Sea $Q(x)=x_{1}^{2}-8x_{1}x_{2}-5x_{2}^{2}$, Realice un cambio de variable que transforma la forma cuadrática $Q$ a una sin productos cruzados

Entonces:

$$
A=\begin{bmatrix}
1 & -4 \\
-4 & -5
\end{bmatrix}
$$

Descubir $P$:

Valores propios:

$$
\det A-\lambda I=(1-\lambda)(-5-\lambda)-16\implies\lambda=\begin{cases}
\lambda_{1}=-7 \\
\lambda_{2}=3
\end{cases}
$$

Ahora se tendrá la forma:

$$
Q(x)=y^{T}\begin{bmatrix}
-7 & 0 \\
0 & 3
\end{bmatrix}y
$$

Los vectores propios son:

$$
v_{1}=\begin{bmatrix}
1 \\
2
\end{bmatrix},v_{2}=\begin{bmatrix}
-2 \\
1
\end{bmatrix}
$$

Normalizados:

$$
u_{1}=\begin{bmatrix}
\frac{1}{\sqrt{ 5 }} \\
\frac{2}{\sqrt{ 5 }}
\end{bmatrix},u_{2}=\begin{bmatrix}
-\frac{2}{\sqrt{ 5 }} \\
\frac{1}{\sqrt{ 5 }}
\end{bmatrix}
$$

Entonces:

$$P=\begin{bmatrix}
\frac{1}{\sqrt{ 5 }}  & -\frac{2}{\sqrt{ 5 }}\\
\frac{2}{\sqrt{ 5 }} & \frac{1}{\sqrt{ 5 }}
\end{bmatrix}$$

Notar que para evaluar $Q(x)=Q(x)=y^{T}\begin{bmatrix}-7 & 0 \\0 & 3\end{bmatrix}y$, se tiene que evaluar el $y$ para $x$, dado que:
$$

y=P^{T}x

$$

