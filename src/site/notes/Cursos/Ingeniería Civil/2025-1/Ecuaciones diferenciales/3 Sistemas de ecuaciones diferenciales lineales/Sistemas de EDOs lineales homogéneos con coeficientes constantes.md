---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/sistemas-de-ed-os-lineales-homogeneos-con-coeficientes-constantes/","tags":["ExMAT1640"]}
---

# Concepto
Se tiene el sistema:
$$
\frac{ d\vec{x} }{ dt } =M\vec{x} \tag{1}
$$
Se aplica una idea similar a la de la ecuación característica en las [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Resolución de EDOs lineales homogéneas de orden superior con coeficientes constantes\|EDOs lineales con coeficientes cosntantes]].
# Solución

> [!theorem] Solución de un sistema lineal de dos EDOs homogéneas
> Si se tiene el sistema:
> $$
> \begin{cases}
> \frac{ \mathrm{d}x }{ \mathrm{d}t } =a_{1}(t)x+b_{1}(t)y \\
> \frac{ \mathrm{d}y }{ \mathrm{d}t } =a_{2}(t)x+b_{2}(t)y
> \end{cases}
> $$
> Si este tiene dos soluciones en un intervalo $I$:
> $$
> \begin{align}
> \begin{cases}
> x=x_{1}(t) \\
> y=y_{1}(t)
> \end{cases} &  & \begin{cases}
> x=x_{2}(t) \\
> y=y_{2}(t)
> \end{cases}
> \end{align}
> $$
> Entonces:
> $$
> \begin{cases}
> x=c_{1}x_{1}(t)+c_{2}x_{2}(t) \\
> y=c_{1}y_{1}(t)+c_{2}y_{2}(t)
> \end{cases}
> $$
> También es solución en $I$. Además, esta solución será general en el intervalo si
> $$
> W(t)=\begin{vmatrix}
> x_{1}(t) & x_{2}(t) \\
> y_{1}(t) & y_{2}(t)
> \end{vmatrix},
> $$
> no se anula en $I$.

# Método de valores propios
Se asume que existe una solución:
$$
\vec{x}(t)=\vec{v}e^{rt}
$$
Las $n$-derivada será:
$$
\frac{d^{n}\vec{x}}{dt^{n}}=r^{n}\vec{x}
$$
Pero solo importa la primera derivada, la cual se pue reemplazar en (1).
$$
\begin{align}
r\vec{x} & =M\vec{x} \\
(M-rI)\vec{x} & =0
\end{align}
$$
Recordar que:
$$
A\text{ es invertible}\iff \det A\neq 0
$$
Entonces se necesita que $M-rI$ no sea invertible. Ahora se llega a la ecuación característica:
$$
\det(M-rI)=0 \tag{2}
$$
Los $r$ válidos en (2) son [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Vectores propios, valores propios y espacio propio\|valores propios]] de $M$. Recordar la ecuación característica de álgebra lineal:

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



> [!definition] Ecuación característica
> Para una matriz $A$, donde $\lambda$ es un valor propio, la ecuación característica está dada por $Det(A-\lambda I)=0$

</div></div>
 


## Caso complejo
Sea $\gamma$ el valor propio de la solución, y tiene la forma $\alpha\pm\beta i$, este va a tener auto-vectores:
$$
\begin{array}{}
v=v_{1}\pm iv_{2}
\end{array}
$$
Las soluciones serán:
$$
\begin{align}
y_{1} & =\underbrace{ \frac{x+\bar{x}}{2} }_{ \operatorname{Re}x } & y_{2}=\underbrace{ \frac{x-\bar{x}}{2i} }_{ \operatorname{\operatorname{Im}}x }
\end{align}
$$
Esto es un teorema:

> [!theorem] linealidad y conjugación de soluciones complejas
> Si en un sistema de ecuaciones lineales $\vec{x}(t)$ de solución del sistema, entonces $\Re(\vec{x})$ y $\Im(\vec{x})$ también son soluciones linealmente independientes 

 
Para resolver esto, se puede tomar un vector $\vec{v}=\vec{p}+\vec{q}i$, y aplicando la [[Identidad de Euler\|Identidad de Euler]]:
$$
\begin{align}
x & =\mathrm{e}^{ \alpha+\beta i }(\vec{p}+\vec{q}i) \\
x & =(\vec{p}+\vec{q}i)\mathrm{e}^{ \alpha } (\cos\beta t+i\sin\beta t) \\
 x & =\mathrm{e}^{ \alpha }\left[ \vec{p}(\cos\beta t +i\sin\beta t) + \vec{q}(i\cos\beta t-\sin\beta t) \right] 
