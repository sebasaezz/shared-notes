---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/operador-divergencia/","tags":["I3MAT1630"]}
---

# Definición
$$
\operatorname{div}\vec{F}=\frac{ \partial P }{ \partial x } +\frac{ \partial Q }{ \partial y } +\frac{ \partial R }{ \partial z } =\nabla·\vec{F}
$$
La divergencia también se puede definir de la siguiente forma:
$$
\nabla·\vec{A}=\lim_{ V \to 0 } \frac{\oint_{\mathcal{S}} \vec{A} \, ·\mathrm{d}\vec{s} }{V} \tag{1}
$$
En el caso bidimensional, la divergencia pasa a ser el flujo pero bidimensional.

$$
\nabla\cdot \vec{F}=\lim^{}_{ A \to 0 }  \frac{1}{A} \oint_\limits{\mathcal{C}} \vec{F} \, \mathrm{d}\vec{s} \tag{2}  
$$
Esto es el limite cuando el volumen tiende a cero del flujo sobre este volumen.

Si este volumen se multiplica en la ecuación, como una cantidad infinitesimal integrada, entonces se va a obtener el [[Cursos/Ingeniería Civil/2025-1/Cálculo III/3 Campos vectoriales e integrales de superficie/Teorema de la divergencia\|Teorema de la divergencia]]:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/teorema-de-la-divergencia/#cea925" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] teorema de la divergencia
> Sea $\mathcal{E}$ una región sólida simple, y sea $\mathcal{S}$ la frontera de $\mathcal{E}$, orientada positivamente ($\mathcal{S}=\partial \mathcal{E}$). Si es que $\vec{F}$ tiene derivadas continuas en un conjunto abierto que contiene a $\mathcal{E}$, entonces:
> $
> \iint_\limits{\mathcal{S}} \vec{F} ·\, \mathrm{d}\vec{s}=\iiint _\limits{\mathcal{E}}(\nabla·\vec{F})\,dV
> $

</div></div>


# Divergencia en otros sistemas de coordenadas
## Casos particulares
### Coordenadas polares
Se puede demostrar que la divergencia en coordenadas polares se calcula como:
$$
\boxed{\nabla\cdot \vec{F}=\frac{1}{r}\frac{ \partial  }{ \partial r } (r\vec{F}_{r})+\frac{1}{r}\frac{ \partial \vec{F}_{\theta} }{ \partial \theta } } 
$$
### Cilíndricas
Polares más el $z$:
$$
\boxed{\nabla\cdot \vec{F}=\frac{1}{r}\frac{ \partial  }{ \partial r } (r\vec{F}_{r})+\frac{1}{r}\frac{ \partial \vec{F}_{\theta} }{ \partial \theta } +\frac{ \partial \vec{F}_{z} }{ \partial z } } 
$$
### Esféricas
El tremendo cocodrilo:
$$
\boxed{\nabla\cdot \vec{F}=\frac{1}{r^{2}} \frac{ \partial  }{ \partial r } (r^{2}\vec{F}_{r})+\frac{1}{r\sin\theta} \frac{ \partial  }{ \partial \theta } (\vec{F}_{\theta}\sin\theta) +\frac{1}{r\sin\theta}\frac{ \partial \vec{F}_{\phi} }{ \partial \phi } }  
$$
_Nota:_ $\theta$ es el ángulo polar (el $\phi$ del Stewart)
## Generalización para cualquier [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Base ortogonal y ortonormal\|base ortogonal]] 

Se puede resolver una fórmula general para cualquier base ortogonal $(u, v, w)$ utilizando los [[Coeficientes de Lamé\|Coeficientes de Lamé]] $(h_{u},h_{v},h_{w})$. Estos de alguna forma indican la longitud de cada infinitesimal en un sistema de coordenadas. Al multiplicarlos entre ellos se obtendrá el [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.11 Geometría de transformaciones de R2 a R2. Matriz Jacobiana/Cambio de variables en integrales dobles\|jacoviano]].

Los mas comunes:
- Cartesianas: $h_{x}=h_{y}=h_{z}=1$
- Cilíndricas: $h_{r}=1, h_{\theta}=r, h_{z}=1$
- Esféricas: $h_{r}=1, h_{\theta}=r, h_{\phi}=r\sin \theta$

De aquí para obtener la divergencia:
$$
\nabla\cdot \vec{F}= \frac{1}{h_{u}h_{v}h_{w}}\left[ \frac{ \partial  }{ \partial u } (\vec{F}_{u}h_{v}h_{w})+\frac{ \partial  }{ \partial v } (h_{u}\vec{F}_{v}h_{w})+\frac{ \partial  }{ \partial w } (h_{u}h_{v}\vec{F}_{w}) \right]
$$

# Ejemplo