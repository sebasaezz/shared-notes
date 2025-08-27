---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-2-producto-vectorial-ecuaciones-vectoriales-de-rectas-y-planos-en-el-espacio/rectas-en-el-espacio-cartesiano/","tags":["I2MAT1620"]}
---

Dadas por ecuaciones paramétricas entre vectores. Existe un vector director y uno de posición.
El vector director estará ponderado por una variable $\lambda$. A medida que $\lambda$ varía, se terminará generando una recta.
Notar que una ecuación en la forma $Ax+By+C=0$ generará un plano. Esta es la forma cartesiana
# Forma vectorial
Ahora se pueden definir los dos vectores:
$$
\vec{p}=\begin{bmatrix}
a \\
b \\
c
\end{bmatrix},\vec{d}=\begin{bmatrix}
a-d \\
b-e \\
c-f
\end{bmatrix}
$$
Definiendo la ecuación:
$$
(x,y,z)=\vec{p}+\lambda \vec{d}=\begin{bmatrix}
a \\
b \\
c
\end{bmatrix}+\lambda \begin{bmatrix}
a-d \\
b-e \\
c-f
\end{bmatrix}
$$
Esto es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Ecuación vectorial\|Ecuación vectorial]].
# Forma paramétrica
La ecuación vectorial se puede dividir en varias ecuaciones paramétricas:
$$
(x,y,z)=\begin{cases}
x & = & a & + & \lambda(a-d) \\
y & = & b & + & \lambda(b-e) \\
z & =  &c & + & \lambda(c-f)   
\end{cases}
$$
Estas dos son equivalentes, y darán una recta que pasa por el punto $(a,b,c)$ y el punto $(d,e,f)$.
