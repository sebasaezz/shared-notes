---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/2-edos-de-orden-superior/resolucion-de-ed-os-lineales-homogeneas-de-orden-superior-con-coeficientes-constantes/","tags":["I2MAT1640"]}
---

De forma general, se resuelve una ecuación de la forma:
$$
y^{(n)}+a_{1}y^{(n-1)}+\dots+a_{n-1}y'+a_{n}y=0
$$
# Estrategia para segundo orden

Se sabe que para las [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Ecuaciones lineales de segundo orden y homogeneas\|EDOs de segundo orden]] **homogeneas**:
1. Encontrar soluciones L.I $y_{1}$ e $y_{2}$.
2. Verificar con el [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Wronskianos de soluciones\|Wronskianos de soluciones]].
3. La solución general es $Ay_{1}+By_{2}$.

Ahora se hace lo mismo notando que la solución casi siempre va a tener la forma $y^{rx}\implies y^{(n)}=r^{n}e^{rx}$.

Sin embargo, se pueden obtener soluciones repetidas $y_{r}$. En ese caso, las dos soluciones son:
- $y_{1}=y_{r}$
- $y_{2}=(A+Bx)y_{r}$

Se la solución de la ecuación característica es un complejo conjugado $\alpha\pm\beta i$, entonces:
$$
y(t)=e^{\alpha t}(c_{1}\cos\beta t+c_{2}\sin\beta t)
$$

# Ejemplo
$y''+y=0$
Se supone que una solución es $y=e^{rx}\implies r''=r^{2}e^{rx}$
Entonces:
$$
\begin{align}
r^{2}e^{rx} & =-e^{rx} \\
r^{2} & =-1 \\
r & =\pm i
\end{align}
$$
Entonces la solución general (ya que son L.I.) es:
$$
y=Ae^{ix}+Be^{-ix}
$$
Aquí se puede aplicar la [[Identidad de Euler\|Identidad de Euler]]:
$$
e^{ix}=\cos x+i\sin x
$$