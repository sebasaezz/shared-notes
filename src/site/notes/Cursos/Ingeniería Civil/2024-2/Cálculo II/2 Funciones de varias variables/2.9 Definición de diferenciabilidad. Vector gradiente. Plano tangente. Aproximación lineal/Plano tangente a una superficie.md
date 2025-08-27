---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-9-definicion-de-diferenciabilidad-vector-gradiente-plano-tangente-aproximacion-lineal/plano-tangente-a-una-superficie/","tags":["I3MAT1620"]}
---

# Definición

> [!theorem] plano tangente a una superficie
> Para $f$ y un punto $(a,b)\in \operatorname{Dom}f$, se tiene el siguiente plano tangente a ese punto:
> $$
> z=f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)+f(a,b)
> $$
> 
## Demostración
`\begin{proof}`
Considerar el producto cruz entre las dos derivadas para las dos direcciones y con este sacar un plano que sea tangente a un punto de una superficie.

Se quiere un plano tangente al punto $(a,b,f(a,b))$. Los vectores directores, como se vio en [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.9 Definición de diferenciabilidad. Vector gradiente. Plano tangente. Aproximación lineal/Rectas tangentes a una superficie\|Rectas tangentes a una superficie]], son
$$
\begin{align}
d_{1} & =\begin{bmatrix}
0 \\
1 \\
\frac{ \partial f }{ \partial y } \biggr\rvert_{(a,b)}^{} \\
\end{bmatrix} \\
d_{2} & =\begin{bmatrix}
1 \\
0 \\
\frac{ \partial f }{ \partial x } \biggr\rvert_{(a,b)}^{}
\end{bmatrix}
\end{align}
$$
El [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.2 Producto vectorial. Ecuaciones vectoriales de rectas y planos en el espacio/Producto cruz\|Producto cruz]] entre estos dos será:
$$
\vec{n}=d_{1}\times d_{2}=\begin{bmatrix}
\frac{ \partial f }{ \partial x } \biggr\rvert_{(a,b)}^{} \\
-\frac{ \partial f }{ \partial y } \biggr\rvert_{(a,b)}^{} \\
-1
\end{bmatrix}
$$
De aquí, considerando [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.2 Producto vectorial. Ecuaciones vectoriales de rectas y planos en el espacio/Planos en R3\|la ecuación vectorial de un plano]]:
$$
\vec{n}·(P-P_{0})=0
$$
$$
\begin{bmatrix}
f_{x}(a,b) \\
-f_{y}(a,b) \\
-1
\end{bmatrix}·
\begin{bmatrix}
x-a \\
y-b \\
z-f(a,b)
\end{bmatrix}=0
$$
$$
\boxed{z=f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)+f(a,b)} 
$$
De otra forma:
$$
z-z_{0}=f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)
$$
`\end{proof}`
# Ejemplo
## Ejemplo 1
Encuentre la ecuación del plano tangente en $(0,1)$
$$
f(x,y)=xe^{xy}
$$
Las derivadas parciales son:
$$
f_{x}(x,y)=e^{xy}+xye^{xy}\implies f_{x}(0,1)=1
$$
$$
f_{y}(x,y)=x^{2}e^{xy}\implies f_{y}(0,1)=0
$$
De aquí y aplicando la ecuación ya vista, se tiene el plano
$$
z=x
$$
## Ejemplo 2
Calcule el plano tangente al paraboloide elíptico $z=2x^{2}+y^{2}$ en $(1,1,3)$.
$$
\frac{ \partial z }{ \partial x } =4x \implies f_{x}(1,1)=4
$$
$$
\frac{ \partial z }{ \partial y } =2y \implies f_{y}(1,1)=2
$$
Ahora, el plano será:
$$
z-3=4(x-1)+2(y-1)
$$
$$
z=4x+2y-3
$$
