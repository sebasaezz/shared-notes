---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-9-definicion-de-diferenciabilidad-vector-gradiente-plano-tangente-aproximacion-lineal/diferenciabilidad-en-r3/","tags":["I3MAT1620"]}
---

La misma idea de [[Cursos/Ingeniería Civil/2024-1/Cálculo I/2 La derivada/Función derivada y diferenciabilidad\|diferenciabilidad en cálculo I]], pero aplicada a superficies. Ahora la superficie se parece a un plano en todos sus puntos de su dominio.

> [!theorem] diferenciabilidad de una función de dos variables
> Una función es diferenciable en $(x_{0},y_{0})$ si se cumple que:
> $$
> \lim_{ (h,k) \to (0,0) } \frac{f(x_{0}+h,y_{0}+k)-f(x_{0},y_{0})-f_{x}(x_{0},y_{0})h-f_{y}(x_{0},y_{0})k}{\sqrt{ h^{2}+k^{2} }}=0
> $$
> Si se aproxima a cero, la distancia entre las diferencias de las derivadas se acerca más rápido a cero que la distancia al punto.

# Diferenciabilidad usando plano tangente
Se tenía para cálculo uno el concepto de diferenciales, y también las diferencias en $x$ y $y$, $\Delta x$ y $\Delta y$. 
Considerando la imagen que se muestra abajo, solo que en vez de $x$ se tiene un punto cualquiera $a$, se puede llegar a la siguiente definición del incremento de $y$:
$$
\Delta y=\underbrace{ f(a+\Delta x) }_{ P }-\underbrace{ f(a) }_{ Q }
$$
![Pasted image 20241102193817.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.9%20Definici%C3%B3n%20de%20diferenciabilidad.%20Vector%20gradiente.%20Plano%20tangente.%20Aproximaci%C3%B3n%20lineal/attachments/Pasted%20image%2020241102193817.png)

Ahora, se sabe que la derivada va a estar dada por:
$$
f'(a)=\lim_{ \Delta x \to 0 } \frac{\Delta y}{\Delta x}\implies \lim_{ \Delta x \to 0 } \left(\frac{\Delta y}{\Delta x}\right)-f'(a)=\lim_{ \Delta x \to 0 } \underbrace{ \left( \frac{\Delta y}{\Delta x}-f'(a) \right) }_{ \varepsilon }=0
$$
Pero mientras no sea límite, va a existir un valor $\varepsilon$ que va a ser una función de $\Delta x$, de aquí que se puede escribir a $\Delta y$ de la siguiente forma:
$$
\varepsilon=\frac{\Delta y}{\Delta x}-f'(a)\implies\Delta y=f'(a)\Delta x-\varepsilon\Delta x
$$
Ahora se puede llegar a una definición de derivabilidad, que dice que en una función derivable se podrá escribir
$$
\Delta y = f'(a)\Delta x+\varepsilon\Delta x: \text{donde } \varepsilon \rightarrow0 \text{ cuando } \Delta x \rightarrow0
$$Ahora, en 2 variables se puede usar este mismo concepto llegando a que

> [!definition] función diferenciable en dos variables 
> Una función diferenciable es aquella que se puede escribir como:
> $$
> \Delta z=f_{x}\Delta x+f_{y}\Delta y+\varepsilon_{1}\Delta x+\varepsilon_{2}\Delta y
> $$
> Donde $\varepsilon_{1}$ y $\varepsilon_{2} \rightarrow 0$ conforme $\Delta x$ y $\Delta y \rightarrow 0$ 

