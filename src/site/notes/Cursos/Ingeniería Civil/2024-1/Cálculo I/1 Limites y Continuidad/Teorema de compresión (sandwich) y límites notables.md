---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/1-limites-y-continuidad/teorema-de-compresion-sandwich-y-limites-notables/"}
---


Dadas tres funciones $f$ $g$ y $h$ tales que:

$$
g(x)\leq f(x)\leq h(x)
$$

Es decir, $f(x)$ está acotado por $g$ y $h$.

Entonces, para todo punto cercano a $x=a$, excepto posiblemente $x=a$ :

$$
\lim_{ x \to a } g(x)=\lim_{ x \to a } h(x)=L \implies \lim_{ x \to a } f(x)=L
$$

![primero.webp](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/1%20Limites%20y%20Continuidad/attachments/primero.webp)

_($c$ es $a$)_

El teorema del sandwich es cierto para límites laterales.

# Ejemplo

Demostrar que:

$$
\lim_{ x \to 0 } x^{2}\sin\left( \frac{1}{x} \right)
$$

Dado el recorrido de la función seno, se tiene que:

$$
-1\leq \sin\left( \frac{1}{x} \right) \leq 1
$$
$$
-x^{2}\leq x^{2}\sin\left( \frac{1}{x} \right) \leq x^{2}
$$
$$
\lim_{ x \to 0 } -x^{2} \leq \lim_{ x \to 0 } x^{2}\sin\left( \frac{1}{x} \right) \leq \lim_{ x \to 0 } x^{2}
$$

Dado el teorema, se concluye que, como los dos límites de las cotas son 0:

$$
\lim_{ x \to 0 } x^{2}\sin\left( \frac{1}{x} \right)=0
$$
```desmos-graph 
 left=-0.35; right=0.35; 
 top=0.1; bottom=-0.1; 
 --- 
 f(x)=x^{2} \sin{1/x}
 g(x)=x^2
 h(x)=-x^2
 ```
 