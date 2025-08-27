---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/2-dinamica-de-particulas/2-6-oscilador-armonico-vibracion-libre/movimiento-armonico-simple/","tags":["ExFIS1514"]}
---

# Concepto
Objeto que muestra un movimiento periódico, usualmente por un resorte.
# Definición
Considerando un bloque de masa $m$ unido a un resorte y sin roces. Se sabe que el sistema va a oscilar si se perturba el equilibrio.
La sumatoria de fuerza en $x$ será simplemente $-kx$, por la [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.1 Leyes de Newton/Ley de Hooke (fuerza elástica)\|Ley de Hooke (fuerza elástica)]], y esta será también la masa por la aceleración $\ddot{x}$.
$$
\sum_{}^{}F_{x}=ma_{x}\implies-kx=m\ddot{x}
$$
De aquí:

$$
\begin{align}
-kx(t) & =m\ddot{x}(t) \\
 0 & = m\ddot{x}+kx \\
 0& =\ddot{x}+\frac{k}{m}x
\end{align}
$$
Ahora, notando que $\frac{k}{m}$ será constante, se le asigna el nombre de frcuencia natural de la siguiente forma:
$$
\omega_{n}=\sqrt{ \frac{k}{m} }
$$
Así:
$$
\boxed{\ddot{x}+\omega^{2}_{n}x=0} 
$$

Esta es una [[Ecuaciónes diferenciales\|ecuación diferencial]], y encontrar una solución no es trivial. Unas de la soluciones a la ecuación está dada por funciones trigonométricas. Por ejemplo:
$$
x(t)=\sin\alpha t\implies \ddot{x}(t)=(-\alpha^{2})\sin\alpha t
$$
De aquí se concluye que $\omega^{2}=\alpha^{2}$.
Lo mismo pasa con coseno.
Se pueden intentar otras funciones, como la exponencial:
$$
x(t)=e^{\gamma t}\implies \ddot{x}(t)=\gamma^{2}e^{t}
$$
Esto no sirve ya que $\gamma^{2}$ siempre será positivo, y se necesita que sea negativo.
## Solución general
La solución _más general_ a la ecuación sería que:
$$
\begin{align}
 & x(t)=A\sin\alpha t+B\cos\alpha t \\
\implies & \ddot{x}(t)=-A\alpha^{2}\sin\alpha t-B\alpha^{2}\cos\alpha t
\end{align}
$$
$$
\ddot{x}(t)=\underbrace{ -\alpha^{2} }_{ -\omega^{2} }\underbrace{ (A\sin\alpha t+B\cos\alpha t) }_{ x(t) }
$$
	De aquí, una solución es que $\alpha=\omega_{n}=\sqrt{ \frac{k}{m} }$.
Ahora, $A$ y $B$ serán constantes que permitirán determinar las condiciones iniciales del sistema, ya que $\omega_{n}$ será constante.
La velocidad y la aceleración estarán dadas por las derivadas de la función posición considerando las condiciones iniciales:

