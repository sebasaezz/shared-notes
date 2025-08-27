---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-8-derivadas-parciales-de-orden-superior-relacion-de-clairaut/derivadas-parciales-de-orden-superior/","tags":["I3MAT1620"]}
---

# Concepto
Para las direcciones simples ($y$ y $x$), las 
# Definición
Van a haber varias serivadas simples, y van a ser de la siguietne forma:
$$
f(x,y)\begin{cases}
\frac{ \partial f }{ \partial x } =f_{x}\begin{cases}
\frac{ \partial \frac{ \partial f }{ \partial x }  }{ \partial x }=  \frac{ \partial^{2} f }{ \partial x^{2} }= f_{xx}   \\
\frac{ \partial \frac{ \partial f }{ \partial y }  }{ \partial y } = \frac{ \partial^{2} f }{ \partial y \partial x } =f_{yx}
\end{cases}  \\
\frac{ \partial f }{ \partial y }=f_{y} \begin{cases}
\frac{ \partial \frac{ \partial f }{ \partial y }  }{ \partial x } = \frac{ \partial^{2} f }{ \partial x \partial y}  =f_{xy}\\
\frac{ \partial \frac{ \partial f }{ \partial y }  }{ \partial y } =\frac{ \partial^{2} f }{ \partial y^{2} } =f_{yy}
\end{cases}
\end{cases}
$$


> [!theorem] teorema de Clairuaut
> Sea $f$ definida en un disco $D$, que contiene al punto $(a,b)$. Si $f_{xy}$ y $f_{yx}$ son continuas en $D$, entonces:
> $$
> f_{xy}(a,b)=f_{yx}(a,b)
> $$
{ #8db770}


Si esto no se cumple, uno debe asumir que una de las dos segundas derivadas no es continua.

`\begin{proof}`
Considerando la diferencia:
$$
\Delta (h)=\left[f(a+h,b+h)-f(a+h,b)\right]-[f(a,b+h)-f(a,b)]
$$
Esto es lo mismo que definir una función $g(x)=f(x,b+h)-f(x,b)$, así:
$$
\Delta(h)=g(a+h)-g(a)
$$
Según el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Teorema de valor medio (TVM)#^0c1fb3\|TVM]] 
Asumiendo verdaderas las dos hipótesis, entonces va a existir un valor $c$ que sea tal que:
$$
g(a+h)-g(a)=g'(c)·h=h[f_{x}(c,b+h)-f_{x}(c,b)]
$$
_Nota:_ se deriva respecto a $x$ ya que la diferencia $a+h$ está en la primera variable de $f$.

Ahora, considerando que $c$ es fijo, se puede aplicar TVM de nuevo, llegando a un valor $d$ tal que:
$$
\underbrace{ f_{x}(c,b+h)-f_{x}(c,b) }_{ \frac{\Delta (h)}{h} }=f_{xy}(c,d)·h
$$
_Nota:_ se deriva respecto a $y$ ya que la diferencia $b+h$ está en la segunda variables de $f$.

De aquí, se puede reemplazar llegando a que:
$$
\Delta (h)=h^{2}f_{xy}(c,d)
$$
Pero como $c$ y $d$ se diferencian de $a$ y $b$ por $h$, si $h \to 0\implies(c,d)\to (a,b)$
$$
\lim_{ h \to 0 } \frac{\Delta(h)}{h^{2}}=\lim_{ (c,d) \to (a,b) } f_{xy}(c,d)=f_{xy}(a,b)
$$

Ahora, si se hace este mismo proceso pero alternando la definiciones de $h$, entonces se va a poder legar a la misma igualdad pero con la otra derivada.
Como el límite en $h$ será el mismo en las dos funciones (a pesar de que $h$ sea definido de formas diferentes, el límite tiene la misma forma y tiende a cero), entonces las derivadas serán iguales.
$$
\Delta (h)=[f(a+h,b+h)-f(a,b+h)]-[f(a+h,b)-f(a,b)]
$$
$$
\lim_{ h \to 0 } \frac{\Delta h}{h^{2}}=f_{yx}(a,b)=f_{xy}(a,b)
$$
Cumpliéndose que:
- $f$ es continua y derivable en un disco $D$ de centro $(a,b)$ (dado por $h$)
Y por efecto:
- $f_{x}$ es continua y derivable en $D$
- $f_{y}$ es continua y derivable en $D$
`\end{proof}`

# Ejemplo