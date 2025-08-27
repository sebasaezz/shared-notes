---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/1-cinematica-de-particulas/1-1-movimiento-rectilineo-1-d/movimientos-donde-la-aceleracion-depende-del-tiempo/","tags":["ExFIS1514"]}
---

# Aceleración dependiendo del tiempo

Se la aceleración depende del tiempo, se deben integrar las siguientes ecuaciones para **despejar una función de velocidad**:

$$
a(t)=\frac{dv}{dt}\implies \int_{v_{0}}^{v} \, dv=\int_{t_{0}}^{t} a(t) \, dt\implies v(t)-v_{0}=\int_{t_{0}}^{t} a(t) \, dt 
$$

Primero se considera a la [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.1 Movimiento rectilíneo (1D)/Aceleración\|Aceleración]] como $\frac{dv}{dt}$, y al integrarla en $dt$ para los intervalos $v_{0}$ (usualmente 0) y $v$, se obtiene $v(t)-v_{0}$. Además así integrando la función de la aceleración.

Ahora con la función de velocidad se puede **despejar una función de desplazamiento**:

$$
	v(t)=\frac{dx}{dt}\implies \int_{x_{0}}^{x}  \, dx =\int_{t_{0}}^{t} v(t) \, dt \implies x(t)-x_{0}=\int_{t_{0}}^{t} v(t) \, dt
$$
## Ejemplo para aceleración constante

Ya se sabe la respuesta para los [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.1 Movimiento rectilíneo (1D)/Movimiento rectilíneo uniformemente acelerado y caída libre\|MRUA]], pero ahora se utilizará este método. Como es constante, se tiene que para todo $t$, $a(t)= a_{0}$.

$$
\begin{align}
v(t)-v_{0}&=\int_{t_{0}}^{t} a(t) \, dx  \\
v(t)-v_{0} & =a_{0}\int_{0}^{t}  \, dx  \\
v(t)-v_{0} & =a_{0}t \\
v(t) & =v_{0}+a_{0}t
\end{align}
$$

Ahora aplicando la siguiente ecuación:

$$
\begin{align}
x(t)-x_{0} & =\int_{0}^{t} (v_{0}+a_{0}t) \, dx  \\
x(t) & =x_{0}+a_{0}t+\frac{1}{2}a_{0}t^{2}
\end{align}
$$
# Cuando la aceleración depende de la velocidad

Si la aceleración depende de la velocidad, se debe partir expresando la función de aceleración de la siguiente forma:

$$
a(t)=\frac{dv}{dt}\implies dt=\frac{dv}{a(v)}
$$

Ahora se debe integrar:

$$
\begin{align}
 &  & \int_{t_{0}}^{t}  \, dt  & =\int_{v_{0}}^{v} \frac{dv}{a(t)} \, dt  \\
 & \implies & t-t_{0} & =\underbrace{ \int_{v_{0}}^{v} \frac{dv}{a(v)} \, dt }_{ \text{Función de velocidad} }  &  &  & 
\end{align}
$$

Esta parte de la ecuación que es una función de velocidad, en general no se puede invertir, y se obtiene una relación implícita ente $v$ y $t$.

Ahora, nuevamente se aplica la definición de la velocidad como $\frac{dx}{dt}$.

De la definición de aceleración se tiene que $a(v)=\frac{dv}{dt}\implies dt=\frac{dv}{a(v)}$

De aquí, aplicando este $dt$ a la definición de velocidad, se tiene:

$$
v=\frac{dx}{dt}=\frac{dx}{\frac{dv}{a(t)}}\implies dx=\frac{vdv}{a(t)}
$$

ahora se integra:

$$
\int_{x_{0}}^{x}  \, dx =\int_{v_{0}}^{v} \frac{vdv}{a(v)} \, dx \implies x-x_{0}=\int_{v_{0}}^{v} \frac{vdv}{a(v)} \, dx 
$$
# Cuando la aceleración depende de la posición

Se parte con el mismo concepto similar al anterior, partiendo con que $a(x)=\frac{dv}{dt}\implies dt=\frac{dv}{a(x)}$, reemplazando en la definición de velocidad:

$$
v=\frac{dx}{dt}=\frac{dx}{\frac{dv}{a(x)}}\implies vdv=a(x) dx
$$

Integrando

$$
\int_{v_{0}}^{v} v \, dv =\int_{x_{0}}^{x} a(x) \, dx \implies \boxed{\frac{1}{2}v^{2}-\frac{1}{2}v_{0}^{2}=\int_{x_{0}}^{x} a(x) \, dx } 
$$

Ahora se tiene una relación explícita de $v$ en términos de $x$, pero la relación inversa (de $x$ en términos de $v$) es implícita (cuesta mucho resolver).

Para resolver se asumirá que la velocidad es una función $f$. $v=f(x)$. Donde $f$ es una función que depende de $a(x)$.

$$
f(x)=\frac{dx}{dt}\implies \int_{t_{0}}^{t}  \, dt =\int_{x_{0}}^{x} \frac{dx}{f(x)}\implies t-t_{0}=\int_{x_{0}}^{x} \frac{dx}{f(x)} 
$$
