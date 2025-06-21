---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/2-edos-de-orden-superior/wronskianos-de-soluciones/","tags":["I2MAT1640"]}
---

# Concepto
Una matriz que si se hace cero indica que las soluciones que se tienen de un sistema son LD, entonces no son todas las soluciones.
# Definición

Si $y_{1}$ e $y_{2}$ son soluciones de una EDO de segundo orden. El wronskiano se define como:
$$
W(y_{1},y_{2})=\det \begin{bmatrix}
y_{1}(a) & y_{2}(a) \\
y_{1}'(a) & y_{2}'(a)
\end{bmatrix}
$$

> [!theorem] wronskiano de solución
> Supóngase que $y_{1}$ y $y_{2}$ son soluciones de la EDO de segundo orden:
> $$
> y''+p(x)y'+q(x)y=0
> $$
> en un intervalo abierto $I$ donde $p$ y $q$ son continuas.
> - Si $y_{1}$ e $y_{2}$ son [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Independencia y dependencia lineal\|L.D.]], entonces $W(y_{1},y_{2})=0$ en $I$.
> - Si $y_{1}$ e $y_{2}$ son L.I., entonces $W(y_{1},y_{2})\neq 0$ en cada punto de $I$.

La demostración de esto está en la naturaleza de las [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Propiedades de determinantes#^96fe07\|propiedades del determinante de una matriz no invertible]].

> [!theorem] solución general de una ecuación homogenea
> Si $y_{1}$ e $y_{2}$ son soluciones a una Ecuación Homogénea de Segundo Orden, y las dos soluciones son linealmente independientes, entonces se cumple para otra solución $Y$:
> $$
> Y(x)=c_{1}y_{1}+c_{2}y_{2}
> $$
> Es decir, es combinación lineal de $y_{1}$ e $y_{2}$.

Esto es una consecuencia directa de juntar los primeros dos teoremas vistos en [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Ecuaciones lineales de segundo orden y homogeneas\|Ecuaciones lineales de segundo orden y homogeneas]].
# Ejemplo