\end{align}
$$
De aquí, se aplica lo que se dijo antes, y:
$$
\begin{align}
\vec{x}_{1} & =\Re(\vec{x}) & \vec{x}_{2} & =\Im(\vec{x}) \\
\vec{x}_{1} & =\mathrm{e}^{ \alpha }(\vec{p}\cos\beta t -\vec{q}\sin\beta t) & \vec{x}_{2} & =\mathrm{e}^{ \alpha }(\vec{p}\sin\beta t+\vec{q}\cos\beta t)
\end{align}
$$
## Si faltan auto-vectores
Se encuentra el primero con $(M-rI)\vec{v}_{1}=0$. 
Se encuentra el segundo con $(M-rI)\vec{v}_{2}=\vec{v}_{1}$
$\vec{v}_{2}$ es un [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Forma canónica de Jordan\|vector generalizado]], y depende de $\vec{v}_{1}$ (no se puede ponderad)
Y así sucesivamente. La solución LI asociada a cada vector $v_{k}$:
$$
\begin{align}
x_{1}(t) & =\mathrm{e}^{ \lambda t }\vec{v}_{1} \\
x_{2}(t) & =t\mathrm{e}^{ \lambda t }\vec{v}_{1} +\mathrm{e}^{ \lambda t }\vec{v}_{2} \\
x_{3}(t) & =\frac{t^{2}}{2}\mathrm{e}^{ \lambda t }\vec{v}_{1}+t\mathrm{e}^{ \lambda t }\vec{v}_{2}+\mathrm{e}^{ \lambda t }\vec{v}_{3} \\
\dots \\
x_{k}(t) & =\sum_{i=1}^{k} \frac{t^{i-1}}{(i-1)!}\mathrm{e}^{ \lambda t }\vec{v}_{i}
\end{align}
$$
# Exponencial de una matriz
Los sistemas de coeficientes lineales se representan como:
$$
\frac{ \mathrm{d}\vec{x} }{ \mathrm{d}t }=M\vec{x} 
$$
Si se toma esto como una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Resolución de EDOs separables\|EDO separable]], entonces la solución simplemente es:
$$
\vec{x}=c_{1}\mathrm{e}^{ Mt }
$$

> [!definition] exponencial de una matriz
> $$
> \mathrm{e}^{ x }=\sum_{k=0}^{\infty} \frac{x^{k}}{k}\implies \mathrm{e}^{ M }=\sum_{k=0}^{\infty} \frac{M^{k}}{k}=I+M+\frac{1}{2}M^{2}+\dots
> $$

La matriz a la que se va allegar es una matriz fundamental. Ahora, las matrices fundamentales se pueden cambiar de base y llegar a otra matriz fundamental $\Phi$. Se va a cumplir lo siguiente:
$$
\mathrm{e}^{ Mt }·\Phi(0)=\Phi(t)
$$
o de otra forma:
$$
\mathrm{e}^{ Mt }=\Phi(t)·\Phi(0)^{-1}
$$
y $\Phi(0)$ sería la matriz de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Cambio de base\|Cambio de base]]. Esta en la propiedad principal de la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Matriz fundamental de un sistema de EDOs\|Matriz fundamental de un sistema de EDOs]].
# Ejemplo
## Ejemplo 1
Resolver el sistema:
$$
\begin{cases}
x'  =y \\
y'=x
\end{cases}
$$
Esto es lo mismo que decir:
$$
\frac{ d\vec{x} }{ dt } =\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
x \\
y
\end{bmatrix}
$$
La ecuación característica será:
$$
\det\left(\begin{bmatrix}
0 & 1 \\
1  & 0
\end{bmatrix}-\begin{bmatrix}
r & 0 \\
0 & r
\end{bmatrix}\right)=\det  \begin{bmatrix}
r & 1 \\
1 & r
\end{bmatrix}  =r^{2}-1=0
$$
Entonces $r_{1,2}=1,-1$.
Como $\vec{v}$ son vectores propios, se debe cumplir que:
$$
Mv_{1}=v_{1}
$$
$$
\begin{align}
Mv_{2} & =-v_{2} \\
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
1 \\
-1
\end{bmatrix} & =\begin{bmatrix}
-1 \\
1
\end{bmatrix}=-v_{2}
\end{align}
$$
$$
\begin{array}{}
\vec{v}_{1}=\begin{bmatrix}
1 \\
1
\end{bmatrix} & \vec{v}_{2}=\begin{bmatrix}
1 \\
-1
\end{bmatrix}
\end{array}
$$
Entonces la solución es:
$$
\vec{x}(t)=c_{1}\begin{bmatrix}
1 \\
1
\end{bmatrix}e^{t}+c_{2}\begin{bmatrix}
1 \\
-1
\end{bmatrix}e^{-t}:c_{1},c_{2}\in\mathbb{R}
$$

> [!quote]
> Se puedes hacer 5 flexiones, puedes hacer una dominada, si puedes hacer 5 dominadas... Ustedes están haciendo flexiones con rodillas, y los estoy ayudando, y con esta mentalidad van a pasar el curso en 3 patadas.
> 
> _Marcos Canedo (2025)_

## Ejemplo 2
$$
\begin{cases}
x' & =3y+4z \\
y' & =6z \\
z' & =0
\end{cases}
$$
Esto es equivalente a:
$$
\begin{align}
\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix} & =\begin{bmatrix}
0 & 3 & 4 \\
0 & 0 & 6 \\
0 & 0 & 0
\end{bmatrix}\begin{bmatrix}
x \\
y \\
z
\end{bmatrix} \\
\vec{x}' & =M\vec{x}
\end{align}
$$
Entonces la solución es:
$$
\vec{x}=\vec{c}_{1}\mathrm{e}^{ \begin{bmatrix}
0 & 3 & 4 \\
0 & 0 & 6 \\
 0 & 0 & 0
\end{bmatrix} t}
$$
Se nota que:
$$
M^{2}=\begin{bmatrix}
0 & 0 & 18 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$
Y que:
$$
M^{3}=\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$
Entonces:
$$
\mathrm{e}^{ Mt }=\sum_{k=0}^{2} \frac{(Mt)^{k}}{k!}
$$
Como todas las demás exponentes se cancelan:
$$
\begin{align}
\mathrm{e}^{ Mt } & =\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}+\begin{bmatrix}
0 & 3t & 4t \\
0 & 0 & 6t \\
0 & 0 & 0
\end{bmatrix}+\frac{1}{2}\begin{bmatrix}
0 & 0 & 18t^{2} \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix} \\
 & =\begin{bmatrix}
1 & 3t & 4t+9t^{2} \\
0 & 1 & 6t \\
0 & 0 & 1
\end{bmatrix}
\end{align}
$$
