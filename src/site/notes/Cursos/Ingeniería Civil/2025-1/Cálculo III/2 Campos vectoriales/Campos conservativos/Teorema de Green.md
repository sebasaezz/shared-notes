---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/campos-conservativos/teorema-de-green/","tags":["I1MAT1630"]}
---

Orientación de una curva:
- Positiva: Antihorario
- Negativa: Horario
# Definición

> [!theorem] teorema de Green
> Sea $\mathcal{C}$ una curva cerrada simple, suave posiblemente a trozos y orientada de manera positiva (antihorario). Sea $\mathcal{D}$ el dominio delimitado por $\mathcal{C}$ ($\mathcal{C}=\partial \mathcal{D}$) y sean $P$ y $Q$ funciones con derivadas parciales continuas en un dominio abierto que contiene a $D$.
> 
> Entonces:
> $$
> \oint_{\mathcal{C}} \langle P,Q \rangle·d\vec{r} =\oint _{\mathcal{C}} P \, dx +Q\,dy=\iint _{\mathcal{D}} \left( \frac{ \partial Q }{ \partial x } -\frac{ \partial P }{ \partial y }  \right) \, dA 
> $$

La derivada de la forma diferencial dentro de la primera integral es lo que está en la segunda integral. De otra forma:
$$
\int _{\partial D}f =\int _{D} \, df  
$$
	Esto es el [[Teorema de Stokes generalizado\|Teorema de Stokes generalizado]], sin embargo, el teorema de Green se puede ver como un caso del [[Cursos/Ingeniería Civil/2025-1/Cálculo III/3 Campos vectoriales e integrales de superficie/Teorema de Stokes\|Teorema de Stokes]], ya que lo que está dentro de la integral doble puede verse como:
$$
\nabla \times \langle P,Q,0 \rangle =\begin{vmatrix}
\hat{\imath} & \hat{\jmath} & \hat{k} \\
\partial_{x} & \partial_{y} & \partial_{x} \\
P & Q & 0
\end{vmatrix}=\langle 0,0,\partial_{x}Q-\partial_{y}P \rangle 
$$
Donde $\nabla$ es el operador gradiente $\nabla=\langle \partial _{x}, \partial_{y}, \partial_{z} \rangle$ que opera como [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Rotacional\|Rotacional]].
Esto se generaliza más adelante.
# Por regiones

Se va a cumplir para [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.1 Definición de integrales dobles para rectángulos en el plano. Integrales iteradas/Integrales dobles sobre regiones generales\|dominios de tipo I]]:
$$
\int P \, dx =-\int _{D} \frac{ \partial P }{ \partial y }  \, dA 
$$

Para regiones de tipo II
$$
\int _{C}Q \, dy =\int _{D}\frac{ \partial Q }{ \partial x }  \, dA 
$$
# Uso del teorema para calcular áreas
Se sabe que se pueden [[Cursos/Ingeniería Civil/2024-2/Cálculo II/3 Integrales Múltiples/3.1 Definición de integrales dobles para rectángulos en el plano. Integrales iteradas/Integrales dobles sobre regiones generales#^87cb72\|usar integrales dobles para calcular áreas]], de forma que:
$$
\iint_{D}1\,dA=\operatorname{area}(D)
$$
Se puede revertir el teorema de green, para encontrar funciones $P$ y $Q$ tales que:
$$
\left( \frac{ \partial Q }{ \partial x } -\frac{ \partial P }{ \partial y }  \right)=1
$$
Esto usualmente se logra con las combinaciones:
$$
\begin{align}
P & =0 & P & =-y & P & =-\frac{1}{2}y \\
Q & =x & Q & =0 & Q & =\frac{1}{2}x
\end{align}
$$
Aplicando el teorema, se llega al siguiente corolario:

> [!corollary]
> Se puede expresar el área $A$ de una región $\mathcal{D}$ por medio del teorema de Green:
> $$
> A=\oint_{\partial \mathcal{D}}x\,dy=-\oint_{\partial \mathcal{D}}y\,dx=\frac{1}{2}\oint_{\partial \mathcal{D}}-y\,dx+x\,dy
> $$
> Recordar que $\partial \mathcal{D}$ es la región $\mathcal{C}$ que es el contorno de $\mathcal{D}$

# Ejemplo