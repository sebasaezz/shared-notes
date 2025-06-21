---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/sistemas-de-ed-os/","tags":["ExMAT1640"]}
---

# Concepto

Si se tiene una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Ecuaciones diferenciales de orden superior\|EDO de orden superior]] dada por:

$$
y^{(n)}=f(x,y,y',\dots,y^{(n-1)}) \tag{1}
$$

Esta EDO se va a poder escribir como un sistema de ecuaciones dado por:

$$
\begin{cases}
y_{1}'=f_{1}(x,y_{1},y_{2},\dots,y_{n}) \\
y_{2}'=f_{2}(x,y_{1},y_{2},\dots,y_{n}) \\
\vdots \\
y_{n}'=f_{n}(x,y_{1},y_{2},\dots,y_{n})
\end{cases}\tag{2}
$$
{ #40be9a}


De hecho, definir lo siguiente en (1):

$$
\begin{align}
y_{1} & =y, &y_{2} & =y', & \dots &  ,&y_{n} & =y^{(n-1)}  
\end{align}
$$

Entonces (1) es equivalente a:

$$
\begin{cases}
y_{1}' =y_{2} \\
y_{2}' =y_{3} \\
\vdots \\
y_{n}'=f(x,y_{1},y_{2},\dots,y_{n})
\end{cases}
$$
Los [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de EDOs lineales homogéneos con coeficientes constantes\|Sistemas de EDOs lineales homogéneos con coeficientes constantes]] resultan prácticos de resolver.

# Existencia y unicidad

> [!theorem] Teorema de existencia y unicidad de un sistema de EDOs
> Sea un sistema como en [[#^40be9a|(2)]], con funciones $f_{1},f_{2},\dots,f_{n}$ y sus derivadas parciales $\frac{ \partial f_{1} }{ \partial y_{1} },\dots \frac{ \partial f_{1} }{ \partial y_{n} },\dots,\frac{ \partial f_{n} }{ \partial y_{1} },\dots \frac{ \partial f_{n} }{ \partial y_{n} }$ continuas en una región $\mathcal{R}$ del espacio $(x,y_{1},y_{2},\dots,y_{n})$. Si $(x_{0},a_{1},a_{2},\dots,a_{n})$ es un punto en $\mathcal{R}$, entonces el sistema tiene solución única $y_{1},y_{2},\dots,y_{n}$ que satisface:
> $$
> \begin{align}
> y_{1}(x_{0}) & =a_{1}, & y_{2}(x_{0}) & =a_{2}, & \dots & , & y_{n}(x_{0})=a_{n}
> \end{align}
> $$


# Ejemplo
$$
\begin{cases}
x' =& 3x+2y \\
y'= & -x
\end{cases}
$$

Esto es equivalente a decir:

$$
\frac{ d\vec{x} }{ dt }=\begin{bmatrix}
3 & 2 \\
-1 & 0
\end{bmatrix} \begin{bmatrix}
x \\
y'
\end{bmatrix}=\lambda \vec{x}
$$

Las soluciones del sistema serán:

$$
\begin{array}{}
\begin{bmatrix}
1 \\
-1 
\end{bmatrix}e^{t} & , & \begin{bmatrix}
2 \\
-1
\end{bmatrix}e^{2t}
\end{array}
$$

Resulta que estos vectores $\vec{v}$ son vectores propios, y se ponen en la forma:

$$
\vec{v}e^{\lambda t}
$$
