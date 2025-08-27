---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/1-cinematica-de-particulas/1-1-movimiento-rectilineo-1-d/velocidad/","tags":["ExFIS1514"]}
---

# Concepto
Vector que define el cambio en posición y la razón en la que está sucediendo con el tiempo. 
# Definición
## Velocidad promedio $\bar{v}$
Se puede obtener la velocidad como la diferencia de posición en una diferencia de tiempo:
$$
\bar{v}=\frac{\Delta \vec{x}}{\Delta t}
$$
## Velocidad constante

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/1-cinematica-de-particulas/1-1-movimiento-rectilineo-1-d/movimiento-rectilineo-uniforme/#f58d7b" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# MUR

</div>


Para calcular el desplazamiento entre un $x_{0}$ y un $x_{f}=x$, se considera a $x_{0}$ como posición inicial, eso es $t=0$, así: 

</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/1-cinematica-de-particulas/1-1-movimiento-rectilineo-1-d/movimiento-rectilineo-uniforme/#e8dca8" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# MUR

</div>


$
\begin{align}
&&\vec{v}&=\frac{x(t)-x_{0}}{t-0}&& \\
\implies&& \vec{v}t&=x(t)-x_{0} \\
\implies&& x(t)&=x_{0}+\vec{v}t
\end{align}
$

</div></div>

## Velocidad instantánea
Se puede tomar a la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/La derivada como una razón de cambio y aplicaciones\|velocidad como derivada]], así obteniendo la velocidad en un punto específico. Así la velocidad es la [[Conocimientos/Matemática/Pure Mathematics/Changes/Calculus/Derivadas/Pendiente en un punto de la función\|pendiente]] de la tangente a la trayectoria $x(t)$. 
$$
\vec{v}=\lim_{ t \to 0 } \frac{\Delta x}{\Delta t}=\frac{d}{dt}x(t)=\frac{dx}{dt}
$$
# Aceleración y gráfico de velocidad vs tiempo
De un gráfico de velocidad vs tiempo se puede obtener información de la aceleración, como la [[Derivadas\|derivada]] de la velocidad. Además se tendrá que el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/La integral definida\|área bajo la curva]] será el [[Cursos/Ingeniería Civil/2025-2/Dinámica de Sistemas Mecánicos/1 Cinemática/Distancia, posición, desplazamiento y trayectoria\|desplazamiento]].

![Pasted image 20240807103105.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Din%C3%A1mica%20-%20FIS1514/1%20Cinem%C3%A1tica%20de%20part%C3%ADculas/1.1%20Movimiento%20rectil%C3%ADneo%20(1D)/attachments/Pasted%20image%2020240807103105.png)
# Velocidad en 2 y 3 dimensiones
{ #260176}


Se mantiene la definición:
$$
\vec{v}=\frac{\Delta \vec{x}}{\Delta t}
$$
y siempre será tangente a la trayectoria.
Para derivar se tendrá que hacer la derivada por cada componente, considerando [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.2 Movimiento en dos y tres dimensiones/Vectores unitarios\|Vectores unitarios]]. Así, por ejemplo para $\mathbb{R}^{3}$:
$$
\begin{align}
\vec{v} & =\frac{d}{dt}(x \hat{i}+y\hat{j}+x\hat{k}) \\
 & =\frac{dx}{dt}\hat{i}+\cancel{ x\frac{d\hat{i}}{dt} }+\frac{dy}{dt}\hat{j}+\cancel{ y \frac{d\hat{j}}{dt} }+\frac{dz}{dt}\hat{k}+\cancel{ z \frac{d\hat{k}}{dt} } \\
 & =\frac{dx}{dt}\hat{i}+\frac{dy}{dt}\hat{j}+\frac{dz}{dt}\hat{k} \\
&=\dot{x}\hat{i}+\dot{y}\hat{j}+\dot{z}\hat{k}
\end{align}
$$

