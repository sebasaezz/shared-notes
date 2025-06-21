---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/2-edos-de-orden-superior/ecuaciones-lineales-de-segundo-orden-y-homogeneas/","tags":["I2MAT1640"]}
---


> [!definition] EDO lineal de segundo orden
> Una EDO lineal de segundo orden tiene la forma:
> $$
> A(x)y''+B(x)y'+C(x)y=F(x)
> $$
> Donde todas estas funciones de $x$ son continuas en un mismo intervalo abierto $I$. Básicamente, todas las derivadas de $y$ deben ser de grado $1$.
> 

Si $F(x)=0$, la EDO es lineal homogénea. No se debe confundir con las [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/2 Ecuaciones diferenciales homogeneas/Ecuaciones diferenciales homogeneas\|Ecuaciones diferenciales homogeneas]].

> [!definition] EDO lineal homogénea
> Una EDO lineal homogénea de segundo orden, es una ecuación de la forma:
> $$
> A(x)y''+B(x)y'+C(x)y=0
> $$


Las EDOs homogéneas siempre se van a poder representar de la forma:
$$
y''+p(x)y'+q(x)=0 \tag{1}
$$
Y aquí se cumple el teorema de superposición.

> [!theorem] teorema de superposición de EDOs lineales homogéneas 
> Si $y_{1}$ e $y_{2}$ son soluciones de la EDO mostrada en (1), entonces para $c_{1}$ y $c_{2}$ pesos reales, y otra solución $y$:
> $$
> y=c_{1}y_{1}+c_{2}y_{2}
> $$
> Es decil, cualquier [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Combinaciones lineales y espacio generado\|combinación lineal]] de $y_{1}$ e $y_{2}$ es solución de la EDO.

# Problemas de valor inicial
Ahora los PVI tienen dos valores iniciales, y se cumple que:

> [!theorem] existencia y unicidad para ecuaciones lineales de segundo orden
> Para un punto $a$ perteneciente al intervalo abierto $I$. Si las funciones $f,g,h$ son continuas en $I$, y la ecuación:
> $$
> y''+g(x)y'+h(x)y=f(x)
> $$
> Se cumple que el problema de valor inicial, con $b_{0},b_{1}$ reales:
> $$
> \begin{array}{}
> y'(a)=b_{0} & y(a)=b_{1}
> \end{array}
> $$
> Resulta en **una** (y solo una) función solución en $I$.

En estas ecuaciones se puede aplicar la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Fórmula de Abel\|Fórmula de Abel]]

Esto se ve en que un mismo punto puede tener varias soluciones, entonces se necesita un valor inicial de su derivada:
![Pasted image 20250413003556.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/2%20EDOS%20de%20orden%20superior/attachments/Pasted%20image%2020250413003556.png)
# Solución general
Si se untan los teoremas 1 y 2, se puede concluir que si se tienen dos funciones [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Independencia y dependencia lineal\|linealmente independientes]], entonces la combinación lineal de ellas será la solución general.

Resolver una EDO de la forma:
$$
y''+p(x)y'+q(x)y=f(x)
$$
se debe usar el siguiente teorema:


> [!theorem] teorema de superposición para EDOs lineales de orden 2
> Si $y_{h}$ es la solución **general** de la ecuación homogénea asociada (cuando $f=0$) e $y_{p}$ es una solución particular, entonces:
> $$
> y=y_{h}+y_{p}
> $$
> es la solución general.

## Encontrar $y_{p}$: Método de coeficientes indeterminados

La función $f$ se debe escribir en términos de la base de la función $f$ y su derivada $f'$. Por ejemplo, si la función es $3+2x$, se asumen un $y_{p}=A+Bx$
Si la función es $e^{2x}$, la solución particular será $Ae^{2x}$ ya que con su derivada son LD.

Ahora solo se reemplaza en la EDO y se resuelven los coeficientes (coeficientes indeterminados).

Puede suceder el caso donde la solución particular dada $y_{p}$ sea igual a la homogénea obtenida. En ese caso, al igual que en la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Resolución de EDOs lineales homogéneas de orden superior con coeficientes constantes\|Resolución de EDOs lineales homogéneas de orden superior con coeficientes constantes]] se multiplica por $x$.
## Que pasa si siempre son LI: Variación de parámetros

LA FÓRMULA
$y_{1}$ e $y_{2}$ son las soluciones de la homogénea.
$$
y_{p}=-y_{1}\int \frac{y_{2}f(x)}{W} \, dx +y_{2}\int \frac{y_{1}f(x)}{W}  \, dx 
$$
# Ejemplo