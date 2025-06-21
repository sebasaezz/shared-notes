---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/3-ecuaciones-diferenciales-exactas/reduccion-de-orden-de-ed-os/","tags":["ExMAT1640"]}
---

Una ecuación sin un $y$ se puede reducir reemplazando $p=y'$.

> [!example]
> 
> $$
> xy''+2y'=6x
> $$
> Se dice $p=y'$, entonces:
> $$
> \begin{align}
> xp'+2p & =6x \\
> p' & =-\frac{2}{x}p+6
> \end{align}
> $$
> Ahora se resuelve con [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/EDOs lineales de primer orden y factor integrante\|factor integrante]] y se integra el resultado.

# Cuando falta el $x$
Se debe poner todo en términos de $y$ 

$$
yy''=(y')^{2}
$$
Se define $p=y'$
Por regla de la cadena:
$$
y''=\frac{ dp }{ dx } =\frac{ dy }{ dx } \frac{ dp }{ dy } =p \frac{ dp }{ dy } 
$$
Entonces:
$$
y\left( p \frac{ dp }{ dy }  \right)=p^{2}
$$
Si $p=0$ entonces $y=C$ es la solución, para $p\neq 0$:
$$
y \frac{ dp }{ dy } =p
$$
Esta es una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Resolución de EDOs separables\|separable]] y se logra integrando.