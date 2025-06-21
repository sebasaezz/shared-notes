---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/1-ecuaciones-diferenciales-de-primer-orden/problemas-de-soluciones-mezclas/","tags":["ExMAT1640"]}
---

# Concepto
Una aplicación de [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/EDOs lineales de primer orden y factor integrante\|EDOs lineales de primer orden y factor integrante]].
# Definición
Se tiene un tanque al que le entra soluto a una velocidad $r_{i}$ y sale solución a otra velocidad $r_{o}$. El soluto entra a una concentración $c_{i}$ y sale a una concentración $c_{o}$.
Se quiere obtener una ecuación para la cantidad de soluto $x(t)$ a partir de un $x(0)=x_{0}$. Para esto debe haber una función del volumen $V(t)$ de modo que:
$$
c_{o}=\frac{x}{V}
$$
Se puede estimar el cambio de soluto $\Delta x$ en un intervalo de tiempo $[t,t+\Delta t]$, de modo que la cantidad de soluto que fluye al entrar será 
$$
c_{i} \left[ \frac{g}{L} \right]·r_{i}\left[ \frac{L}{s} \right]·\Delta t[s]
$$
La cantidad de soluto que fluye hacia afuera será:
$$
c_{o}·r_{o}·\Delta t
$$
Ahora, se puede tener una expresión aproximada para el cambio en la cantidad de soluto, ya que será la diferencia entre lo que entra y lo que sale en $\Delta t$.
$$\Delta x\approx r_{i}c_{i}\Delta t-r_{o}c_{o}\Delta t$$
Ahora, se va a tener una razón de cambio:
$$
\frac{\Delta x}{\Delta t}\approx r_{i}c_{i}-r_{o}c_{o}
$$
Tomando una aproximación diferencial:
$$
\frac{ dx }{ dt } 
=
r_{i}c_{i}-r_{o}c_{o}:c_{0}=\frac{x(t)}{V(t)}
$$
o de otra forma:
$$
\frac{ dx }{ dt } =r_{i}c_{i}-\frac{r_{o}}{V}x
$$
Esta es una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/EDOs lineales de primer orden y factor integrante\|EDO lineal de primer orden]], y se resuelve con el factor integrante.
![Pasted image 20250406183522.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/1%20Edos%20de%20primer%20orden/1%20Ecuaciones%20diferenciales%20de%20primer%20orden/attachments/Pasted%20image%2020250406183522.png)
# Ejemplo