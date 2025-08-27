---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/aproximaciones-lineales-y-diferenciales/","tags":["I2MAT1610"]}
---

# Aproximaciones lineales 
## Concepto

Se quiere calcular un punto $f(a)$ en una función difícil de calcular. Entonces, se recurre a una aproximación dada por la tangente en $(a,f(a))$.

## Definición

Se define la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/2 La derivada/Cálculo de recta tangente a un punto\|ecuación para la recta tangente]] en un punto $a$ como:

$$
y=f(a)+f'(a)(x-a)
$$

A esta recta, pero dada por una función $L(x)$ como linealización de a.

Entonces, dado lo dicho anteriormente, se hace la aproximación:

$$
f(x) \approx f(a)+f'(a)(x-a)
$$
## Ejemplo
### Ejemplo 1

Encuentre la linealización de la función $f(x)=\sqrt{ x+3 }$ en 𝑎 = 1 y úsela para obtener una aproximación de los números $\sqrt{ 3.98 }$ y $\sqrt{ 4.05 }$.
	Se define a $f'(x)=\frac{1}{\sqrt{ x+3 }}·1$.
	Así, se define la linealización en $1$ como $L(x)=\sqrt{ 4 }+\frac{1}{\sqrt{ 1+3 }}(x-1)=2+\frac{1}{2}(x-1)$.
	Entonces, dado lo definido anteriormente: $\sqrt{ 0.98+3 }=2+\frac{1}{2}(0.98-1)=1.99$.
	Se comprueba así, que el valor real es aproximadamente el obtenido: $|v_{r}-v_{o}| = |1.99499-1.99|=0.00499$.

# Diferenciales
{ #83904c}


Para una función $y=f(x)$, en su derivada siempre van a existir diferencias $dx$ y $dy$, dados por $\frac{dy}{dx}=f'(x)$. Estos diferenciales (en el caso de $\frac{dy}{dx}$) al cambio de $y$ en la recta tangente a un punto dado un cambio en $x$, un diferencial.

Por otro lado está el delta $x$ e $y$, representados como $\Delta x$ y $\Delta y$, los mismo que se utilizan para el cálculo de [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/La derivada como una razón de cambio y aplicaciones\|razones de cambio]], y es que estos hablan de la función en sí, y no de su tangente o función linearización.

Si la derivada es hecha respecto a $x$, entonces quiere decir que $\Delta x=dx$, y que $dy=dxf'(x)$.
De aquí que una aproximación lineal se puede ver como:
$$
f(x)=f(a)+dy
$$
Cond $dy$ una función de $x$, y dado por $f'(a)(x-a)$
![Pasted image 20241102205828.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/3%20Aplicaciones%20de%20la%20Derivada/attachments/Pasted%20image%2020241102205828.png)
![Pasted image 20240503012135.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/3%20Aplicaciones%20de%20la%20Derivada/attachments/Pasted%20image%2020240503012135.png)
