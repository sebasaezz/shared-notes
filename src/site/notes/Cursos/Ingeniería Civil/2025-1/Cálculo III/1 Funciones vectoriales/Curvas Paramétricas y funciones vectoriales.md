---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/curvas-parametricas-y-funciones-vectoriales/","tags":["I1MAT1630"]}
---

# Concepto
Líneas en cualquier dimensión definidas por el recorrido de un vector trazando un conjunto de puntos.
![Pasted image 20250311083131.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/1%20Funciones%20vectoriales/attachments/Pasted%20image%2020250311083131.png)
Las ecuaciones que definen cada coordenada del vector con respecto a un parámetro ($t$) se llaman ecuaciones paramétricas, es decir, se encuentran de la forma:
$x=f(t)$
$y=g(t)$
$z=h(t)$
# Ejemplo
## Ejemplo 1
Indique las ecuaciones paramétricas de la curva parametrizada:
$$
\vec{r}(t) = \begin{bmatrix}
2t \\
1-t
\end{bmatrix}
$$
Ecuaciones paramétricas:
$x=2t$
$y=1-t$
Describa la curva:
Se puede representar de la forma vectorial:
$$
\begin{bmatrix}
x \\
y
\end{bmatrix}=\begin{bmatrix}
2t \\
1-t
\end{bmatrix}=
\begin{bmatrix}
0 \\
1
\end{bmatrix}+t\begin{bmatrix}
2 \\
-1
\end{bmatrix}
$$
Entonces es una recta que pasa por $(0,1)$ y tiene como vector director a $\langle 2,-1 \rangle$.
## Ejemplo 2
Describa la curva:
$$
\vec{r}(t)=\sin (t) \hat{i}+\cos(t) \hat{j}-t\hat{k}
$$
Paramétricas:
$x=\sin t$
$y=\cos t$
$z=-t$
Espiral que va hacia abajo.
<iframe width='400' height='500' src='https://www.wolframcloud.com/obj/5521f214-10fd-44cc-acb6-ca1faf8f4beb' frameborder='0'></iframe>
## Ejemplo 3
Encuentre parametrización de la intersección de $x^{2}+y^{2}=1$ e $y+z=2$.
Es un cilindro y un plano.
La curva tiene que satisfacer las dos cosas al mismo tiempo. La solución está en parametrizar una variable, como $z$ o $x^{2}+y^{2}$ que se sabe que es un círculo.
$x=\cos t$
$y=\sin t$
$\implies z=2-\sin t$
Entonces:
$$
\vec{r}(t)=\langle \cos t,\sin t,2-\sin t \rangle 
$$
![Pasted image 20250311090501.png|800](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/1%20Funciones%20vectoriales/attachments/Pasted%20image%2020250311090501.png)