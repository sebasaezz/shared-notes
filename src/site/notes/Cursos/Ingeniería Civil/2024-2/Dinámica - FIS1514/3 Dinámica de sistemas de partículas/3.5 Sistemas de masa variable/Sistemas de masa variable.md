---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/3-dinamica-de-sistemas-de-particulas/3-5-sistemas-de-masa-variable/sistemas-de-masa-variable/","tags":["ExFIS1514"]}
---

# Concepto
Cohetess
# Definición
Considerando un dispositivo como un cohete, que expulsa masa.
Se considera a $m$ a la masa en un instante, $\vec{v}$ su velocidad en el mismo instante, expulsando también una masa $m_{e}$ a una velocidad $\vec{v}_{e}$.

En un intervalo $dt$, existe un aumento de velocidad $d\vec{v}$ dado que expulsa una masa $dm_{e}$.

$$
\underbrace{ mv-m_{e}v_{e} }_{ p_{i} }+\underbrace{ \sum_{}^{}F_{\text{ext}}dt }_{ I }=\underbrace{ (m-dm_{e})(v+dv)-(m_{e}+dm_{e})v_{e} }_{ p_{f} }
$$
$$
\sum_{}^{}F_{\text{ext}}=m \frac{ dv }{ dt } -(v+v_{e})\frac{ dm_{e} }{ dt } =\boxed{m \frac{ dv }{ dt } -v_{D/e}\frac{ dm_{e} }{ dt } } 
$$
# Ejemplo