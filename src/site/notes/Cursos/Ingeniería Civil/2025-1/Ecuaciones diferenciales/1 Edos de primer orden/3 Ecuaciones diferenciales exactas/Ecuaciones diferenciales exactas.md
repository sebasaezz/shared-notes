---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/3-ecuaciones-diferenciales-exactas/ecuaciones-diferenciales-exactas/","tags":["ExMAT1640"]}
---

# Forma de la ecuación exacta
La ecuación:
$$
M(x,y) dx+N(x,y)dy=0
$$
es equivalente a decir:
$$
M(x,y)+N(x,y) \frac{ dy }{ dx } =0 \tag{1}
$$
# Método con derivadas parciales
Idealmente, se quiere llegar de algo así a una forma implícita:
$$
F(x,y(x))=C
$$
Y si se deriva con respecto a $x$ ([[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.10 Composición de una función real de varias variables y una curva. Regla de la cadena/Regla de la cadena en dos variables\|cadena]]):
$$
\frac{ \partial  }{ \partial x } F(x,y(x))=F_{x}+F_{y} \frac{ dy }{ dx } 
$$
Esto tiene la misma forma que Ecuación 1.

> [!definition] ecuación diferencial exacta
> Una ecuación de la forma:
> $$
> M(x,y)+N(x,y)y'=0
> $$
> Es exacta si existe una función $F(x,y)$ que cumpla que:
> 
> - $F_{x}=M$
> - $F_{y}=N$
> 
> Además se debe cuplir que:
> $$
> F_{xy}=F_{yx}
> $$
> Por [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.8 Derivadas parciales de orden superior. Relación de Clairaut/Derivadas parciales de orden superior#^8db770\|teorema de Clairaut]] 
> De otra forma:
> $$
> M_{y}=N_{x}
> $$






> [!example]
> la ecuación: $ydx+xdy=0$ es equivalente a decir:
> $$
> y+xy'=0
> $$
> Según lo visto, se puede asociar las derivadas parciales:
> - $F_{x}=y$
> - $F_{y}=x$
> 
> Ahora se integran las dos funciones:
> 
> - $\int \frac{ \partial F }{ \partial x } \, dx=\int y \, dx=xy+C(y)$
> - $\int \frac{ \partial F }{ \partial y } \, dx=\int x \, dy=xy+D(x)$
> 
> De aquí la forma implícita para que se cumplan las derivadas parciales será:
> $$
> xy=C
> $$


## Cuando no funciona el método

> [!example]
> Para la ecuación:
> $$
> y'=y+e^{x}
> $$
> $$
> -y-e^{x}+y'
> $$
> - $F_{x}=-y-e^{x}$
> - $F_{y}=1$
> 
> Integrando:
> 
> - $\int -y-e^{x} \, dx=\boxed{-xy}-e^{x}+C(y)$
> - $\int 1 \, dy=y+D(x)$
> 
> El $-xy$ en la primera no puede ser $D(x)$, ya que depende de $y$, entonces no se puede usar el método. **No es exacta**.

# Como saber si es exacta

> [!theorem] teorema de ecuaciones diferenciales exactas
> Si se tiene la EDO:
> $$
> M(x,y)+N(x,y) \frac{ dy }{ dx } =0
> $$
> Suponiendo que $M$ y $N$ tienen derivadas parciales continuas de primer orden en $R=(a,b) \times (c,d)$
> Entonces la eso es exacta si y solo si $M_{y}=N_{x}$ en todo el rectángulo.

Volviendo al ejemplo anterior:

> [!example]
> Para la ecuación:
> $$
> -y-e^{x}+y'=0
> $$
> 
> - $M=-y-e^{x}\implies M_{y}=-1$
> - $N=1\implies N_{x}=0$
> 
> Como $M_{y}\neq N_{x}$, la ecuación no puede ser exacta.