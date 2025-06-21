---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/1-ecuaciones-diferenciales-de-primer-orden/campos-de-direccion-e-isoclinas/","tags":["I1MAT1640"]}
---

# Concepto
Una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Introducción a las Ecuaciones diferenciales ordinaias\|EDO]] de la forma:
$$
\frac{ dy }{ dx } =f(x,y)
$$
Nos dice directamente el valor de la derivada de la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Solución de una ecuación diferencial ordinaria, solución general, implícita y explícita\|solución]] en un punto. Usando esto se puede crear un [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Campos vectoriales\|campo vectorial]] para graficar el comportamiento de las soluciones.
# Ejemplo
La EDO:
$$
\frac{ dy }{ dx } =\sin x+y
$$
Tiene la forma necesaria para asociarle un campo de dirección, y este se vería de la siguiente forma (Usar `VectorPlot[]` en wolfram):
![Pasted image 20250315145448.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/1%20Edos%20de%20primer%20orden/1%20Ecuaciones%20diferenciales%20de%20primer%20orden/attachments/Pasted%20image%2020250315145448.png)
## Interpretación
La ecuación mostrada tiene como solución (difícil de resolver):
$$y= C e^x - \frac{\sin(x) + \cos(x)}{2}$$
Variar $C$ en esta función resultará en distintas funciones que van a seguir las derivadas que se ven en el campo de dirección.
<iframe width='500' height='500' src='https://www.wolframcloud.com/obj/d56cd282-bfc0-4199-9147-160e1fd4914d' frameborder='0'></iframe>

$$
\frac{ dA }{ dt }=  A(t) 
$$