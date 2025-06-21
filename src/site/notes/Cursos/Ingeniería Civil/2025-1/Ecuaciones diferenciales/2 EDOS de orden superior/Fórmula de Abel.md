---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/2-edos-de-orden-superior/formula-de-abel/","tags":["I2MAT1640"]}
---


> [!theorem] fórmula de Abel
> Si se tiene una EDO de la forma:
> $$
> y''+p(x)y'+q(x)y=0
> $$
> Si se conoce una solución particular $y_{1}$, se puede obtener la segunda solución usando que:
> $$
> y_{2}(x)=y_{1}(x) \int \frac{e^{\int -p(x) \, dx }}{(y_{1}(x))^{2}} \, dx 
> $$ 


`\begin{proof}`
Se puede hacer el cambio $y=y_{1}(x) z(x)$ tal que $z(x)=\int u \, dx$.
Así, se tiene:
- $y'=y_{1}'z+y_{1}z'$
- $y''=y_{1}''z+2y_{1}'z'+y_{1}z''$
Reemplazando, y sabiendo que como $y_{1}$ es solución particular se cumple que: $y_{1}''+py'+qy=0$:
$$
\begin{align}
(y_{1}''z+2y_{1}'z'+y_{1}z'')+p(y_{1}'z+y_{1}z')+q(y_{1}z) & =0 \\
z\cancelto{ 0 }{ (y_{1}''+py_{1}'+qy_{1}) }+2y_{1}'z'+y_{1}z''+py_{1}z' & =0 \\ 
2y_{1}'z'+y_{1}z''+py_{1}z' & =0
\end{align}
$$
Como $z=\int u \, dx$, $z'=u$ y $z''=u'$.
$$
\begin{align}
u(2y_{1}'+py_{1})+y_{1}u' & =0 \\
\frac{ du }{ dx }  & =-\frac{u(2y_{1}'+py_{1})}{y_{1}} \\
\int  \, \frac{du}{u}  & =-\int 2\frac{y_{1}'}{y_{1}}+p \, dx  \\
\ln u  & =-\ln y_{1}^{2}-\int p \, dx  \\
 e^{\ln u+\ln y_{1}^{2}} & =-\int p \, dx  \\
uy_{1}^{2} & =-\int p \, dx  \\
u & =\frac{e^{-\int p \, dx }}{y_{1}^{2}} \\
z & =\int \frac{e^{-\int p \, dx }}{y_{1}^{2}} \, dx  \\
y & =y_{1}\int \frac{e^{-\int p \, dx }}{y_{1}^{2}} \, dx
\end{align}
$$
$y$ es otra solución $y_{2}$.
`\end{proof}`


# Ejemplo