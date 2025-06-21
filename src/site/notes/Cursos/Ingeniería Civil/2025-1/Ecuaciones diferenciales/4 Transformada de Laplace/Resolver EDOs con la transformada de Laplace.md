---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/4-transformada-de-laplace/resolver-ed-os-con-la-transformada-de-laplace/","tags":["ExMAT1640"]}
---

# Concepto
Transformar una ecuación diferencial a una algebraica con la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/4 Transformada de Laplace/Transformada de Laplace\|Transformada de Laplace]] y después devolverla con una anti-transformada. Solo se aplica transformada a una ecuación.
# Definición
# Ejemplo
## Ejemplo 1
transforme la ecuación $x''-x'-6x=0$ con condiciones $x(0)=2$ y $x'(0)=-1$
La transformada de 0 es 0, entonces se sigue en la función de la izquierda.
$$
\begin{align}
\mathcal{L}\{ x''-x'-6x \} & =\mathcal{L}\{ x'' \}-\mathcal{L}\{ x' \}-6\mathcal{L}\{ x \}
\end{align}
$$
Se va a definir a $\mathcal{L}\{ x \}=L$.
Por transformada de una derivada:
$$
\begin{align}
\mathcal{L}\{ x'(t) \} & =-x(0)+sL \\
 &  =-2+sL
\end{align}
$$
Lo mismo:
$$
\begin{align}
\mathcal{L}\{ x''(t) \} & =-x'(0)+s\mathcal{L}\{ L \} \\
 & =1+s(-2+sL) \\
 & =s^{2}L-2s+1
\end{align}
$$
Ahora la ecuación final queda:
$$
\begin{align}
s^{2}L-2s+1+2-sL-6L & =0 \\
(s^{2}-s-6)L & =2s-3 \\
L & =\frac{2s-3}{s^{2}-s-6}
\end{align}
$$
Para resolver esto se pueden usar fracciones parciales, llegando a que:
$$
L=\mathcal{L}\{ x \}=\frac{2s-3}{s^{2}-s-6}=\frac{3}{5} \frac{1}{(s-3)}+ \frac{7}{5} \frac{1}{(s+2)}
$$
Se debe encontrar la anti-transformada de $L$, la cual evidentemente es:
$$
\mathcal{L}^{-1}\{ L \}=\mathcal{L}^{-1}\{ \mathcal{L}\{ x \} \}=x(t)= \frac{3}{5} \mathrm{e}^{ 3t } + \frac{7}{5}\mathrm{e}^{ -2t }
$$