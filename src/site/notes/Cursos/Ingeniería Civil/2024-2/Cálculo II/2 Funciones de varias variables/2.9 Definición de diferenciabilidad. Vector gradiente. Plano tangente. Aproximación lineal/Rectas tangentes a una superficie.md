---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-9-definicion-de-diferenciabilidad-vector-gradiente-plano-tangente-aproximacion-lineal/rectas-tangentes-a-una-superficie/","tags":["I3MAT1620"]}
---

# Concepto
## Pendiente de una recta en el plano
Si una recta en $\mathbb{R}^{2}$ tiene pendiente $m$, se puede decir que su dirección es $(1,m)$.

# Definición
# Ejemplo
Encuentre ecuaciones paramétricas de la tangente a la elipse $4x^{2}+2y^{2}+z^{2}=16$ en la intersección del plano $y=2$ para $(1,2,2)$:
Para $y=2$, se tiene el plano $4x^{2}+z^{2}=18$.
La interpretación de la pendiente será dada por:
$$
d=\left( 1,0,\frac{ \partial z }{ \partial x } \biggr\rvert_{(1,2,2)}^{} \right)
$$
$$
\begin{align}
  & &  8x+2z·\frac{ \partial z }{ \partial x }  & =0 \\
 &  & \frac{ \partial z }{ \partial x }  & =-\frac{4x}{z}
 &  &  \\
\implies &  & \frac{ \partial z }{ \partial x } \biggr\rvert_{(1,2,2)}^{} & =-2\end{align}

$$
De aquí se interpreta el vector director como:
$$
d=(1,0,-2)
$$
y el posición es el punto, $p=(1,2,2)$.
Así, la recta es:
$$
\begin{bmatrix}
1 \\
2 \\
2
\end{bmatrix}+\begin{bmatrix}
1 \\
0 \\
-2 
\end{bmatrix}\lambda=\begin{cases}
x=1+\lambda \\
y=2 \\
z=2-2\lambda
\end{cases}:\lambda \in\mathbb{R}
$$
<iframe width='500' height='500' src='https://www.wolframcloud.com/obj/cf0c6411-a334-41c8-bb07-83483df01707' frameborder='0'></iframe>
