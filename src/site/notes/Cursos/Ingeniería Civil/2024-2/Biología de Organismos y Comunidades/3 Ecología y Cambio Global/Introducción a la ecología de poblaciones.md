---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/biologia-de-organismos-y-comunidades/3-ecologia-y-cambio-global/introduccion-a-la-ecologia-de-poblaciones/","tags":["P3BIO110C","C5BIO110C"]}
---

Dar cuenda de dinámicas poblacionales, explicando su diversidad y complejidad a través de reglas, principios y relaciones que evoquen procesos ecológicos.
# Población

> [!definition] población local
> Conjunto de organismos de una misma especie que habitan en un mismo tiempo y lugar.

El concepto de población, y la razón por la que se restringe en especie y tiempo, es por que una población se caracteriza por su reproducción.

La población donde todos los organismos conviven en el mismo lugar, es una población local, pero la definición de población no se restringe al mismo lugar.

## Cómo identificar una población
Se pueden identificar analizando la estructura genética. Si bien son la misma especie, la cada población se caracteriza por su reproducción exclusiva.

## Escalas de definición de unidades poblacionales
La definición de población es arbitraria al investigador, y se muestran patrones clasificados como:
- Parches
- Poblaciones
- Meta-poblaciones
![Pasted image 20241022151813.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241022151813.png)
## Tipos de poblaciones
Población dependiente: sumidero
población independiente
población temporal: fuente-sumidero
# Dinámica de poblaciones
## Uso de modelos
Representaciones simples de la realidad, se usan muchos modelos matemáticos para formular principios, leyes o postulados.
Principios de selección de modelos:
- Generalidad
	- 
- Realismo
	- El método usado está basado en la realidad?
- Precisión
	- Los resultados están correctos?
## Principios de dinámica de poblaciones
### Principio Malthusiano
Hay dos postulados:
- Los recursos son necesarios
- Las necesidades de una población son infinitas
	- Ya que crece de forma exponencial
Ecuaciones de cambio poblacional para tiempo discreto.
- $\Delta N=N_{t}-N_{0-1}$: Diferencia de población, población 
- $\Delta N=$ nacimientos ($BN_{0-1}$) - muertes ($DN_{0-1}$)
- $\Delta N=BN_{0-1}-DN_{0-1}$
De todo esto se puede concluir que:
$$
N_{t+1}=N_{t}\lambda
$$
$$
\implies\lambda=\frac{N_{t+1}}{N_{t}}
$$
De aquí se define a la tasa per cápita de cambio $R$ como el logaritmo de la tasa finita de cambio poblacional $\lambda$.
$$
R=\log\left( \frac{N_{t+1}}{N_{t}} \right)=\log\lambda
$$
$$
N_{t+1}=N_{t}e^{R}
$$
Según el crecimiento planteado por Malthus, $R$ es constante. Esto cambia al consdiderar los otros principios. 
### Cooperación
Si los individuos cooperan, entonces a medida que hay más individuos, la tasa de crecimiento ($R$) debe aumentar.

Considerando una población $N$ depredada por otra $Y$. Ahora se tendrá, por ejemplo, una tasa de depredación $D_{N}$ dada por:
$$
D_{N}= \frac{wY}{N}
$$
Ahora, esta tasa se le debe restar a la tasa de de cambio malthusiano $R_{m}$.
$$
N_{t+1}=N_{t}e^{R-D_{N}}=N_{t}e^{R- \frac{wY}{N_{t}}}
$$
![Pasted image 20241022155745.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241022155745.png)
Un ejemplo de ese crecimiento hiper-exponencial es el crecimiento humano, dada cosas como la revolución industrial.

### Competencia
Visión inversa. Ahora hay procesos que en vez de aumentar el valor de $R$, lo can a disminuir. En el mismo ejemplo anterior, se puede plantear que la taza de crecimiento de $Y$ va a depende de cuanto $N$ puede depredar. Así la tasa va a disminuir conforme $Y$ aumenta (empiezan a competir).
Ahora se va a tener $R_{t}=R- \frac{nY_{t}}{D}$
$$
Y_{t+1}=Y_{t}e^{R- \frac{nY_{t}}{D}}
$$
Donde $D$ es la densidad de $N$.
Se define a un valor $K$ como la ==capacidad de carga==, siendo el valor de $Y_{t}$ para el que $R_{t}$ sea nulo.
Capacidad de carga: Máximo tamaño de población que el ambiente puede soportar, _no es el máximo tamaño que el ambiente puede alcanzar_.
![Pasted image 20241022160820.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241022160820.png)
# Interacciones entre poblaciones


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/biologia-de-organismos-y-comunidades/3-ecologia-y-cambio-global/interacciones-entre-poblaciones/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




