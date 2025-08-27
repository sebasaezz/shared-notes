---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/3-integrales-multiples/3-1-definicion-de-integrales-dobles-para-rectangulos-en-el-plano-integrales-iteradas/integrales-dobles-sobre-regiones-generales/","tags":["I2MAT1620"]}
---

# Concepto
Ya se vio [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.1 Definición de integrales dobles para rectángulos en el plano. Integrales iteradas/Integrales dobles sobre regiones rectangulares\|Integrales dobles sobre regiones rectangulares]], ahora se tendrán regiones más complejas.
# Definición
## Regiones de tipo I
Cuando se tiene una región, donde el eje $y$ se mueve con una función arriba y una abajo, y el eje $x$ está restringido entre $a$ y $b$.
![Pasted image 20241108110904.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/3%20Integrales%20M%C3%BAltiples/3.1%20Definici%C3%B3n%20de%20integrales%20dobles%20para%20rect%C3%A1ngulos%20en%20el%20plano.%20Integrales%20iteradas/attachments/Pasted%20image%2020241108110904.png)
Ahora la integral será simplemente:
$$
\iint f(x,y)\,dy\,dx=\int_{a}^{b} \int_{g_{1}(x)}^{g_{1}(x)} f(x,y) \, dy  \, dx 
$$
## Regiones de tipo II
Ahora la función define al eje $x$ con una función.
![Pasted image 20241108111328.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/3%20Integrales%20M%C3%BAltiples/3.1%20Definici%C3%B3n%20de%20integrales%20dobles%20para%20rect%C3%A1ngulos%20en%20el%20plano.%20Integrales%20iteradas/attachments/Pasted%20image%2020241108111328.png)
$$
\underset{ D }{ \iint } f(x,y)\,dy\,dx=\int_{c}^{d} \int_{h_{1}(y)}^{h_{1}(y)} f(x,y) \, dx  \, dy 
$$
# Propiedades de las integrales dobles
Se aplican todas las [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Propiedades de la integral definida\|Propiedades de la integral definida]] de cálculo I. La única que varía un poco es que:
Si $D=D_{1} \cup D_{2}$ y $D_{1} \cap D_{2}=\emptyset$.
Entonces:
$$
\underset{ D }{ \iint }f(x,y) \, dA=\underset{ D_{1} }{ \iint }f(x,y) \, dA+\underset{ D_{2} }{ \iint }f(x,y) \, dA
$$

Si se integra la función $1$, se obtiene un volumen ($L^{3}$) que tiene el mismo valor numérico que el área ($L^{2}$) de $D$.
$$
\underset{ D }{ \iint }1 \,dA=\operatorname{Area(D)}
$$
{ #87cb72}



# Ejemplo
## Ejemplo 1
Calcular la integral para $f(x,y)=x+2y$ sobre la región acotada por las parábolas $y=2x^{2}$ e $y=1+x^{2}$.
Se debe partir analizando que las dos funciones suben, una más rápido que la otra, entonces se van a intersecar en dos puntos. Estos serán los límites de $x$ de la integral.
$$
\begin{align}
2x^{2} & =1+x^{2} \\
x^{2} & =1 \\
x & =\pm 1
\end{align}
$$
Ahora se toma a $a=-1$ y $b=1$.
$$
\underset{ D }{ \iint }f(x,y) \,dy\,dx=\int_{-1}^{1} \int_{2x^{2}}^{1+x^{2}} x+2y \, dy  \, dx =\frac{32}{15}
$$
La región será:
![Pasted image 20241108114543.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/3%20Integrales%20M%C3%BAltiples/3.1%20Definici%C3%B3n%20de%20integrales%20dobles%20para%20rect%C3%A1ngulos%20en%20el%20plano.%20Integrales%20iteradas/attachments/Pasted%20image%2020241108114543.png)
Y la integral se representa por:
![Pasted image 20241108115508.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/3%20Integrales%20M%C3%BAltiples/3.1%20Definici%C3%B3n%20de%20integrales%20dobles%20para%20rect%C3%A1ngulos%20en%20el%20plano.%20Integrales%20iteradas/attachments/Pasted%20image%2020241108115508.png)

