---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/4-transformada-de-laplace/transformada-de-laplace/","tags":["ExMAT1640"]}
---

# Concepto
Similar a la [[Transformada de Fourier\|Transformada de Fourier]]
# Definición

> [!definition]
> La transformada de Laplace se define como:
> $$
> \mathcal{L}\{ f(t) \}=\int_{0}^{\infty} f(t)·e^{-st} \, \mathrm{d}t 
> $$
> con $s \in\mathbb{C}$. 

# Propiedades

> [!theorem]
> La transformada de Laplace es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Transformaciones lineales\|transformación lineal]].

> [!theorem]
> Sea $f$ una función exponencialmente acotada, eso es que $\lvert f(t) \rvert\leq M\mathrm{e}^{ at }$, entonces $f$ tiene una transformada de Laplace definida $\mathcal{L}\{ f(t) \}$.

> [!theorem]
> Si existe transformada de Laplace para una función exponencialmente acotada $f$, entonces $\mathcal{L}\{ f \}$ decrece a cero cuando $s$ tiende a infinito.

# Transformadas notables
$$
\mathcal{L}\{ \mathrm{e}^{ at } \}=\frac{1}{s-a}
$$
$$
\mathcal{L}\{ t^{n} \}= \frac{n!}{s ^{n+1}}
$$
$$
\mathcal{L}\{ \cosh(at) \}=\frac{s}{s^{2}-a^{2}}
$$
$$
\mathcal{L}\{ \cos(at) \}=\frac{s}{s^{2}+a^{2}}
$$
## Transformada de $t^{a}$ y función gamma
La función $n!$ se generaliza en la [[Función gama\|Función gama]] ($\Gamma$), dada por:
$$
\Gamma(x)=\int_{0}^{\infty} \mathrm{e}^{ -t }t^{x-1} \, \mathrm{d}t =(x-1)!
$$
Esto es simplemente $\mathcal{L}\{ t^{x-1} \}$ con $s=1$.
Entonces $\Gamma$ cumple que:
$$
\Gamma(n)=(n-1)!:n\in\mathbb{N}
$$
## Transformada de una derivada
$$
\begin{align}
\mathcal{L}\{ f'(x) \} & =\int_{0}^{\infty} \mathrm{e}^{ -st } f'(t)  \, \mathrm{d}t  \\
 & = \cancelto{ -f(0) }{ \mathrm{e}^{ -st }f(t) \biggr\rvert_{0}^{\infty} }+ s\int_{0}^{\infty}\mathrm{e}^{ -st } f(t)  \, \mathrm{d}t  \\
 & =s\mathcal{L}\{ f \}-f(0)
\end{align}
$$
Esto se cumple entonces para una $f$ exponencialmente acotada por $M\mathrm{e}^{ ct }$. Entonces la transformada converge para $s>c$.
## Transformada de una integral
$$
\begin{align}
\mathcal{L}\left\{  \int_{0}^{t} f(\tau) \, \mathrm{d}\tau   \right\} & =\frac{1}{s}\mathcal{L}\{ f \}
\end{align}
$$
De otra forma, se va a tener:
$$
\int_{0}^{t} f(t) \, \mathrm{d}t =\mathcal{L}^{-1}\left\{  \frac{1}{s}\mathcal{L}\{ f \}  \right\}
$$
Esto es muy útil para [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/4 Transformada de Laplace/Resolver EDOs con la transformada de Laplace\|Resolver EDOs con la transformada de Laplace]], ya que si se tiene una función $\mathcal{L}\{ f \}=F$ que se quiere anti-transformar (para obtener $f$), entonces se tiene que:
$$
\mathcal{L}^{-1}\left\{  \frac{F}{s}  \right\}=\int_{0}^{t} \underbrace{ \mathcal{L}^{-1}\{ F \}  }_{ f }\, \mathrm{d}t 
$$
## Transformada de una función a trozos
Si una función se defina a trozos con una frontera $a$, por ejemplo:
$$
u_{a}(t)=\begin{cases}
u_{2}(t) ,t\geq a \\
u_{1}(t), t<a
\end{cases}
$$
Entonces se puede hacer lo siguiente:
$$
\mathcal{L}\{ u_{a}(t) \}=\int_{0}^{a} u_{1}(t) \mathrm{e}^{ -st } \, \mathrm{d}t + \int_{a}^{\infty} u_{2}(t)\mathrm{e}^{ -st } \, \mathrm{d}t  
$$
## Desplazamiento de una transformada
Transformar el producto de una función $f(t)$ tal que $\mathcal{L}\{ f (t)\}=F(s)$ con una función $\mathrm{e}^{ at }$, se interpreta como un desplazamiento de la transformada.
$$
\begin{align}
\mathcal{L}\{ \mathrm{e}^{ at }f(t) \} & =\int_{0}^{\infty} \mathrm{e}^{ -st }·(\mathrm{e}^{ at }f(t)) \, \mathrm{d}t \\
  & =\int_{0}^{\infty} \mathrm{e}^{ -(s-a)t }f(t) \, \mathrm{d}t \\
  & =F(s-a)