Si una población $A$ interactúa con $B$, cada una con un _fitness_ $\omega_{A}$ y $\omega _{B}$.
![Pasted image 20241024150421.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024150421.png)
- Depredación/parasitismo
	- Disminuyen el fitness de una a costa de la otra
	- Herbivoría es un caso especial de depredación, ya que puede ser una depredación modular.
	- Parasitismo
		- No hay mortalidad
		- Hay disminución en el _fitness_ del huesped.
		- Parasitoidismo
			- El adulto es de vida libre, pero la larva es libre.
- Competencia
	- Las dos se ven perjudicadas en _fitness_
	- Produce desarrollo de adaptaciones de defensa y ataque.
- Mutualismo
	- Las dos se ven beneficiadas en _fitness_. Por ejemplo, abejas y plantas con flores.
	- Puede producir diversificación evolutiva.
- Interacciones neutrales
	- Amensalismo
	- Comensalismo
	- Neutralismo
# Factores ambientales y principio consumidor-recurso
Cuando el ambiente, recurso/amenaza afecta a la población 
![Pasted image 20241024152003.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024152003.png)
## No-reactivos
El ambiente afecta directamente a la población y el ambiente no es afectado por el tamaño poblacional.
## Reactivos
El ambiente afecta a la población, pero la población afecta a el ambiente.
Esto genera dinámicas más complejas.
Como los dos tamaños poblacionales depende de cada uno, van a suceder ciclos. Estos son los ciclos de Lotka-Volterra.
![Pasted image 20241024152740.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024152740.png)

# Tipos de respuestas funcionales de Holling
Antes se planteó una tasa de depredación, pero ahora existen varias respuestas
Lo que se tiene son distintas funciones que conectan la abundancia de la presa con la eficiencia del depredador. 
## Tipo I
El depredador no se satisface en el tiempo de manipulación, no es sostenible. El depredador alcanza una saturación.
![Pasted image 20241024154421.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154421.png)
![Pasted image 20241024154516.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154516.png)
## Tipo II![Pasted image 20241024154421.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154421.png)
Supone un tiempo de manipulación. Hay un limitante de la tasa de consumo.
![Pasted image 20241024154434.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154434.png)
![Pasted image 20241024154534.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154534.png)
## Tipo III
Se tiene una fase acelerada inicial, debido a la formación de una imagen de búsqueda
![Pasted image 20241024154445.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154445.png)
![Pasted image 20241024154551.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241024154551.png)
- [x] no entendí nada  [completion:: 2025-04-20]
# Competencia interespecífica
De la misma forma vista en 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/biologia-de-organismos-y-comunidades/3-ecologia-y-cambio-global/introduccion-a-la-ecologia-de-poblaciones/#competencia" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Competencia
Visión inversa. Ahora hay procesos que en vez de aumentar el valor de $R$, lo can a disminuir. En el mismo ejemplo anterior, se puede plantear que la taza de crecimiento de $Y$ va a depende de cuanto $N$ puede depredar. Así la tasa va a disminuir conforme $Y$ aumenta (empiezan a competir).
Ahora se va a tener $R_{t}=R- \frac{nY_{t}}{D}$
$
Y_{t+1}=Y_{t}e^{R- \frac{nY_{t}}{D}}
$
Donde $D$ es la densidad de $N$.
Se define a un valor $K$ como la ==capacidad de carga==, siendo el valor de $Y_{t}$ para el que $R_{t}$ sea nulo.
Capacidad de carga: Máximo tamaño de población que el ambiente puede soportar, _no es el máximo tamaño que el ambiente puede alcanzar_.
![Pasted image 20241022160820.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Biolog%C3%ADa%20de%20Organismos%20y%20Comunidades/3%20Ecolog%C3%ADa%20y%20Cambio%20Global/attachments/Pasted%20image%2020241022160820.png)

</div></div>


Si dos poblaciones $Y$ e $Y_{1}$ compiten entre ellas, se da una competencia intraespecífica. Dos competidores pueden compartir un nicho fundamental, dando dos nichos realizados. 
# Mutualismo


</div></div>
