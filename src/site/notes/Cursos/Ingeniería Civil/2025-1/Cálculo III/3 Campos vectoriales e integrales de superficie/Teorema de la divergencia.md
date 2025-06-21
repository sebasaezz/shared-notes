---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/teorema-de-la-divergencia/","tags":["I1MAT1630"]}
---

# Concepto
Es como una generalización del [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Campos conservativos/Teorema de Green\|teorema de green]] escrito es la [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Formas vectoriales del teorema de Green y flujo\|forma normal]]:
$$
\oint_\limits{\mathcal{C}} (\vec{F}·\hat{n}) \, \mathrm{d}s=\iint_\limits{\mathcal{D}} (\nabla·\vec{F}) \, \mathrm{d}A  
$$
El teorema de la divergencia, lo que hace es generalizar esta relación, pero como un volumen.
Ahora $\mathcal{S}$ es una superficie frontera de un volumen $\mathcal{E}$. Esta relación se extiende si el volumen $\mathcal{E}$ es una **región sólida simple**. Esto es una región que es simultáneamente de [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.1 Definición de integrales dobles para rectángulos en el plano. Integrales iteradas/Integrales dobles sobre regiones generales\|tipo I, tipo II y tipo III]]. Es decir, siempre se puede escribir en forma de gráficos en todas su direcciones (uno de sus límites está dado por una parametrización en números reales y el resto depende de ella).
# Definición

> [!theorem] teorema de la divergencia
> Sea $\mathcal{E}$ una región sólida simple, y sea $\mathcal{S}$ la frontera de $\mathcal{E}$, orientada positivamente ($\mathcal{S}=\partial \mathcal{E}$). Si es que $\vec{F}$ tiene derivadas continuas en un conjunto abierto que contiene a $\mathcal{E}$, entonces:
> $$
> \iint_\limits{\mathcal{S}} \vec{F} ·\, \mathrm{d}\vec{s}=\iiint _\limits{\mathcal{E}}(\nabla·\vec{F})\,dV
> $$

# Ejemplo
## Ejemplo 1
Encuentre el flujo de $\vec{F}(\vec{x})=\vec{x}$ sobre la esfera de radio $5$ centrada en el punto $(-1,1,1)$.
Sea $\mathcal{S}$ la esfera, se pide:
$$
\iint_\limits{\mathcal{S}} \vec{x} · \mathrm{d}\vec{s} 
$$
Pero la esfera es una región sólida simple, y la función es continua y derivable en todas partes. Entonces se aplica el teorema:
$$
\iint_\limits{\mathcal{S}} \vec{x} · \mathrm{d}\vec{s} =\iiint_\limits{B_{5}(-1,1,1)} (\nabla·\vec{x}) \, \mathrm{d}V 
$$
Donde $B_{5}(-1,1,1)$ es la bola sólida de radio $5$.
$$
\begin{align}
\nabla·\vec{x} & =\nabla·\langle x,y,z \rangle  \\
 & =1+1+1 \\
 & =3
\end{align}
$$
Entonces la integral se evalúa como 3 veces el volumen de la esfera.
$$
\begin{align}
\iiint_\limits{B_{5}(-1,1,1)} 3 \, \mathrm{d}V  & =3\left( \frac{4}{3}\pi·5 \right)  \\
 & =500\pi
\end{align}
$$
## Ejemplo 2 
Encuentre el flujo de $\vec{F}=\langle xy,y^{2}+\mathrm{e}^{ xz^{2} },\sin(xy) \rangle$ sobre la frontera de la región sólida determinada por el cilindro parabólico $z=1-z^{2}$, el plano $z=0$, el plano $y=0$ y el plano $y+z=2$.
![Pasted image 20250610084832.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250610084832.png)
Sea $\mathcal{S}$ esta superficie, que al rellenarla se obtiene $\mathcal{E}$, entonces:
$$
\begin{align}
\iint_\limits{\mathcal{S}}  \vec{F} · \mathrm{d}\vec{s} & =\iiint_\limits{\mathcal{E}} \nabla·\langle xy,y^{2}+\mathrm{e}^{ xz^{2} },\sin(xy) \rangle \, \mathrm{d}V  \\
 & =\iiint_\limits{\mathcal{E}} y+2y+0 \, \mathrm{d}V  \\
 & =\int_{-1}^{1}\int_{0}^{1-x^{2}}  \int_{0}^{2-z}  3y \, \mathrm{d}y \, \mathrm{d}z \,\mathrm{d}x  \\
 & =\frac{180}{35}
\end{align}
$$
## Ejemplo 3
Sea $E(\vec{x})=\mu \frac{\vec{x}}{\lvert \lvert \vec{x} \rvert \rvert^{3}}$ el campo eléctrico asociado a una carga en el origen. Muestre que si $\mathcal{S}$ es cualquier superficie que encierra dentro al origen, entonces:
$$
\iint_\limits{\mathcal{S}} E· \mathrm{d}\vec{s}=\mu4\pi 
$$
Notar que en $(0,0,0)$, $E$ se indefine. por esto se debe tomar una superficie que encierre al origen.
Se calcula la divergencia:
$$
\begin{align}
\nabla·E & =\mu\left( \frac{3(x^{2}+y^{2}+z^{2})^{3/2}-3(x^{2}+y^{2}+z^{2})(x^{2}+y^{2}+z^{2})^{1/2}}{(x^{2}+y^{2}+z^{2})^{3}} \right) \\
 & =\mu(3(x^{2}+y^{2}+z^{2})^{3/2-3}-3(x^{2}+y^{2}+z^{2})^{3/2-3}) \\
 & =0
\end{align}
$$
Se asume que existe una bolita de radio $\epsilon$ que contiene al origen la cual se le va a restar a la superficie para obtener un solido que no se indefine en ningún punto.
El teorema de la divergencia aplica en la región $\mathcal{E}$ cuya frontera es $\mathcal{S} \cup\partial B_{\epsilon}$
Es importante que la bolita se debe tomar con una normal que mira hacia adentro, mientras que $\mathcal{S}$ tiene la normal que mira hacia afuera. Entonces, por teorema de la divergencia:
$$
\begin{align}
\iint_\limits{\mathcal{S}} E · \mathrm{d}\vec{s}  &= \iint_\limits{\mathcal{S}} E· \mathrm{d}\vec{s}+\iint_\limits{\partial B_{\epsilon}} E· \mathrm{d}\vec{s}- \iint_\limits{\partial B_{\epsilon}} E· \mathrm{d}\vec{s}  \\
 & =\iint_\limits{\mathcal{S\cup \partial B_{\epsilon}}} E · \mathrm{d}\vec{s} -\iint_\limits{\partial B_{\epsilon}} E· \mathrm{d}\vec{s} \\
 & =\cancelto{ 0 }{ \iiint_\limits{\mathcal{E}} (\nabla·E) \, \mathrm{d}V } -\iint_\limits{\partial B_{\epsilon}} E·\mathrm{d}\vec{s} \\
 & =-\iint_\limits{\partial B_{\epsilon}} E· \mathrm{d}\vec{s} \\
\end{align}
$$
Esto se despeja, recordando que la bola estaba recorrida en dirección negativa, entonces el menos se tacha.


