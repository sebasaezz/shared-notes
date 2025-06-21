---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/unidad-1/6-balance-en-sistemas-abiertos/balance-en-sistemas-abiertos/","tags":["I1IIQ1003"]}
---

Existe intercambio de materia y energía por medio de **corrientes de flujo**.
Un flujo puede operar de dos modos:

- **Estacionario:** Implica un flujo constante de materia o energía, de forma que no haya un cambio neto. Se considera un caso particular para una ecuación de estados no estacionarios.
- **No estacionario:** La mayoría de los procesos no son estacionarios.

# Flujo de masa (corriente de flujo)
$$
\frac{ dm }{ dt } =\dot{m} [\pu{ kg/s}]
$$
En una cañeríacon un líquido de densidad $\rho$, esta variable de relaciona con la velocidad $v$ y el área de una sección transversal $a$. Así como el volumen específico $\bar{V}$.
$$
\dot{m}=\rho·v·a=\frac{v·a}{\bar{V}}
$$
## Relación con energía 
Si una corriente con flujo másico intercambia una unidad de calor co trabajo $Q$ o $W$ por kilogramo de masa, se cumple que:
$$
\dot{Q}=\dot{m}Q
$$
$$
\dot{W}=\dot{m}W
$$
De otra forma:
$$
\dot{Q}dt=Qdm
$$
$$
\dot{W}dt=Wdm
$$
Equipos que generan cambio de presión:
 - Turbina
 - Compresor
 - Bomba
 - Válvula
Equipos que no generan cambios de presión (despreciable):
- Transferencia de calor
	- Intercambiador de calor
	- Condensador
	- Evaporador
	- Caldera o generador de vapor
- Separación o mezcla de corrientes:
	- Separador flash
	- Mezclador
	- Divisor
## Balance general
Se puede hacer una balance de masa de todo un sistema de la forma:
$$
\Delta \dot{m}=\sum_{}^{}m_{\text{in}}-\sum_{}^{}m_{\text{out}}
$$
# Balance de energía
Se debe cumplir que:
$$
\delta E=\left( \frac{v^{2}}{2}+gz+U+PV \right)\delta m
$$

$${\frac{d}{d t}}{\big(}U+E_{K}+E_{p}{\big)}=\sum_{k=1}^{K}{\dot{m}}_{k}\left(u+{\frac{v^{2}}{2}}+g z\right)_{k}+{\dot{Q}}+{\dot{W}}+{\dot{W}}_{s}+\sum_{k=1}^{K}{\dot{m}}_{k}(P V)_{k}$$
Quitando energía potencial y cinética, y factorizando:
$${\frac{d U}{d t}}=\sum_{k=1}^{K}{\dot{m}}_{k}h_{k}+{\dot{Q}}+{\dot{W}}+{\dot{W}}_{s}$$