\end{align}
$$
Esto es muy útil para calcular antitransformadas, por ejemplo, si se quiere la siguiente antitransformada:
$$
\mathcal{L}^{-1}\left\{  \frac{k}{(s-a)^{2}+k^{2}}  \right\}
$$
Se puede considerar simplemente $\frac{k}{s^{2}+k^{2}}$, que es la transformada de $\sin kt$ y desplazarla.
$$
\mathcal{L}^{-1}\left\{  \frac{k}{(s-a)^{2}+k^{2}}  \right\}=\mathrm{e}^{ at }\sin kt
$$
## Derivada de una transformada y antitransformada de una derivada
Se tiene la siguiente identidad para $\mathcal{L}\{ f \}=F$
$$
F'=-\mathcal{L}\{ tF \}
$$
Implicando que:
$$
\boxed{\mathcal{L}^{-1}\{ F' \}=- \frac{\mathcal{L}^{-1}\{ F \}}{t}} 
$$
De otra forma:
# Ejemplo
## Ejemplo 1
Transforme la función $f(t)=1$.
$$
\begin{align}
\mathcal{L}\{ 1 \} & =\int_{0}^{\infty} \mathrm{e}^{-st} \, \mathrm{d}t \\
  & =\lim_{ k \to \infty } -\frac{1}{s}\mathrm{e}^{ -st }\biggr\rvert_{0}^{k} \\
 & =\lim_{ k \to \infty } -\frac{1}{s}\mathrm{e}^{ -st }+\frac{1}{s} \\
 &=\frac{1}{s} \text{  para } s>0
\end{align}
$$
## Ejemplo 2
Calcule $\mathcal{L}\{ t \}$
$$
\begin{align}
\mathcal{L}\{ t \} & =\int_{0}^{\infty} t\mathrm{e}^{ -st } \, \mathrm{d}t  \\
 & =\lim_{ t \to \infty } \left( \cancelto{ 0 }{ -\frac{1}{s}\mathrm{e}^{ -st }t } +\frac{1}{s}\int_{0}^{t} \mathrm{e}^{ -st } \, \mathrm{d}t \right)  \\
 & =\frac{1}{s^{2}}
\end{align}
$$
## Ejemplo 3
Calcule $\mathcal{L}\{ e^{at} \}$

$$
\begin{align}
\mathcal{L}\{ \mathrm{e}^{ at } \} & =\int_{0}^{\infty} 
\mathrm{e}^{ at }· \mathrm{e}^{ -st } \, \mathrm{d}t \\
 & =\int_{0}^{\infty} \mathrm{e}^{ (a-s)t } \, \mathrm{d}t \\
  & = \frac{1}{s-a}
\end{align}
$$
## Ejemplo 4
Calcule $\mathcal{L}\{ t\mathrm{e}^{ at } \}$.
$$
\begin{align}
\mathcal{L}\{ t\mathrm{e}^{ at } \} 
\end{align}
$$
sea $f(t)=t\mathrm{e}^{ at }$. Si se deriva se tiene $f'(t)=\mathrm{e}^{ at }+at\mathrm{e}^{ at }$.
$$
\begin{align}
\mathcal{L}\{ f' \} & =\frac{1}{s-a}+a\mathcal{L}\{ f \} \\
\text{por el teorema visto}\rightarrow & =\cancelto{ 0 }{ -f(0) }+s\mathcal{L}\{ f\} \\
 \frac{1}{s-a} & =(s-a)\mathcal{L}\{ f \} \\
\mathcal{L}\{ f \} & =\frac{1}{(s-a)^{2}}
\end{align}
$$
## Ejemplo 5
Calcule $\mathcal{L}\{ t\sin t \}$.
Sea $f(t\sin t)$ entonces $f'(t)=\sin t+t\cos t$ y $f''(t)=2\cos t-t\sin t$.
$$
\begin{align}
\mathcal{L}\{ f'' \} & =2 \frac{s}{s^{2}+1}-\mathcal{L}\{ f \} \\
 & =\cancelto{ 0 }{ -f'(0) }+s\mathcal{L}\{ f' \} \\
 & =s\left[ \cancelto{ 0 }{ -f(0) }+s\mathcal{L}\{ f \}\right]  \\
s^{2}\mathcal{L}\{ f \} & = \frac{2s}{s^{2}+1}-\mathcal{L}\{ f \} \\
 \mathcal{L}\{ f \} & =\frac{2s}{(s^{2}+1)^{2}}
\end{align}
$$
## Ejemplo 6
