---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/4-balance-en-maquinas/balance-de-entropia/","tags":["I2IIQ1003"]}
---


> [!important]
> La condición isoentrópica sucede solo cuando un proceso es adiabático y mecánicamente revesible

Si se tiene un proceso mecánicamente reversible, se sabe que:
$$
Q_{rev}=Tds
$$
Entonces se usa:
$$
Q_{\text{rev}}=\int_{A}^B T \, dS 
$$
Esta es el área bajo la curva de un gráfico T-S.
![Pasted image 20250425081533.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/4%20Balance%20en%20m%C3%A1quinas/attachments/Pasted%20image%2020250425081533.png)
De forma general:
$$
\frac{ dS }{ dt } =\frac{\dot{Q}}{T}+\sum_{k=1}^{n}\dot{m}_{k}{s}_{k}+\dot{S}_{\text{generada}}
$$
Todos los procesos generan entropía, y esto es lo que representa $\dot{S}_{\text{generada}}$.
- Es un estado de equilibrio, se tiene que $\frac{ dS }{ dt } =\dot{S}_{\text{generada}}=0$.
- Lo mismo en un sistema adiabático, cerrado y reversible.
- Para sistemas adiabáticos,  $\dot{Q}=0$.
- Para sistemas reversibles, $\dot{S}_{\text{generada}}=0$.
- Un sistema abierto y estacionario tiene $\frac{ dS }{ dt }=0$.
# Combinación primera y segunda ley
Se puede llegar a que:
$$
dU=T\,dS+P\,dV
$$
# Ejemplos
## Ejemplo 1
![Pasted image 20250507082947.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/4%20Balance%20en%20m%C3%A1quinas/attachments/Pasted%20image%2020250507082947.png)

Para el flujo 1:
- $T_{1}=450 \, \pu{ ºC}$
- $P_{1}=5\, \pu{ bar}$
Para el flujo 2:
- $T_{2}=???$
- $P_{2}=1\, \pu{ bar}$
- $v_{2}=??? \leftarrow$ velocidad 
Primero, se va a hacer el balance de energía:
$$
\cancelto{ 0 }{ \frac{ d(U+E_{k}+E_{p}) }{ dt } } = \sum_{k=1}^{2}\dot{m}_{k}\left( h+\frac{v^{2}}{2}+\cancel{ gz } \right)_{k}+\cancelto{ 0 }{ \dot{Q} }+\cancelto{ 0 }{ \dot{W}_{s} }+\cancelto{ 0 }{ \dot{W} }
$$

> [!important]
> No hay trabajo termodinámico $\dot{W}$, ya que las fronteras no son móviles.

También de balance de masa se sabe que $\dot{m}_{1}=-\dot{m}_{2}$.
Entonces:
$$
h_{1}+\cancel{ \frac{v_{1}^{2}}{2} }-h_{2}-\frac{v_{2}^{2}}{2}=0
$$
La velocidad de entrada se puede despreciar (el ejercicio debería decir eso):
$$
v_{2}=\sqrt{ 2(h_{1}-h_{2}) }
$$
Ahora se ven las tablas. Se obtiene $h_{1}$ usando $T_{1}$ y $P_{1}$. Se obtiene $h_{2}$ usando $P_{2}$ y el hecho de que es reversible, entonces $s_{1}=s_{2}$. Ahora se puede buscar en tabla $h_{2}$ usando $s_{2}$ y $P_{2}$.