$$
\begin{align} x & =A\sin\alpha t+B\cos\alpha t\\
v  =\dot{x} & =A\omega_{n}^{2}\cos\omega_{n}t-B\omega _{n}^{2}\sin\omega_{n}t \\
a  =\ddot{x} & =-A\omega_{n}^{2}\sin\omega_{n}t-B\omega_{n}^{2}\cos\omega_{n}t
\end{align}
$$
Ahora, se nota que si $t=0$, el término con seno de $x$ se anulará, y el de coseno será $1$. Así:
$$
\boxed{B=x_{0}} 
$$
Haciendo lo mismo en $t=0$ para $v$, se da que:
$$
v_{0}=A\omega_{n}\implies \boxed{A=\frac{v_{0}}{\omega_{n}}} 
$$
## Otra solución
Existe otra solución, en la que las situaciones iniciales están dadas por constantes $C$ y $\phi$.
$$
\boxed{x(t)=C\sin(\omega_{n}t+\phi)} 
$$
Esta función es completamente análoga a la anterior y se relaciona con la anterior de la siguiente forma:
- $A=C\cos \phi$
- $B=\sin \phi$
## Características del movimiento
### Frecuencia y periodo
Si se considera un periodo $\tau$, se puede considerar su relación con la frecuencia de la forma:
$$
\omega_{n}=\frac{2\pi}{\tau}\implies \tau=\frac{2\pi}{\omega_{n}}
$$
==Ambigüedad:== a $\omega_{n}$ usualmente se le llama "frecuencia natural", pero realmente no es la frecuencia del movimiento, sino su velocidad anguar. La frecuencia $f$ es $\tau^{-1}$. 
$$
f=\tau^{-1}=\frac{\omega_{n}}{2\pi}
$$
### Amplitud
Por la naturaleza de la función trigonométrica, se sabe que $C$ debe ser la amplitud del desplazamiento, eso es el desplazamiento máximo y mínimo que alcanza la partícula.
# Método energéticos
Considerando la energía total de un sistema de un carro que oscila con un resorte de constante $k$:
![Pasted image 20241021100913.png|350](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Din%C3%A1mica%20-%20FIS1514/2%20Din%C3%A1mica%20de%20part%C3%ADculas/2.6%20Oscilador%20arm%C3%B3nico%20(vibraci%C3%B3n%20libre)/attachments/Pasted%20image%2020241021100913.png)
$$
E=K+U=\frac{1}{2}mv^{2}+\frac{1}{2}kx^{2}
$$
Donde $U$ es la [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.5 Energía potencial/Energía potencial gravitacional y elástica#Energía potencial elástica\|energía potencial elástica]]
Se sabe que:
$$
x=C\sin(\omega_{n}t+\phi)\implies \dot{x}=C\omega_{n}\sin(\omega_{n}t+\phi)=v
$$
Ahora se puede escribir la energía como:
$$
E=\frac{1}{2}m(C\omega_{n}\sin(\omega_{n}t+\phi))^2+\frac{1}{2}k(C\sin(\omega_{n}t+\phi))^2
$$
Usando la [[Conocimientos/Matemática/Pure Mathematics/Structures (algebra)/Algebra/Trigonometría/Identidades trigonométricas#^25ecb8\|identidad pitagórica]] y simplificando considerando que $\omega_{n}^{2}=\frac{k}{m}$se puede llegar a que
$$
E=\frac{1}{2}kC^{2}
$$
## Volver a la ecuación de movimiento usando solo energía
Se sabe que la energía es constante, se ahí su derivada debe ser cero.
$$
E=K+U=\frac{1}{2}m\dot{x}^{2}+\frac{1}{2}kx^{2}
$$
$$
\begin{align}
0 & =\frac{d}{dt}(K+U) \\
0 & =m\dot{x}\ddot{x}+kx\dot{x} \\
0 & =m\ddot{x}+k\dot{x}
\end{align}
$$
Esta es la misma ecuación con la que se partió usando la segunda ley de newton.
# Péndulo simple
Se quiere obtener la ecuación de movimiento para el siguiente péndulo.
![Pasted image 20241021103028.png|200](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Din%C3%A1mica%20-%20FIS1514/2%20Din%C3%A1mica%20de%20part%C3%ADculas/2.6%20Oscilador%20arm%C3%B3nico%20(vibraci%C3%B3n%20libre)/attachments/Pasted%20image%2020241021103028.png)
$$
¿¿¿¿¿¿¿¿a=r\dot{\theta}^{2}=-r\omega_{n}^{2}??????????
$$
### Intento 1
Considerando la segunda ley de newton para el eje de la tensión:
$$
\sum_{}^{}F_{\hat{r}}= T-mg\cos \theta=ma
$$
#### Intento 2: energía
Se sabe que:
$$
E=K+U=\frac{1}{2}mv^{2}+mgh
$$
Sea $l=r$ el largo de la cuerda, entonces $h=l\cos \theta$
Como se mide desde arriba, se debe considerar como negativa. Ahora:
$$
E=\frac{1}{2}mv^{2}-mg(l-l\cos \theta)
$$
Ahora se puede escribir la velocidad en función de $l$, usando las nociones de velocidad en [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.3 Coordenadas polares y cilíndricas/Coordenadas polares y sus vectores unitarios\|coordenadas polares]], se tiene que:
$$
v=\dot{\theta}r\implies v=l\omega
$$
$$
E=\frac{1}{2}ml^{2}\omega^{2}-mg(l-l\cos \theta)
$$
Derivando con respecto al tiempo:
$$
ml^{2}\dot{\theta}\ddot{\theta}+mgl\sin (\theta)\dot{\theta}=0
$$
$$
l \ddot{\theta}+g\sin \theta=0
$$
$$
\implies \ddot{\theta}=-\frac{g}{l}\sin \theta
$$
Pero $\sin \theta$ se parece mucha a $\theta$ para ángulos pequeños. Ahora:
$$
\ddot{\theta}=-\omega^{2}\theta
$$

- [x] no entendi nada  [completion:: 2025-04-20]

# Ejemplo