---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/1-ecuaciones-diferenciales-de-primer-orden/clasificacion-de-ecuaciones-diferenciales/","tags":["I1MAT1640"]}
---

# Clasificación por Tipo
Existen [[Ecuaciones diferenciales ordinarias (EDO)\|Ecuaciones diferenciales ordinarias (EDO)]] y [[Ecuaciones diferenciales parciales (EDP)\|Ecuaciones diferenciales parciales (EDP)]].
## EDO
Son [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Introducción a las Ecuaciones diferenciales ordinaias\|Introducción a las Ecuaciones diferenciales ordinaias]] que solo tienen derivadas respecto a una sola variable independiente. Por ejemplo:
$${\frac{d y}{d x}}+\,5y=e^{x},\qquad{\frac{d^{2}y}{d x^{2}}}-{\frac{d y}{d x}}+\,6y=0,\qquad \text{y}\qquad{\frac{d x}{d t}}+{\frac{d y}{d t}}=\,2x+\,y$$
Como se puede ver, las derivadas pueden ser de ordenes mayores y la ecuación puede tener derivadas de otras variables dependientes.
### Ejemplo de EDO
La [[Ley de enfriamiento de Newton\|Ley de enfriamiento de Newton]] está dada por la siguiente ecuación.
$$
\frac{ dT }{ dt } =-k(T-A)
$$
Donde $T$ es la temperatura de un objeto que se encuentra en un medio a temperatura $A$. $k$ es una constante positiva.
Se puede interpretar que si $A > T$, entonces $\frac{ dT }{ dt }$ será positivo y la temperatura sube y viceversa.

Las [[Cursos/Ingeniería Civil/2024-2/Biología de Organismos y Comunidades/3 Ecología y Cambio Global/Introducción a la ecología de poblaciones\|poblaciones]] suelen modelar su crecimiento según la ecuación diferencial (con tasas de natalidad y mortalidad constantes):
$$
\frac{ dP }{ dt } =kP
$$
De aquí la solución a la ecuación es $Ce^{kt}$.
![Pasted image 20250310141533.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/1%20Edos%20de%20primer%20orden/1%20Ecuaciones%20diferenciales%20de%20primer%20orden/attachments/Pasted%20image%2020250310141533.png)
Gráficas de $P(t) = Ce^{kt}$ con $k=\ln 2$.
Esto se interpreta que $k$ es la taza de crecimiento de la población y $C$ es la [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Condiciones iniciales de EDOs\|condición inicial]], que dice la cantidad de población en el tiempo $t=0$. 

# Clasificación por orden
Las ecuaciones diferenciales se pueden clasificar por su orden, este siendo el orden de la derivada de mayor.
# Clasificación por Grado
El grado algebraico de la ecuación. El orden polinómico.
# Clasificación por cantidad de parámetros
Se clasifican las ecuaciones diferenciales en base a la cantidad de parámetros que tenga, por ejemplo, la solución a la ecuación:
$$
y''+\omega^{2}y=0
$$
es:
$$
y=A\cos(\omega t)+B\sin(\omega t)
$$
De aquí la ecuación es **biparamétrica** ya que tiene dos parámetros, $A$ y $B$.
# Regla general del orden y forma normal
Como regla general, aunque hay excepciones, una ecuación diferencial de orden $n$ tendrá $n$ parámetros. Esto usualmente cuando se resuelve de forma explícita. Para esto se define la forma normal de una ecuación diferencial.
> [!definition] forma normal de una ecuación diferencial
> Forma de una EDO en la que se separa a la derivada de mayor orden $n$ de la forma:
> $$
> y^{(n)}=G(x,y,y',y'',\dots,y^{(n-1)})
> $$
