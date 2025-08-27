---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/3-integrales-multiples/3-10-coordenadas-esfericas-calculo-de-integrales-triples-utilizando-coordenadas-cilindricas-y-esfericas/coordenadas-esfericas/","tags":["I2MAT1620"]}
---

# Concepto
Van a haber dos ángulos $\theta$ (proyección con eje $xy$) y $\phi$ (proyección con eje $zy$) , y un radio $\rho$.
$\theta$ varía de $0$ a $\pi$
$\phi$ varía de $0$ a $\pi$, para que no se repita la región.

Para la proyección e $x$, va a haber un $r=\rho \sin \phi$. De esta forma:
- $x=\rho \sin \phi \cos\theta$
- $y=\rho \sin \phi \sin \theta$
- $z=\rho \cos \phi$

# Vectores unitarios
Se puede trabajar con vectores unitarios al usar estas coordenadas, con las siguientes equivalencias:
$$
\begin{cases}
\hat{r} & = & \sin\theta \cos \phi \,\hat{x} + \sin\theta \sin \phi\, \hat{y}+\cos\theta\,\hat{z} \\
\hat{\theta} & =  & \cos\theta \cos \phi\, \hat{x}+\cos\theta \sin \phi\, \hat{y}-\sin\theta\, \hat{z} \\
\hat{\phi} & = & -\sin\, \hat{x}+\cos \phi\,\hat{y}
\end{cases}
$$
Importante: Para vectores unitarios, normalmente se usa la convención más usada en física, donde $r=\rho$, $\theta=\phi$ y $\phi=\theta$. Es decir, $\theta$ es el ángulo polar (de $0$ a $\pi$) y $\phi$ es azimutal (de $0$ a $2\pi$). En estas ecuaciones se usa esa convención.
# Definición
# Ejemplo