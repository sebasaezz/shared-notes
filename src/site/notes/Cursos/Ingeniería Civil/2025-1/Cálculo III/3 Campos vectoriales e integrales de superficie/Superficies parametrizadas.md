---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/superficies-parametrizadas/","tags":["I3MAT1630"]}
---

# Definición

> [!definition] superficie parametrizada
> Una superficie parametrizada por $\vec{r}$ es el conjunto de puntos $(x,y,z)$ en $\mathbb{R}^{3}$ que cumple con las ecuaciones:
> $$
> \begin{array}{}
> x=x(s,t) & y=y(s,t) & z=z(s,t)
> \end{array}
> $$
> Para algún $(s,t)\in D$.

# Curvas reticulares
Si se toman rectas en $(s,t)$, estas van a ser curvas que den la vuelta a la superficie. Estas son las curvas reticulares.
![Pasted image 20250514101910.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250514101910.png)
# Superficies de revolución
Se tiene una función $f(x)$ que se hace rotar en el eje $x$. Se puede parametrizar $x=x$. Ahora se parametriza con respecto a un ángulo $\theta$ en el eje $yz$. Así la parametrización será:
$$
\langle x,f(x)\cos\theta, f(x)\sin \theta \rangle 
$$
El área es:
$$
2\pi \int_{a}^{b} f(x)\sqrt{ 1+f'(x)^{2} } \, \mathrm{d}x 
$$
# Ejemplo
## Superficies simples
### Esfera
Parametrice:
$$
x^{2}+y^{2}+z^{2}=a^{2}
$$
Esto se hace con [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.10 Coordenadas esféricas. Calculo de integrales triples utilizando coordenadas cilíndricas y esféricas/Cambio a coordenadas esféricas para resolver integrales triples\|coordenadas esféricas]] el radio de la esfera $\rho=a$. De aquí se toman las parámetros $\theta$ y $\phi$, y se usa la parametrización que ya se conoce:
- $x=\rho \sin \phi \cos\theta$
- $y=\rho \sin \phi \sin \theta$
- $z=\rho \cos \phi$
Ahora el cambio de variable a un punto $(\theta,\phi)$ con $D=\{ (\theta,\phi):0\leq\theta \leq 2\pi,0\leq \phi \leq \pi \}$ muestra las curvas reticulares.
![Pasted image 20250514102540.png|200](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250514102540.png)
### Cilindro
Encontrar las ecuaciones paramétricas del cilindro:
$$
x^{2}+y^{2}=4: 0\leq z\leq 1
$$
Como está libre en $z$, se toma $z=z$. Para las otras dos coordenadas se toma un circulo en $\theta$:
$$
\langle 2\cos \theta ,2\sin\theta,z\rangle :0\leq\theta \leq 2\pi,0\leq z\leq 1
$$
### Paraboloide
Parametrize el paraboloide:
$$
z=x^{2}+2y^{2}
$$
Se puede considerar como una función de dos variables, donde simplemente $z=f(x,y)=x^{2}+2y^{2}$. Entonces hacer este reemplazo ya deja solo dos variables, $x$ e $y$.
$$
\langle x,y,\underbrace{ x^{2}+2y^{2} }_{ f(x,y) } \rangle 
$$
Cualquier superficie dada por $z=f(x,y)$ se parametriza de la forma:
$$
\langle x,y,f(x,y) \rangle 
$$
## Superficies de revolución
