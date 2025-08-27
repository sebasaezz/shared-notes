---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/propiedades-de-la-integral-definida/","tags":["I3MAT1610"]}
---


Con $a,b,c\in\mathbb{R}$

# Orden de límites de integración
{ #acbffe}


Si se cambia el orden de los límites de integración, la integral resulta en su versión negativa:

$$
\boxed{\int _{a}^{b}f(x) \, dx =-\int _{b}^af(x) \, dx} 
$$
# Área bajo un punto
$$
\boxed{\int_{a}^{a} f(x) \, dx=0 } 
$$
# Integral de una constante

Se puede interpretar como el área de un rectángulo:

$$
\boxed{\int_{a}^{b} c  \, dx =c(b-a):c\in\mathbb{R}} 
$$
# Integral de suma de funciones o suma de integrales
$$
\boxed{\int_{a}^{b} f(x)\pm g(x) \, dx =\int_{a}^{b} f(x) \, dx \pm\int_{a}^{b} g(x) \, dx } 
$$

# Ponderación escalar
$$
\boxed{\int_{a}^{b} c·f(x) \, dx=c·\int_{a}^{b} f(x) \, dx  :c\in\mathbb{R}} 
$$
# Integral intermedia

Se puede tomar un valor entremedio del intervalo de integración, entonces así se puede separar una integral en dos integrales. Es decir:

$$
\boxed{\int_{a}^{b} f(x) \, dx=\int_{a}^{c}  f(x)\, dx+\int_{c}^{b}  f(x)\, dx  :a\leq c\leq b } 
$$

_Nota: esta propiedad es sumamente útil para calcular integrales en funciones a trozos_

![Pasted image 20240524130136.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/C%C3%A1lculo%20I/4%20La%20Integral/attachments/Pasted%20image%2020240524130136.png)

# Signo de integral por signo de función

Dada una función $f(x)\geq 0$, para $a\leq x \leq b$, entonces $\int_{a}^{b} f(x) \, dx\geq 0$

# Orden de integrales por orden de funciones

si $f(x)\geq g(x)$ para $a\leq x\leq b$, entonces $\int_{a}^{b} f(x) \, dx\geq \int_{a}^{b} g(x) \, dx$
