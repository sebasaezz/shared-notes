---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/2-gases-ideales/indice-adiabatico/","tags":["I2IIQ1003"]}
---


Es la relación entre [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/5 Calorimetría/Calorimetría, capacidad calorífica y calor latente\|calores específicos]] de volumen y de presión constante de un [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Modelo de gases ideales\|gas ideal]].
$$
\gamma=\frac{C_{p}}{C_{v}}
$$
*con los valores de $C_{p}$ y $C_{v}$ constantes*
Muchos fenómenos dependen de él, como la [[Velocidad del sonido\|Velocidad del sonido]]. En general, depende del tipo de gas y de la temperatura, aunque a cambios pequeños de temperatura permanece constante.

Se usa principalmente en cálculos de [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Procesos adiabáticos reversibles en gases ideales\|Procesos adiabáticos reversibles en gases ideales]].


# Proceso de Clément y Désormes
Son dos procesos que ocurren en un recipiente de gran volumen.
- Estado inicial: Se aumenta la presión ingresando aire al sistema
- Estado intermedio (proceso 1): Se produce una expansión adiabática. Disminuye la presión al dejar escapar aire.
- Estado final (proceso 2): Un proceso [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/1 Fundamentos de la termodinámica/Procesos termodinámicos\|isocórico]]. Luego de la expansión, aumenta la presión pero son cambiar el volumen.
## Laboratorio de termodinámica
Se usa un [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Manómetro de dos ramas abiertas\|Manómetro de dos ramas abiertas]] donde:
$$
P\approx P_{0}+\rho_{m} gh
$$
Con $h$ la diferencia de alturas de agua en el manómetro y $P_{0}=P_{atm}$. 

### Proceso inicial ($P_{1},v_{1},T_{1}$)
Se llega a una presión inicial levemente mayor que la atmosférica $P_{1}$ y se mide $h_{1}$. 
### Proceso intermedio ($P_{0},v_{0},T_{2}$)
Se libera aire **rápidamente** para evitar intercambio de calor. Hasta alcanzar presión $P_{0}$. Se llega a un volumen específico $v_{0}$ mayor que $v_{1}$. Y se usa:
$$
P_{1}v_{1}^{\gamma} = P_{0}v_{0}^{\gamma}
$$
La expansión disminuye la temperatura del aire, a una temperatura menor a la ambiental $T_{2}$.

### Proceso final ($P_{2},v_{2},T_{1}$)
El sistema absorbe energía hasta llegar a $T_{1}$ y aumentando su presión a $P_{2}$ (registrar $h_{2} <h_{1}$). El volumen se mantiene constante, $v_{2}=v_{0}$.

Con esta información ya se va a poder despejar $\gamma$, llegando a que:
$$
\gamma=\frac{h_{1}}{h_{1}-h_{2}}
$$
