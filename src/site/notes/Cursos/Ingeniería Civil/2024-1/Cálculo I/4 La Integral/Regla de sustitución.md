---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/regla-de-sustitucion/","tags":["ExMAT1610","Técnicas-de-integración"]}
---

# Concepto

Hacer un cambio de variable para resolver una integral

# Definición

> [!theorem] Regla de sustitución
> Si $u=g(x)$ con rango en un intervalo $I$, y $f$ es continua sobre $I$, Entonces:
> $$
> \int f(g(x))·g'(x) \, dx =\int f(u) \, du 
> $$
{ #1388eb}


## Para integrales definidas

Se deben ajustar los límites de integración para la nueva variable. Los límites normales son para $x$, no para $u$.

Como esta integral tiene un valor numérico, no se necesita reemplazar $u$ con $f(x)$ tras calcular las antiderivadas, ya que estas se establecieron según los nuevos límites de integración

> [!theorem] Regla de sustitución para integrales definidas
> Si $g'$ es continua sobre $[a,b]$ y $f$ es continua sobre el rango de $u=g(x)$:
> $$
> 	\int_{a}^{b} f(g(x))·g'(x) \, dx=\int_{g(a)}^{g(b)}  f(u)\, du  
> $$

### Ejemplo

Se elige $u=2x+1\implies du=2dx$

$$\int_{0}^{4}  \sqrt{ 2x+1 }\, dx= \frac{1}{2} \int_{9}^{1} \sqrt{ u } \, du $$

# Ejemplo

Calcular $\int 2x\sqrt{  1+x^{2}} \, dx$

Se hace un cambio de variable, considerando $u=1+x^{2}\implies du=2xdx$. ([[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Aproximaciones lineales y diferenciales#^83904c\|diferenciales]]).

Ahora:

$$
\int 2x\sqrt{ 1+x^{2} } \, dx=\int \sqrt{ u } \, 2xdx=\int \sqrt{ u } \, du =\frac{2}{3}u^{3/2}+C  
$$

Ahora hay que devolverse del cambio de variable:

$$
\frac{2}{3}(1+x^{2})^{3/2}+C
$$
## Ejemplo 2
---

#### Enunciado

Calcula la integral definida $\int_{1}^{3}  (2x+1)^3\, dx$ usando la regla de sustitución.

---
#### Desarrollo

Para resolver esta integral, podemos hacer un cambio de variable. Elegimos $u=2x+1$, entonces la derivada de $u$ respecto a $x$ es $du\,=\,2dx$.

Ahora reescribimos la integral en términos de $u$. Además, debemos cambiar los límites de integración para que correspondan a los valores de $u$: cuando $x = 1$, $u = 2*1 + 1 = 3$; cuando $x = 3$, $u = 2*3 + 1 = 7$. Entonces la integral se convierte en:

$$ \frac{1}{2}\int_{3}^{7} u^3 \, du $$

La antiderivada de $u^3$ es $(1/4)u^4$. Usando el Teorema Fundamental del Cálculo obtenemos:

$$ F(b) - F(a) = \left. \frac{1}{4} u^4 \right|_{3}^{7} = \frac{7^4}{4}-\frac{3^4}{4}= \frac{(2400)}{4}=600 $$

Por lo tanto, la integral dada es igual a 600.