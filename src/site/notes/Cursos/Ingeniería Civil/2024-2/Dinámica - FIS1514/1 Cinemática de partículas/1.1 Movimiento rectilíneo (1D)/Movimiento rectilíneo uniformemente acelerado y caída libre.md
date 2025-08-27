---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/1-cinematica-de-particulas/1-1-movimiento-rectilineo-1-d/movimiento-rectilineo-uniformemente-acelerado-y-caida-libre/","tags":["ExFIS1514"]}
---


Aquel movimiento donde la velocidad no se mantiene constante, sino incrementa linealmente, la pendiente de la función que representa la velocidad es conocida como aceleración.

# Velocidad

Análogo al comportamiento de la posición en un [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.1 Movimiento rectilíneo (1D)/Movimiento rectilíneo uniforme\|MUR]], se tiene que la velocidad para un instante de tiempo se define como:

$$
\vec{v}(t)=\vec{v}_{0}+\vec{a}t \tag{1}
$$
{ #1917fb}


# Posición

La función [[Cursos/Ingeniería Civil/2025-2/Dinámica de Sistemas Mecánicos/1 Cinemática/Distancia, posición, desplazamiento y trayectoria\|posición]] (trayectoria), se puede obtener interpretar como la acumulación de velocidad en el tiempo (integral). O también, como la velocidad es la derivada de la función posición, entonces la posición será la integral de la función velocidad. Así:

$$
\begin{align}
&&\vec{v}(t)&=\frac{dx}{dt}  &  \\
&&\implies dx&=\vec{v}(t)dt & 
\end{align}
$$

Integrando para un intervalo desde $x=x_{0}$ en $t=0$:

$$
\begin{align}
&&\int_{x_{0}}^{x}  \, dx&=\int_{0}^{t} \vec{v}_{0}+\vec{a}t \, dx \\
&&x-x_{0}&=\vec{v}_{0}t+\frac{1}{2}\vec{a}t^{2} \\
 \implies&&x(t)&=x_{0}+\vec{v}_{0}t+\frac{1}{2}\vec{a}t^{2} & 
\end{align}
$$

Finalmente, la ecuación de la posición en un movimiento rectilineo uniformemente acelerado será:

$$
x=x_{0}+v_{0}t+\frac{1}{2}at^{2} \tag{2}
$$
{ #5a15d1}


Finalmente, lo que se tendrá es una parábola. La concavidad de la parábola dependerá de la aceleración. Ahora, si se quiere buscar un $t$ cualquiera dado un $x$ y el resto de variables, se tendrá que utilizar la fórmula cuadrática:

![Pasted image 20240812082146.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Din%C3%A1mica%20-%20FIS1514/1%20Cinem%C3%A1tica%20de%20part%C3%ADculas/1.1%20Movimiento%20rectil%C3%ADneo%20(1D)/attachments/Pasted%20image%2020240812082146.png)

$$
\begin{align}
 &  & 0 & =\frac{1}{2}\vec{a}t^{2}+\vec{v}_{0}t+(x_{0}-x_{f}) &  &  \\
 &  & 0 & =\frac{1}{2}\vec{a}t^{2}+\vec{v}_{0}t-\Delta x &  &  \\
 & \implies & t & = \frac{-\vec{v}_{0}\pm \sqrt{ \vec{v}_{0}^{2}+2\vec{a}\Delta x }}{\vec{a}} &  &  & 
\end{align}
$$

Notar como se tendrán dos puntos en los que se llega al mismo tiempo. Esto se cumple dado que en un movimiento retardado o desacelerado, se logrará la misma posición dos veces en el tiempo (con velocidades opuestas).

Para otros movimientos siempre se tendrá que considerar puntos donde el tiempo sea positivo.

# Caída libre

Se tiene una situación muy parecida, solo que ahora la velocidad inicial siempre será 0, y la aceleración será la [[Aceleración de gravedad\|Aceleración de gravedad]] de la tierra ($g$).

## Tiempo hasta tocar el suelo

Esto significa que solo se alcanzará la misma posición una vez en el tiempo.

Reemplazando en la ecuación anterior con $v_{0}=0$:

Además, por convención se considera que la posición final es el 0, y la posición inicial es $h$.

$$
\begin{align}
0 & = \frac{1}{2}\vec{g}t^{2}+\cancel{ \vec{v}_{0}t }+h \\
0 & = \frac{1}{2}\vec{g}t^{2}-\Delta x \\
t & =\sqrt{ \frac{2\Delta x}{\vec{g}} }
\end{align}
$$

Realmente, como el objeto bajó, $\Delta x<0$, pero $|\vec{g}|<0$ entonces se podrán considerar los dos valores como positivos.

Finalmente, como en una caída la diferencia de posiciones hasta el suelo se denomina altura ($h$):

$$
\boxed{t=\sqrt{ \frac{2h}{g} }} 
$$
# Lanzamiento vertical

Si se lanza una partícula de forma vertical hacia arriba, hay tres incógnitas que se pueden pedir usualmente. La altura máxima ($h$), el tiempo en el que la partícula volverá al suelo y el tiempo hasta alcanzar la altura máxima.

Se mantendrán las definiciones anteriores, solo que ahora la posición inicial será $x_{0}=0$ (antes era $h$)

Notar que también a la altura se le suele denominar $y$.

$$
h(t)=y(t)=-\frac{1}{2}gt^{2}+v_{0}t+\cancel{ x_{0} }
$$

Notar que la aceleración de gravedad $g$ so considera negativa.

## Tiempo a altura máxima $t_{max}$

La altura máxima se logra cuando la velocidad es igual $0$, esto se puede lograr [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Mínimos y máximos de una función, teorema de Fermat, teorema de valor extremo y puntos críticos\|derivando]] o utilizando la fórmula que dice que el vértice de una parábola dada por $ax^{2}+bx+c=0$ será $-\frac{b}{2a}$.

$$
t_{max}=\frac{v_{0}}{g}
$$
## Altura máxima $h_{max}$

Se puede reemplazar el valor ya descubierto del tiempo a altura máxima para lograr despejar esta altura:

$$
\begin{align} \\
h_{max} & =y(T) \\
h_{max} & =-\frac{g}{2} ·\frac{v_{0}^{2}}{g^{2}}+\frac{v_{0}^{2}}{g} \\
h_{max} & =\frac{v_{0}^{2}}{g}-\frac{v_{0}^{2}}{2g}=\frac{v_{0}^{2}}{2g}
\end{align}
$$
## Tiempo de vuelta

Sea $t_{v}$ el tiempo que se demora en volver a la misma altura, este se logra despejando la ecuación de posición igualada a 0:

$$
\begin{align}
&&0 & =v_{0}t-\frac{1}{2}gt^{2} &  &  \\
&&0 & =t\left( v_{0}-\frac{1}{2}gt \right) &  & t_{1}=0 \\
&&0 & =v_{0}-\frac{1}{2}gt \\
 & \implies &  t_{2}& =\frac{2v_{0}}{g}& 
\end{align}
$$
# Ecuación sin tiempo (itinerario)

Se puede despejar la siguiente ecuación:

$$
\boxed{2a(x-x_{0})=v^{2}-v_{0}^{2}} 
$$

Esto es simplemente reemplazar la [[#^1917fb|ecuación 1]] en la [[#^5a15d1|ecuación 2]]  