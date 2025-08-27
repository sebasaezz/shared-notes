---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/2-la-derivada/derivacion-implicita/","tags":["I2MAT1610"]}
---


Se han visto funciones que se pueden escribir de la forma $y=f(x)$. Pero no todas las funciones se pueden escribir de esta forma, por ejemplo: $x^{2}+y^{2}=25$ es una circunferencia de radio $5$, pero no puede ser una función, dado que cada valor de $x$ tiene dos valores de $y$.

Para solucionar esto, se deben considerar dos funciones:

Para $x^{2}+y^{2}=25$, se define:

$f(x)=-\sqrt{ 25-x^{2} }$

$g(x)=\sqrt{ 25-x^{2} }$

```desmos-graph 
 x^{2}+y^{2}=25 
 ```

Así, se puede calcular la derivada de cada una.

# Cálculo II, derivación implícita en funciones de varias variables

#I3MAT1620 

# Ejemplo
## Ejemplo 2
$$
x^{3}+(f(x))^{3}=3xf(x)
$$

o

$$
x^{3}+y^{3}=3xy
$$
```desmos-graph 
 x^3+y^3=2xy
 ```

 Se puede calcular de derivada de la siguiente forma:

 $$
3x^{2}+3y^{2}· \frac{dy}{dx}=6\left( 1·y+x· \frac{dy}{dx} \right)
$$
$$
3x^{2}+2y^{2} \frac{dy}{dx}=6y+6x+6x \frac{dy}{dx}
$$
$$
\implies (3y^{3}-6x) \frac{dy}{dx}=6y-3x^{2}
$$
$$
\implies \frac{dy}{dx}= \frac{6y-3x^{2}}{3y^{3}-6x}
$$

Así, se llega a una derivada depende tanto de $x$ como de $y$, no es una función.

Entonces, ante la pregunta: ¿Cuál es la pendiente en el punto $(3,3)$?

Se reemplaza $x$ por 3 e $y$ por 3.

$$
m=\frac{6·3-3·9}{3·27-18}=-1
$$

¿En qué punto en el primer cuadrante es horizontal la tangente?

$$
\frac{6y-3x^{2}}{3y^{3}-6x}=0 \iff 6y-3x^{2}=0 \iff y=\frac{1}{2}x^{2}
$$

Entonces, se vuelve a la ecuación original, así:

$$
x^{3}+\left( \frac{1}{2}x^{2} \right)^{3}=6x\left( \frac{1}{2}x^{2} \right)
$$
$$
\implies x^{3}\left( \frac{1}{8}x^{3}-2 \right)=0 \implies \begin{cases}
x^{3} & = & 0 \implies x_{1}=0 \\
\frac{1}{8}x^{3}-2 & = & 0\implies x_{2}=2\sqrt[3]{ 2 }
\end{cases}
$$

Como $y=\frac{1}{2}x^{2}$, se tienen los puntos $(0,0)$ y $(2\sqrt[3]{2  },2\sqrt[3]{ 4 })$

Solo uno de estos puntos pertenece al cuadrante especificado, y ese es $(2\sqrt[3]{2  },2\sqrt[3]{ 4 })$.
