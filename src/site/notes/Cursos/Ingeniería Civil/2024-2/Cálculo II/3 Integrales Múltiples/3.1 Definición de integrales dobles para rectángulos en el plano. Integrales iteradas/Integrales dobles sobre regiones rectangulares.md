---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/3-integrales-multiples/3-1-definicion-de-integrales-dobles-para-rectangulos-en-el-plano-integrales-iteradas/integrales-dobles-sobre-regiones-rectangulares/","tags":["I2MAT1620"]}
---

# Concepto
La integral normal se puede interpretar como un [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Suma de Riemann\|área bajo una curva]] usando la suma de Riemman.
Ya no se tiene una curva, se tiene una superficie. Antes se tenían los ejes entre un $a$ y un $b$. Ahora va a haber una región $\mathcal{D}$.

Considerando una partición entre $a$ y $b$ en el eje $x$ y entre $c$ y $d$ en el eje $y$, con $i$ y $j$ perteneciendo a cada uno respectivamente.
Ahora se puede considerar un $\Delta A$ como un diferencial de área. 
Si el $\Delta x= \frac{b-a}{n}$ y el $\Delta y=\frac{d-c}{n}$, ahora el diferencial de área sera:
$$
\Delta A=\frac{b-a}{n}· \frac{d-c}{m}
$$
Sea $x_{ij}^*$ la $ij$-ésima partición del eje $x$, y $y_{ij}^*$ la $ij$-ésima partición del eje $y$.
	
![Pasted image 20241106151537.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/3%20Integrales%20M%C3%BAltiples/attachments/Pasted%20image%2020241106151537.png)

Entonces se puede definir:
> [!definition] integral doble
> $$
> \iint_{\mathcal{D}}f(x,y)dA=\lim_{ (m,n) \to \infty } \sum_{i=1}^{n}\sum_{i=1}^{m}f(x_{ij}^*,y_{ij}^*)\Delta A
> $$

> [!theorem] Teorema de Fubini
> Si $f$ es continua en el rectángulo $R=[a,b]\times[c,d]$, entonces:
> $$
> \iint_{R}f(x,y)dA=\int_{a}^{b} \int_{c}^{d} f(x,y) \, dy  \, dx =\int_{d}^{c} \int_{a}^{b} f(x,y) \, dx  \, dy 
> $$




# Ejemplo
## Ejemplo 1
Calcular en el cuadrado $\mathcal{D}=[0,2]\times[0,2]$ para la función $f(x,y)=16-x^{2}-y^{2}$. Desde la esquina superior derecha de cada cuadrado
Se puede saber que:
- $\Delta y=\frac{2}{n}$
- $\Delta x=\frac{2}{m}$
El punto muestra, para una coordenada $ij$ será $\left( \frac{2}{m}i, \frac{2}{n}j \right)$.
Ahora el volumen del prisma para $ij$ será $f\left( \frac{2}{m}i, \frac{2}{n}j \right)\Delta A$.
$$
\lim_{ (m,n) \to \infty } \sum_{j=1}^{n}\sum_{i=1}^{m}f\left( \frac{2}{m}i, \frac{2}{n}j \right)\Delta A=\underset{ [0,2]\times[0,2] }{ \iint } f(x,y)dA
$$
## Ejemplo 2
Calcular:
$$
\iint_{R}\sqrt{ 1-x^{2} }dA
$$
para: $R= [-1,1]\times[-2,2]$
Pero esta función es simple. Es un medio círculo de $-1$ a $1$ en el eje $xz$ libre en $y$. Es decir, un semicírculo cilíndrico.
En el eje libre, piden desde $-2$ a $2$, y el cilindro está en todo el eje $x$ de $R$.
Ahora el volumen será simplemente el volumen de un medio cilindro de altura 4. (o un cilindro de altura 2)
$$
A=\frac{\pi r^{2}h}{2}=\frac{\pi ·1^{2}·4}{2}=2\pi
$$
