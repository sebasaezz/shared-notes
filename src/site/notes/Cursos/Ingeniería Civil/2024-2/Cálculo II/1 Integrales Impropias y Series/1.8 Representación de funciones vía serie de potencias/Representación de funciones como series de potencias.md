---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-8-representacion-de-funciones-via-serie-de-potencias/representacion-de-funciones-como-series-de-potencias/","tags":["I2MAT1620"]}
---

# Concepto
Tomar una función, y representarla como serie de potencias.

Se va a cumplir la siguiente propiedad:
$$
\sum_{n=0}^{\infty}x^{n}=\frac{1}{1-x}:\lvert x \rvert<1 
$$
![Pasted image 20240904113452.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/1%20Integrales%20Impropias%20y%20Series/1.8%20Representaci%C3%B3n%20de%20funciones%20v%C3%ADa%20serie%20de%20potencias/attachments/Pasted%20image%2020240904113452.png)

De aquí, se puede reemplazar $x$ con cualquier expresión. Por ejemplo, si se quiere encontrar la serie para $f(x)=\frac{1}{x+2}$.
$$
\begin{align}
f(x) & =\frac{1}{2\left( 1-\left( -\frac{x}{2} \right) \right)} \\
 &=\frac{1}{2}\sum_{n=0}^{\infty}\left( -\frac{x}{2} \right)^{n} \\
 & =\frac{1}{2} \sum_{n=0}^{\infty}( -1 )^{n} \frac{x^{n}}{2^{n}} \\
 & =\sum_{n=0}^{\infty}(-1)^{n}\left( \frac{x^{n}}{2^{n+1}} \right)
\end{align}
$$
# Derivación de este teorema

> [!theorem] derivación e integración de funciones en su representación como serie
> Si la serie de potencias centrada en $a$ posee un radio $R>0$, entonces es continua y derivable en $(a-R,a+R)$. Ahora, derivando:
> $$
> f'(x)=c_{1}+2c(x-a)+3(x-a)^{2}+\dots=\sum_{n=0}^{\infty}nc_{n}(x-a)^{n-1}
> $$
> Y también se puede integrar:
> $$
> \begin{align}
> \int f(x) \, dx & = \int\!fx\,\operatorname{d}xC+c_{0}(x-a)+ c_{1}\frac{(x-a)^{2}}{2}+c_{2} \frac{(x-a)^{3}}{3}+\dots \\
>  
>  & =C+\sum_{n=0}^{\infty}c_{n} \frac{(x-a)^{n+1}}{x+1}
> \end{align}
> $$

Ahora se puede integrar la primera función ya vista ($\frac{1}{x-1}$) o derivar.
Por ejemplo:
$$
\begin{align}
\frac{1}{x-1} & =\sum_{n=0}^{\infty}x^{n} \\
\int \frac{1}{x-1} \, dx  & =\sum_{n=0}^{\infty} \frac{x^{n+1}}{x+1} \\
\ln \lvert x-1 \rvert+C  & =\sum_{n=0}^{\infty} \frac{x^{n+1}}{x+1}+C
\end{align}
$$


# Ejemplo