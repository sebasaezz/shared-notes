---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/pendiente-y-concavidad-de-una-curva-parametrica/","tags":["I1MAT1630"]}
---

# Pendiente
Si $\vec{r}=\langle x(t), y(t) \rangle$ describe a la curva $C$ de modo que la variable $y$ es función derivable de $x$, es decir $y=y(x)$. Por regla de la cadena:
$$
\frac{ dy }{ dt } =\frac{d}{dt}y(x(t))=\frac{ dy }{ dx } ·\frac{ dx }{ dt } 
$$
Entonces la pendiente $\frac{ dy }{ dx }$ será:
$$
\frac{ dy }{ dx } =\frac{\frac{ dy }{ dt } }{\frac{ dx }{ dt } }
$$
Aquellos puntos donde la pendiente se indefine, y la pendiente inversa ($\frac{ dx }{ dy }=\frac{x'}{y'}$) es igual a $0$, resultarán en verticales (no necesariamente asíntotas). 
# Concavidad
Tiene el mismo efecto que la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Intervalos de monotonía y concavidad de una función\|concavidad en una variable]]. Para obtener una ecuación para ella, se debe pensar de la misma forma que se pensó antes, ya que la concavidad de alguna forma es la pendiente de la pendiente.
Si $\frac{ dy }{ dx }=g(x(t))\implies$
$$
\frac{d}{dt} g(x(t))=\frac{ d }{ dx }g(x)·\frac{ dx }{ dt }  
$$

$$
\frac{d}{dx} g(x)=\frac{ d^{2}y }{ dx^{2} } =\frac{\frac{d}{dt} g(x(t))}{\frac{ dx }{ dt } }=\frac{\frac{d}{dt} \left( \frac{ dy }{ dx }  \right)}{\frac{ dx }{ dt } }
$$
# Ejemplo
Para el círculo de radio 2 definido por $\vec{r}=\langle 2\cos t , 2\sin t\rangle$, en $\frac{\pi}{4}$ su pendiente será:
- $x'(t)=-2\sin t$
- $y'(t)=2\cos t$
$$
\implies \frac{ dy }{ dx } =- \frac{2\cos t}{2\sin t}=-\cot t
$$
En $\frac{\pi}{4}$, $-\cot \frac{\pi}{4}=-1$.

