---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-1-vectores-y-geometria-del-plano-y-del-espacio-producto-punto/espacio-cartesiano/","tags":["I2MAT1620"]}
---

Se considera un espacio donde los puntos están definidos por las coordenadas $xyz$. Es un [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Espacio vectorial\|Espacio vectorial]] dado por $\mathbb{R}^{3}$.
Está dividido en 8 regiones llamadas octantes (antes eran cuadrantes).
# Distancia entre dos puntos 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/longitud-o-norma-de-un-vector-vector-unitario-y-distancia-entre-vectores/#812913" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!definition] distancia entre vectores
> $
> dist(v,u)=\lvert \lvert v-u \rvert  \rvert 
> $

</div></div>

Considerando la definicion de norma:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/longitud-o-norma-de-un-vector-vector-unitario-y-distancia-entre-vectores/#2b7762" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!definition] longitud o norma de un vector
> Gráficamente, es la longitud de un vector, matemáticamente se representa para $v\in\mathbb{R}^{n}$ como $\lvert \rvert v \rvert \rvert$ y se define como:
> $\lvert \lvert v \rvert  \rvert =\sqrt{ v_{1}^{2}+v_{2}^{2}+\dots+v_{n}^{2} }=\sqrt{ v·v }$
> Esto además implica que:
> $ \lvert \lvert v \rvert  \rvert ^{2}=v·v $
> y, con $c\in\mathbb{R}$
>$\lvert \lvert cv \rvert  \rvert=\lvert c \rvert· \lvert \lvert v \rvert  \rvert  $

</div></div>
 Así:
$$
\operatorname{Dist}((a,b,c);(d,e,f))=\sqrt{ (a-d)^{2}+(b-e)^{2} +(c-f)^{2}}
$$
# Planos y superficies
Una ecuación en la forma $Ax+By+C=0$, no representa una recta, sino un plano.
Toda ecuación en la forma $z=f(x,y)$ tendrá a $z$ como variable libre. Así, todo lo que se proyecta en el plano $xy$, tendrá los mismos valores para todo $z$. (un círculo se convierte en un cilindro y una recta en un plano).
```mathematica-plot 
raster:
  dim: 3D
  background: None
  size:
    height: Automatic
    width: "100"
general:
  axes: "True"
  axesLabel: "{x, y}"
  frame: "True"
  boxed: "True"
  plotLabel: Cilindro
  frameLabel: ""
graphs:
  - id: graph_0
    options:
      plotStyle: ""
    type: contourPlot
    contourPlot:
      expression: x^2+y^2==1
      domain:
        x:
          min: "-2"
          max: "2"
        y:
          min: "-2"
          max: "2"
        z:
          min: "-2"
          max: "2"

 ```

Ahora también se pueden aplicar ecuaciones que tengan sentido lógico, como la de la esfera unitaria:
$$
x^{2}+y^{2}+z^{2}=1
$$
```mathematica-plot 
raster:
  dim: 3D
  background: None
  size:
    height: Automatic
    width: "100"
general:
  axes: "True"
  axesLabel: "{x, y}"
  frame: "False"
  boxed: "True"
graphs:
  - id: graph_0
    options: {}
    type: contourPlot
    contourPlot:
      expression: x^2+y^2+z^2==1
      domain:
        x:
          min: "-2"
          max: "2"
        y:
          min: "-2"
          max: "2"
        z:
          min: "-2"
          max: "2"

 ```
O una esfera centrada en un punto $(a,b,c)$:
$$
(x-a)^{2}+(y-b)^{2}+(z-c)^{2}=r^{2}
$$
# Desigualdades
Ahora los objetos van a estar llenos.
Ejemplo:
$$
1\leq x^2+y^2+z^2\leq4
$$

<iframe width='800' height='400' src='https://www.wolframcloud.com/obj/4f4d7631-937e-4b71-8dba-6fd8f1189ee7' frameborder='0'></iframe>
 