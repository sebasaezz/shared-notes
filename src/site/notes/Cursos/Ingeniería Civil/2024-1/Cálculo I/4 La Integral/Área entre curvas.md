---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/area-entre-curvas/","tags":["ExMAT1610"]}
---

# Para funciones con un orden en un intervalo

Se quiere calcular el siguiente área entre $f$ y $g$ en $[a,b]$ tales que $f(x)>g(x) \forall x \in [a,b]$. 

![Pasted image 20240619122152.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/4%20La%20Integral/attachments/Pasted%20image%2020240619122152.png)

Entonces se tendrá la suma de Riemann:

$$
\begin{align}
A & =\lim_{ n \to \infty } \sum_{i=1}^{n}(f(x_{i})-g(x_{i})\Delta x) \\
 & =\int_{a}^{b} f(x)-g(x) \, dx 
\end{align}
$$

> [!theorem] área entre curvas con orden definido para un intervalo
> Sea $f$ y $g$ funciones continuas y $f(x)\geq g(x) \forall x \in[a,b]$, entonces el área entre $a$ y $b$ es:
>$$
>\int_{a}^{b} f(x)-g(x) \, dx 
>$$

# Para funciones sin orden definido en un intervalo

Para funciones tale como:

![Pasted image 20240619124149.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/4%20La%20Integral/attachments/Pasted%20image%2020240619124149.png)

Se notará que si se aplica lo anterior, el área naranja quedará negativa, y el área azul positiva.

Si se aplica valor absoluto a lo anterior, se calcularía el área total.

> [!theorem] área entre curvas
> Sea $f$ y $g$ funciones continuas, entonces el área entre $a$ y $b$ es:
>$$
>\int_{a}^{b} |f(x)-g(x)| \, dx 
>$$

# Para funciones en la forma $x=f(y)$

Simplemente cambiar $x$ por $y$ (no es implícita).

# Ejemplo
## Ejemplo 1 (con orden)

Calcular el área entre las parábolas $y=x^{2}$ e $y=2x-x^{2}$.

No dan intervalos, así que hay que buscar puntos de intersección.

$$
x^{2}=2x-x^{2}\implies x=\begin{cases}
x_{1}=0\implies y=0 \\
x_{2}=1 \implies y=1
\end{cases}
$$

Se cumplirá que $2x-x^{2}\geq x^{2}:\forall x \in[0,1]$ y exclusivamente en ese intervalo, ya que no hay más intersecciones. Así esta será la única área calculable.

Finalmente:

$$
\begin{align}
A & =\int_{0}^{1} 2x-x^{2}-x^{2} \, dx  \\
 & =\left[ x^{2}-\frac{2}{3}x^{3} \right]^{1}_{0} \\
 & =\frac{1}{3}u^{2}
\end{align}
$$

![Pasted image 20240619130018.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/4%20La%20Integral/attachments/Pasted%20image%2020240619130018.png)

## Ejemplo 2 (sin orden)

Calcular el área entre las curvas $y=\sin x$ e $y=\cos x$, para $x \in \left[ 0, \frac{\pi}{2} \right]$.

Evaluar el valor absoluto:

$$
|\cos x-\sin x|=\begin{cases}
\cos x-\sin x & , & 0\leq x\leq \frac{\pi}{4} \\
\sin x -\cos x & , & \frac{\pi}{4}<x\leq \frac{\pi}{2}
\end{cases}
$$

Ahora:

$$
\begin{align}
A & =\int_{0}^{\frac{\pi}{2}} |\cos x-\sin x| \, dx  \\
 & =\int_{0}^{\frac{\pi}{4}} \cos x-\sin x \, dx +\int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \sin x-\cos x \, dx  \\
 & =[\sin x]^{\pi/4}_{0}+[\cos x]^{\pi/4}_{0}-[\cos x]^{\pi/2}_{\pi/4}-[\sin x]^{\pi/2}_{\pi/4} \\
 & = (2\sqrt{ 2 }-2)u^{2}
\end{align}
$$
## Ejemplo 3 ($x=f(y)$)

Calcular área entre las rectas $y=x-1$ y $y^{2}=2x+6$

Se pone en función de $y$:

$$
\begin{cases}
y=x-1 & \implies & x=y+1 & =f(y) \\
y^{2}=2x+6 & \implies & x=\frac{1}{2}y^{2}-3 & =g(y)
\end{cases}
$$

Se debe evaluar qué función está más a la derecha, esto se logra evaluando un punto en el intervalo de intersección.

Puntos de intersección:

$$
y+1=\frac{1}{2}y^{2}-3\implies y=\begin{cases}
y_{1}=-2 \\
y_{2}=4
\end{cases}
$$

Evaluando en $0$, $f(0)=1\leq g(0)=-3$.

$$
\begin{align}
A & =\int_{-2}^{4} |y+1-\frac{1}{2}y^{2}-3| \, dy \\
 & =18
\end{align}
$$
