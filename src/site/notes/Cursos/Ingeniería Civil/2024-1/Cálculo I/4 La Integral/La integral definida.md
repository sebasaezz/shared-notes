---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/la-integral-definida/","tags":["I3MAT1610"]}
---


Dada la integral:

$$\int_a^bf(x)dx$$

Si $a$ y $b$ $\not \exists$, la integral es indefinida, pero si $a,b\in\mathbb{R}$, entonces es definida.

Tomando una interpretación de sumatoria conocida como [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Suma de Riemann\|Suma de Riemann]], se cumple que:

$$
\int _{a}^b f(x)\, dx=\lim_{ n \to \infty } \sum_{i=1}^{n}f(x_{i}^{*})\Delta x 
$$

Donde $x_{i}^{*}$ es un intervalo infinitamente pequeño del dominio de la función.

![Pasted image 20240522124048.png|650](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/4%20La%20Integral/attachments/Pasted%20image%2020240522124048.png)

# Resolución con antiderivadas

Para una integral definida, se define como:

$$\int_a^bf(x)dx=F(b)-F(a)$$

$F(x)$ es la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Antiderivada particular\|Antiderivada particular]] de $f(x)$.

# Ejemplo

$$\int_{0}^{5}(t^2+3)dt$$

La antiderivada de $f(x)=t^2+3$ es $F(x)=\frac{t^3}{3}+3t+c$

Así $\int_{0}^{5}(t^2+3)dt=F(5)-F(0)=(\frac{125}{3}+15+c)-(0+0+c)=\frac{125}{3}+15\approx56,67$
