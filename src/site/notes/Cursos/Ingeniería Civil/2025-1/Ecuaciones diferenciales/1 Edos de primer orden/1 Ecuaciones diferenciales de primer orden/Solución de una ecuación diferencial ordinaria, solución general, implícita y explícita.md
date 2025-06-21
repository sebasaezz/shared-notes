---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/1-ecuaciones-diferenciales-de-primer-orden/solucion-de-una-ecuacion-diferencial-ordinaria-solucion-general-implicita-y-explicita/","tags":["I1MAT1640"]}
---

La solución de una ecuación diferencial será una función $u(x)=u$ tal que para un intervalo $I$ en ecuación general de la forma:
$$
F(x,y,y',y'',\dots,y^{(n)})=0 \tag{1}
$$
se tenga que:
$$
F(x,u,u',u'',\dots,u^{(n)})=0
$$
Formalmente, se dice que $u$ **satisface** a la ecuación diferencial $(1)$ en $I$.

Como se define en un mismo intervalo $I$, se puede dar confusión con la cantidad de soluciones de una ecuación
# Existencia y unicidad

# Tipos de soluciones
## Solución implícita
Tiene la forma:
$$
K(x,y)=0
$$

# Ejemplo
La ecuación:
$$
\frac{ dy }{ dx } =y^{2}
$$
tiene como _solución general_ a
$$
y=\frac{1}{C-x}
$$
ya que:
$$
\frac{ dy }{ dt } =\frac{0·(C-x)-1·(-1)}{(C-x)^{2}}=\left(\frac{1}{C-x}\right)^{2}=y^{2}
$$
Pero realmente son dos las soluciones obtenidas, ya que siempre va a haber una discontinuidad en $C$, resultando en una función en el intervalo $I_{1}=(-\infty,C)$ y la otra en $I_{2}=(C,\infty)$.
