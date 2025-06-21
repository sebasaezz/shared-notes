---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/2-ecuaciones-diferenciales-homogeneas/ecuacion-de-bernoulli-edo/","tags":["ExMAT1640"]}
---

Básicamente cuando se tiene un $y$ grado $1$ y otro grado $n$ y nada más. 
Tener una ecuación que no es lineal solo por un factor.

$$
\begin{align}
\frac{ dy }{ dx }  & =P(x)y+Q(x)y^{n} \\
\frac{1}{y^{n}} \frac{ dy }{ dx }  & =P(x)\underbrace{ y^{1-n} }_{ u }+Q(x) 
\end{align}
$$
- $u=y^{1-n}$
- $\frac{ du }{ dx }=(1-n)y^{-n} \frac{ dy }{ dx }$
$$
\frac{1}{1-n} \frac{ du }{ dx } =P(x)u+Q(x) \leftarrow \text{lineal}
$$


# Ejemplo
$$
\begin{align}
0 & =y'+y+e^{x}y^{2} 
\end{align}
$$