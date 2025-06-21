---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/1-ecuaciones-diferenciales-de-primer-orden/resolucion-de-ed-os-separables/","tags":["I1MAT1640"]}
---

# Nivel 0, ecuaciones explícitas?
$$
\frac{ dy }{ dx } =\underbrace{ f(x) }_{ \text{conocida} }
$$
Se resuelve integrando, es decir:
$$
y=F(x)+C
$$
Con $F(x)$ la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Antiderivada particular\|Antiderivada particular]] de $f$.
# Ecuaciones diferenciales separables (Nivel 1)

> [!definition] EDO separable
> Una ecuación diferencial separable tiene la forma:
> $$
> \frac{ dy }{ dx } =F(x)·G(y)=\frac{F(x)}{H(y)}
> $$

Recordando el [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.11 Geometría de transformaciones de R2 a R2. Matriz Jacobiana/Cambio de variables en integrales dobles\|cambio de variable]]:
Si se tiene:
$$
\int F(y) \, dy 
$$
Que pasa si $y:=y(x)$.
Entonces, por [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.10 Composición de una función real de varias variables y una curva. Regla de la cadena/Regla de la cadena en dos variables\|regla de la cadena]]:
$$
\int F(y) \, dy =\int F(y(x)) \frac{ dy }{ dx }  \, dx 
$$
Entonces si se tiene algo como:
$$
\begin{align}
\frac{ dy }{ dx }  & =y \\
\frac{1}{y} \frac{ dy }{ dx }  & =1 \\
\int \frac{1}{y} \frac{ dy }{ dx }  \, dx  & =\int  \, dx =x+C \\
\int \frac{dy}{y}  & =x+C \\
\ln \lvert y \rvert  & =x+C_{1} \\
e^{\ln \lvert y \rvert } & =e^{x+C_{1}} \\
\lvert y \rvert  & =C_{2}e^{x} :C_{2}>0 
\end{align}
$$
# Método general
Si se tiene:
$$
\begin{align}
\frac{ dy }{ dx } =\frac{F(x)}{G(y)}  & \iff G(y) \frac{ dy }{ dx } =F(x) \\
 & \iff \int G(y) \, dy =\int F(x) \, dx \\
  & \iff \boxed{H(y)=A(x)+C} \leftarrow\text{solución implícita} 
\end{align}
$$

## Ejemplo
### ejemplo 1  
$$
x+y\frac{ dy }{ dx } =0
$$
Tiene como solución implícita a:
$$
y^{2}+x^{2}=C
$$
Pero esto no es una función. Y realmente hay dos soluciones generales:
$$
y(x)=\pm \sqrt{ C-x^{2} }
$$

### Ejemplo 2
$$
\begin{align}
\frac{ dy }{ dx } =\frac{4-2x}{3y^{2}-5} & \iff \int 3y^{2}-5 \, dy =\int 4-2x \, dx   \\
 & \iff y^{3}-5y=4x-x^{2}+C
\end{align}
$$
