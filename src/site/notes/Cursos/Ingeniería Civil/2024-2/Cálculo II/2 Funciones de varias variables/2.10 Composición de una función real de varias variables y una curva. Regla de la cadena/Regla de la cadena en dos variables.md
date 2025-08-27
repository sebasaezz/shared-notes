---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-10-composicion-de-una-funcion-real-de-varias-variables-y-una-curva-regla-de-la-cadena/regla-de-la-cadena-en-dos-variables/","tags":["I3MAT1620"]}
---

# Primer caso
con $z=f(x,y)$, una función derivable, y $x=g(t)$ e $y=h(t)$, entonces se tiene $z=f(g(t),h(t))$.
Notar que $f$ es una función de UNA VARIABLE, $t$.
Entonces se cumple que:
$$
\frac{ dz }{ dt } =\frac{ \partial z }{ \partial x } \frac{ dx }{ dt } +\frac{ \partial z }{ \partial y } \frac{ dy }{ dt } 
$$
## Ejemplo
$$
f(x,y)=3x^{2}y
$$
Sea $x=t^{2}$ e $y=3t+\sin t$

Entonces se tiene la función $f(t)=3t^{2}(3t+\sin t)$

Calculando las derivadas parciales:
- $\frac{ \partial f }{ \partial x }=6xy$
- $\frac{ \partial f }{ \partial y }=3x^{2}$
- $\frac{ d x }{ d t }=2x$
- $\frac{ dy }{ dt }=3+\cos t$
Así:
$$
\frac{ df }{ dt } =\frac{ \partial f }{ \partial x } \frac{ dx }{ dt } +\frac{ \partial f }{ \partial y } \frac{ dy }{ dt } =3xy·2x+3x^{2}·(3+\cos t)
$$
# Caso 2
$z=f(x,y)$
- $x=g(t,s)$
- $y=h(s,t)$

Entonces, como ahora la función si es de dos variables ($s$ y $t$), se tienen derivadas parciales.
$$
\frac{ \partial z }{ \partial s } =\frac{ \partial z }{ \partial x } \frac{ \partial x }{ \partial s } +\frac{ \partial z }{ \partial y } \frac{ \partial y }{ \partial s } 
$$
$$
\frac{ \partial z }{ \partial t } =\frac{ \partial z }{ \partial x } \frac{ \partial x }{ \partial t } +\frac{ \partial z }{ \partial y } \frac{ \partial y }{ \partial t } 
$$
# Forma general
Ahora una función de $n$ variables, donde cada otra función depende de $m$ variables. Es decir:
- $z=f(x_{1},x_{2},\dots,x_{n})$
- $x_{j}=g_{j}(t_{1},t_{2},\dots,t_{m})$
- Entonces $f(t_{1},t_{2},\dots,t_{m})=f(g_{1}(t_{1},t_{2},\dots,t_{m})\cdots)$
Se cumple:
$$
\frac{ \partial z }{ \partial t_{i} } =\frac{ \partial z }{ \partial x_{1} } \frac{ \partial x_{1} }{ \partial t_{1} }+\frac{ \partial z }{ \partial x_{2} }\frac{ \partial x_{2} }{ \partial t_{i} }   \dots+\frac{ \partial z }{ \partial x_{n} }\frac{ \partial x_{n} }{ \partial t_{i} }  
$$
# Ejemplo
Sea $W(s,t)=F(u(s,t),v(s,t))$. $u$ y $v$ son derivables.
$$
\begin{align}
u(1,0) & =2 & v(1,0) & =3 \\
u_{s}(1,0) & =-2 &v_{s}(1,0) & =5 \\
u_{t}(1,0) & =6 &v_{t}(1,0) & =4 \\
  F_{u}(2,3) & =-1 & F_{v}(2,3) & =10
\end{align}
$$
Determine $W_{s}(1,0)$ y $W_{t}(1,0)$
$$
W_{s}=F_{s}=\frac{ \partial F }{ \partial s } =\frac{ \partial F }{ \partial u } \biggr\rvert_{(2,3)}^{}\frac{ \partial u }{ \partial s }\biggr\rvert_{(1,0)}^{}+\frac{ \partial F }{ \partial v }\biggr\rvert_{(2,3)}^{} \frac{ \partial v }{ \partial s } \biggr\rvert_{(1,0)}^{}
$$
Esto es lo mismo que decir:
$$
W_{s}(1,0)=F_{s}(u(1,0),v(1,0))=F_{s}(2,3)
$$
