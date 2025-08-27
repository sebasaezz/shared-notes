---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-11-derivadas-direccionales/derivadas-direccionales-y-vector-gradiente/","tags":["I3MAT1620"]}
---

# Concepto
# Definición

> [!definition] derivada direccional
> La derivada en la dirección de un vector $\hat{u}=(a,b)$
> $$
> D_{\hat{u}}f(x_{0},y_{0})=\frac{ \partial f }{ \partial \hat{u} } =\lim_{ h \to 0 } \frac{f(x_{0}+ha,y_{0}+hb)-f(x_{0},y_{0})}{h}
> $$
> La dirección además puede estar dado por un ángulo, donde:
> $$
> \hat{u}= \left< \cos\theta,\sin\theta \right> 
> $$
> 

Tomando esta definición, ahora es lógico pensar que las derivadas parciales normales con casos específicos de esto, donde $\hat{u}=\hat{i}$ para $\frac{ \partial z }{ \partial x }$ y $\hat{u}=\hat{j}$ para $\frac{ \partial z }{ \partial y }$.

Haciendo una demostración bien lógica, se puede llegar a partir de la definición anterior, que para la dirección $\hat{u}=(a,b)$, se va a tener:
$$
D_{\hat{u}}f(x_{0},y_{0})=f_{x}(x_{0},y_{0})a+f_{y}(x_{0},y_{0})b=
\underbrace{ \begin{bmatrix}
f_{x}(x_{0},y_{0}) \\
f_{y}(x_{0},y_{0})
\end{bmatrix} }_{ \nabla f(x_{0},y_{0}) }
·\begin{bmatrix}
a \\
b
\end{bmatrix}
$$
A este vector que multiplica a $\hat{u}$ se le denomina vector gradiente.
# Vector gradiente

vector gradiente
El vector gradiente para una función $f(x,y)$ se define como:
$$
\nabla f(x_{0},y_{0})=\left( \frac{ \partial f }{ \partial x }\biggr\rvert_{(x_{0},y_{0})}^{},\frac{ \partial f }{ \partial y } \biggr\rvert_{(x_{0},y_{0})}^{} \right)
$$
## Significado del vector gradiente
1. El vector gradiente es perpendicular a un punto en su curva de nivel.
## Uso del vector gradiente

> [!theorem] derivada direccional con vector gradiente
> Se cumple lo siguiente para una función $f$ diferenciable en $(x_{0},y_{0})$ para una dirección dada por el vector unitario $\vec{v}=(a,b)$:
> $$
> D_{\vec{v}}f(x_{0},y_{0}) = \nabla f(x_{0},y_{0})·\vec{v}=f_{x}(x_{0},y_{0})a+f_{y}(x_{0},y_{0})b
> $$
> Esto se puede generalizar para $\mathbb{R}^{n}\rightarrow\mathbb{R}$

De aquí se pueden sacar muchas conclusiones:
$$
\nabla f(P)·\vec{v}=\lvert \lvert \nabla f(P) \rvert \rvert  \cos\theta
$$
(recordando que $\vec{v}$ es unitario)

Notar que $\theta$ es el ángulo **entre** el gradiente y la dirección, no es el ángulo de la dirección con respecto al eje.

De aquí, considerando el dominio de $\cos\theta$:
- La derivada direccional es máxima si $\theta=0$. Esto es lo mismo que decir que $\vec{v}=\frac{\nabla f}{\lvert \lvert \nabla f \rvert \rvert}$.
- La derivada es mínima si $\theta=\pi$.
- La derivada es cero si $\theta=\pm \frac{\pi}{2}$
![Pasted image 20241103132647.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.11%20Derivadas%20direccionales/attachments/Pasted%20image%2020241103132647.png)
## Ejemplo 2