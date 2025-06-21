---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/6-ciclo-rankine/ciclo-de-rankine/","tags":["ExIIQ1003"]}
---

Es un [[Cursos/Ingeniería Civil/2025-1/Termodinámica/6 Ciclo Rankine/Ciclos de Potencia\|Ciclos de Potencia]]
# Ciclo básico
Tiene cuatro partes principales

- Hervidor, caldera o generador de vapor
- Turbina
- Condensador
- Bomba

Se espera que el trabajo de la turbina sea mayor al de la bomba.

![Pasted image 20250602084044.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250602084044.png)

![Pasted image 20250602083824.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250602083824.png)
Lo importante de este gráfico es reconocer que hay dos isobaras. una que trabaja por el lado del condensador y otra por el del hervidor.

Si en la bomba se tiene vapor, puede cavitar y dañarse. Lo mismo con la turbina, si tiene liquido se puede dañar.
## Balance de energía
En una situación ideal cerrada:
$$
Q_{B}+Q_{C}+W_{T}+W_{P}=0
$$
El trabajo será:
$$
W=W_{T}+W_{P}
$$
	Esto da un valor negativo, por que sale.
De otra forma:
$$
W=W_{T}-\lvert W_{P} \rvert 
$$
	Esto da un número positivo, pero se habla de trabajo que sale.

De cualquier forma:
$$
\eta=\frac{\lvert W \rvert }{\lvert Q_{B} \rvert }
$$
Todos estos trabajos y calores van a estar dados simplemente por el $\Delta h$ de cada fase.

## Balance de entropía
$$
S_{\text{gen}}=-\frac{Q_{B}}{T_{B}}-\frac{Q_{C}}{T_{C}}
$$
Resolviendo para $Q_{C}$, y reemplazando la eficiencia se va a tener:
$$
\eta=\underbrace{ 1- \frac{T_{C}}{T_{B}} }_{ \eta_{\text{carnot}} }-\frac{T_{C}S_{\text{gen}}}{Q_{B}}
$$
Notar que como se había predicho en [[Cursos/Ingeniería Civil/2025-1/Termodinámica/3 Ciclos termodinámicos/Ciclo de Carnot\|Ciclo de Carnot]], la eficiencia es menor a $\eta_{\text{carnot}}$.

## Modificaciones

Disminuir la presión del condensador aumenta la cantidad de trabajo, pero puede disminuir la calidad dentro de la turbina, lo cual puede causar problemas:

![Pasted image 20250602085459.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250602085459.png)
	Como se ve, aumenta el área, pero $4'$ cae con baja calidad.

Sobrecalentar el vapor también puede aumentar el trabajo neto, pero también puede requerir más $Q_{B}$, entonces se debe encontrar un equilibrio.
![Pasted image 20250602085637.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250602085637.png)

Aumentar la presión de la caldera aumenta también el rendimiento (trabajo), pero nuevamente puede aumentar la humedad en $4'$.

![Pasted image 20250602085815.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250602085815.png)
# Rankine con recalentamiento

Tiene una turbina dividida en dos secciones
Antes de generar la caída completa de presión, el fluido se saca y se recalienta en la caldera.
![Pasted image 20250604083902.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250604083902.png)
Ahora se van a tener 3 presiones. Como se ve, el área interior es mayor.
Que pasa con $\eta$? $Q_{H}$ se divide en cos componentes, el calor que se le entrega a la caldera, y el calor del recalentamiento. En la imagen:
$$
Q_{H}=Q_{61}+Q_{21}
$$
$$
W_{\text{neto}}=W_{T_{1}}+W_{T_{2}}-W_{P}
$$
$$
\eta=\frac{W_{{T_{1}}}+W_{T_{2}}-W_{P}}{Q_{61}+Q_{23}}
$$

# Generación con intercambiador cerrado
Se tiene en la turbina una desviación de flujo dada por una constante $y$.
Esta desviación de flujo se va a un intercambiador de calor cerrado
![Pasted image 20250604085300.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250604085300.png)
# Generación con intercambiador abierto
Lo mismo, pero con un intercambiador que mezcla dos flujos. Comp un mezclador adiabático.
![Pasted image 20250604085524.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/6%20Ciclo%20Rankine/attachments/Pasted%20image%2020250604085524.png)
