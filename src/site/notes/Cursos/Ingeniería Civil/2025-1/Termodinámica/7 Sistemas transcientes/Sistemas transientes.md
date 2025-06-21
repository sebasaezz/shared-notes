---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/7-sistemas-transcientes/sistemas-transientes/","tags":["ExIIQ1003"]}
---

Tienen un balance de masa y energía distinto de cero.
$$
\begin{align}
\frac{ \mathrm{d}U }{ \mathrm{d}t }  & \neq 0 & \frac{ \mathrm{d}m }{ \mathrm{d}t }  & \neq 0
\end{align}
$$
Generalmente se van a tener tanques, donde el trabajo termodinámico es nulo, $W=0$, sin embargo, se se va a tener un trabajo de eje $W_{\text{s}}\neq 0$.
# Procesos transientes simples
Se tienen los siguiente supuestos típicos:
- Se considera que **el flujo de entrada es uniforme**, esto es con una entalpía constante.
- En cualquier momento, la energía que presenta una unidad de masa dentro del sistema es igual para todas las unidades de masa. Esto es un sistema **perfectamente agitado** o estado uniforme.
Con estos supuestos, se construye el siguiente balance de energía:
$$
\frac{ \mathrm{d}(m u) }{ \mathrm{d}t } =\sum_{k=1}^{K}\dot{m}_{k}h_{k}+\dot{Q}-P\Delta V+\dot{W}_{\text{s}}
$$
Si se evalúa en un tiempo $t$, se facilita el análisis del sistema.
$$
\Delta(m u)=\sum_{k=1}^{K}m_{k}h_{k}+Q-P\Delta V+W_{\text{s}}
$$