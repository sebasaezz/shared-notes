---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/unidad-1/3-energia-calor-y-trabajo/calor-trabajo-y-energia-en-termodinamica/","tags":["I1IIQ1003"]}
---

El calor, [[Cursos/Ingeniería Civil/2024-1/Química para Ingeniería/4 Termoquímica. Energía y Quimíca/El trabajo (w) en termodinámica (gases)\|trabajo]] y energía tienen las mismas unidades, pero representan cosas distintas.
La energía ($U$) es una [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/1 Fundamentos de la termodinámica/Sistemas termodinámicos, estado de un sistema y función de estado\|función de estado]], pero el calor ($q$) y el trabajo ($w$) son las propiedades alteradas para cambiar una función de estado, son procesos.
# Energía
Habilidad de un sistema de hacer cambios a sí mismo o alrededores. Lo ideal en un traspaso de energía, es que sea transmitida totalmente a través de trabajo, pero esto es imposible, siempre se perderá energía en forma de calor.
$$
E=U+E_{k}+E_{p}
$$
Donde $U$ es la [[Energía interna\|Energía interna]]. Las otras cinética y potencial.
Si el sistema es **fijo**, entonces no hay cambio de potencial y cinética
# Trabajo
La definición física es la siguiente:
$$
W=F_{\text{externa}}·\Delta x
$$
Es importante que el trabajo tiene una dirección, y para ello se debe definir un marco de referencia.
Siempre que haya compresión o expansión de las paredes, va a haber cambio en el trabajo.
También existe el [[Trabajo de eje\|Trabajo de eje]], donde el trabajo se transmite por un eje en movimiento sin cambiar el tamaño del sistema.
## Convención de signos
Esto es medio ambiguo, pero se toma que:
- El trabajo se hace sobre el sistema es positivo
- El trabajo realizado por el sistema es negativo
Finalmente, el trabajo se define como:
$$
W=-\int_{V_{i}}^{V_{f}} P_{a} \, dV 
$$
# Ley cero
Con cuerpos en contacto $A$, $B$ y $C$, si $A$ y $B$ están en equilibrio, entonces $C$ y $B$ también.
![Pasted image 20250317090945.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Unidad%201/attachments/Pasted%20image%2020250317090945.png)
# Ejercicio
Estanque rígido de $1\pu{ m^{3}}$ de capacidad. tiene $1.2\pu{ kg}$ de agua a $1$ bar y $99.63ºC$ Hayq ue agregar calor para que la presión sea $3$ bar.
Como es rígido, entonces:
$$
\Delta U=\cancel{ \Delta W } + \Delta Q
$$
- $P_{1}=1\pu{ Bar }$
- $T_{1}=99.63ºC$
- $\bar{V}_{1}=\frac{1\pu{ m^{3}}}{1.2\pu{ kg}}=0.833 \frac{m^{3}}{kg}$

- $P_{2}=3\pu{ bar }$
- $T_{2}=?$
- $\bar{V}_{2}=\bar{V}_{1}$ ya que es **rígido**.

ahora se ven las tablas.
![Pasted image 20250317091820.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Unidad%201/attachments/Pasted%20image%2020250317091820.png)
Considerando el volumen ya dado y los volúmenes de la tabla:
$$
x= \frac{V_{1}-V_{L}}{V_{v}-V_{L}}=\frac{0.833-0.00104}{1.69-0.00104}=0.49=\frac{U_{1}-U_{L}}{U_{v}-U_{L}}=\frac{U_{1}-417.36}{2506.1-417.36}
$$
$$
U_{1}=0.49·(2506.1-417.36)+417.36=1440.84 \pu{ \frac{kJ}{kg} }
$$
Ahora hay que usar la calidad $x$, para calcular $U_{2}$, pero esto no se puede hacer ya que a las $3\pu{ atm}$ el agua pasa a ser un vapor sobrecalentado. Esto ya que el volumen específico de gas en menor que el volumen específico total. $(\implies x>1)$
![Pasted image 20250317102415.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Unidad%201/attachments/Pasted%20image%2020250317102415.png)
