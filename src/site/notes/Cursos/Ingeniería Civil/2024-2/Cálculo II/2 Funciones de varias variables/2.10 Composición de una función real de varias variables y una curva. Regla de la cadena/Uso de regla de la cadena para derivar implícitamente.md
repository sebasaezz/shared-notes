---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-10-composicion-de-una-funcion-real-de-varias-variables-y-una-curva-regla-de-la-cadena/uso-de-regla-de-la-cadena-para-derivar-implicitamente/","tags":["I3MAT1620"]}
---

Lo que antes era una ecuación, por ejemplo $x^{2}+y^{2}=0$, se [[Cursos/Ingeniería Civil/2024-1/Cálculo I/2 La derivada/Derivación implícita\|derivaba implícitamente]] ahora va a ser considerada como una función de dos variables $F(x,y)=x^{2}+y^{2}$ igualada a cero.
Digamos que queremos derivar con respecto a $x$, es decir, encontrar $\frac{ dy }{ dx }$. Se debe considerar a las dos variables de la función como funciones de $x$. Es decir $F(x,y)=F(x(x),y(x))$.
Utilizando la [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.10 Composición de una función real de varias variables y una curva. Regla de la cadena/Regla de la cadena en dos variables\|Regla de la cadena en dos variables]]:
$$
\begin{align}
 &  &  \frac{ dF }{ dx }  =0 & =\frac{ \partial F }{ \partial x }\cancelto{ 1 }{  \frac{ dx }{ dx }  } +\frac{ \partial F }{ \partial y } \frac{ dy }{ dx }=0   &  &  &  & \\
\implies &  &  \frac{ dy }{ dx } & =-\frac{\frac{ \partial F }{ \partial x }}{\frac{ \partial F }{ \partial y } }=-\frac{F_{x}}{F_{y}}
\end{align}
$$
# En más de dos variables
Sea, por ejemplo:
$$
F(x,y,z)=3xyz+\sin(xz)=0
$$
Se quiere encontrar $\frac{ \partial z }{ \partial x }$ (derivar implícitamente respecto a x), para esto se deben considerar todas las variables dependientes de $x$. Es decir: $F(x(x),y,z(x))$, donde $y$ es una constante.
Aplicando regla de la cadena:
$$
\frac{ \partial F }{ \partial x } =0=\frac{ \partial F }{ \partial x }\cancelto{ 1 }{  \frac{ \partial x }{ \partial x } } +\frac{ \partial F }{ \partial y } \cancelto{ 0 }{ \frac{ \partial y }{ \partial x } } +\frac{ \partial F }{ \partial z } \frac{ \partial z }{ \partial x } 
$$
Es lo mismo que decir:
$$
F_{x}+F_{z} \frac{ \partial z }{ \partial x } =0
$$
$$
\frac{ \partial z }{ \partial x } =-\frac{F_{x}}{F_{z}}
$$


# Ejemplo
## Ejemplo 1
Se quiere encontrar $\frac{ dy }{ dx }$ en la ecuación:
$$
3\sin (yx)-e^{xy}=2x
$$
Se considera la función $F(x,y)=3\sin(xy)-e^{xy}-2x=0$
Ahora:
$$
F_{x}=3y\cos(yx)-ye^{xy}-2
$$
$$
F_{y}=3x\cos(yx)-xe^{xy}
$$
Así:
$$
\frac{ dy }{ dx } =- \frac{F_{x}}{F_{y}}=- \frac{3y\cos(yx)-ye^{xy}-2}{3x\cos(yx)-xe^{xy}}
$$
