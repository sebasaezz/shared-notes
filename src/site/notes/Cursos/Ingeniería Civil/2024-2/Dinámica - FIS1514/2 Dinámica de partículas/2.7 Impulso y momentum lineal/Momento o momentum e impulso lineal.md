---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/2-dinamica-de-particulas/2-7-impulso-y-momentum-lineal/momento-o-momentum-e-impulso-lineal/","tags":["ExFIS1514"]}
---

# Concepto
Integrar la [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.1 Leyes de Newton/Fuerza y leyes de Newton, Diagramas de cuerpo libre\|fuerza neta]] sobre un intervalo de tiempo para conseguir una cantidad de movimiento y un impulso.
# Definición
Se sabe, de las [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.1 Leyes de Newton/Fuerza y leyes de Newton, Diagramas de cuerpo libre\|leyes de newton]], que:
$$
\sum_{}^{}F=\vec{F}_{\text{neta}}=m\vec{a}=m \frac{ d\vec{v} }{ dt } 
$$
Ahora se va a [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/La integral definida\|integrar]]:
$$
\vec{I}=\int_{t_{1}}^{t_{2}} \vec{F} \, dt =m\int_{t_{1}}^{t_{2}}  \frac{ d\vec{v} }{ dt }  \, dt=m\int_{\vec{v}_{1}}^{\vec{v}_{2}}  \, d\vec{v} =m\vec{v}_{2}-m\vec{v}_{1}=\vec{p}_{2}-\vec{p}_{1}=\Delta \vec{p}
$$
De aquí se define:
- $\vec{p}_{t}=$ momentum
- $\Delta \vec{p}=$ impulso $\vec{I}$
Notar que:
- Es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Ecuación vectorial\|Ecuación vectorial]].
- Requiere de un sistema de referencia, y se debe satisfacer en ambos ejes (separar ecuaciones).
$$
\begin{align}
 &  & \vec{I}=0 & =\vec{p}_{2}-\vec{p}_{1}&  &   \\
\implies &  & \vec{p}_{1} & =\vec{p}_{2} \iff F_{\text{neta}}=0
\end{align}
$$
Es decir, si no hay fuerza neta, el momentum se conserva.
# Ejemplo