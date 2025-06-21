---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/unidad-1/5-calorimetria/calorimetria-capacidad-calorifica-y-calor-latente/","tags":["I1IIQ1003"]}
---


# Calorimetría

Estudio de la cantidad de calor que se intercambia en una reacción.

El calorímero.

![Pasted image 20240411121804.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/Qu%C3%ADmica%20para%20Ingenier%C3%ADa/4%20Termoqu%C3%ADmica.%20Energ%C3%ADa%20y%20Quim%C3%ADca/attachments/Pasted%20image%2020240411121804.png)

# Capacidad calorífica ($C$)

La cantidad de energía en forma de $q$, necesaria para modificar $T$ depende de :

- Cuando deba cambiar $T$
- Cantidad de sustancia
- La naturaleza de la sustancia
Ejemplo: Definición de caloría.
Así, se define la capacidad calórica como la cantidad de energía necesaria para aumentar un grado K o C, a un gramo (específica) o 1 mol (molar) de sustancia.
La capacidad calórica se mide en $\frac{cal}{gºC}$.

Así, se puede definir a la capacidad calorífica como el cambio de calor con respecto a la temperatura, dejando $P$ y $V$ constante:
$$
C=\frac{ dQ }{ dT } 
$$
## Volumen constante
Si se considera presión o volumen, se deben considerar [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.7 Derivadas parciales. Interpretación de concepto de derivadas parciales/Derivadas parciales\|Derivadas parciales]].
Con volumen constante, no hay trabajo, así que $Q \propto U$:
$$
\Delta U=Q+\cancel{ W }
$$
$$
C_{V}=\left( \frac{ \partial U }{ \partial T }  \right)_{V}
$$
De aquí, y como la energía interna es una función de estado:
$$
dU=C_{V}dT
$$
$$
U_{A-B}=\int_{T_{A}}^{T_{B}} C_{V} \, dT
$$

## Presión constante
Con **presión** constante, $Q= H$:
$$
C_{P}=\left( \frac{ \partial H }{ \partial T }  \right)_{P}
$$
Como $H$ es función de estado:
$$\Delta H_{A-B}=\int_{T_{A}}^{T_{B}}C_{P}\,d T$$


Para simplificar los cálculos, se pueden tomar cantidades promedio:
$$\bar{C}_{P}=\frac{\int_{T_{1}}^{T_{2}}C_{P}d T}{T_{2}\;-\;T_{1}}$$
De aquí:
$$\Delta H_{A-B}=\bar{C}_{P}\left(T_{B}-\,T_{A}\right)$$
### Como cambia con presión constante
La capacidad calorífica tiene a subir mientras se mantenga como gas, al pasar a ser líquido, la capacidad calorífica deja de subir ya que son incompresibles.
![Pasted image 20250324085610.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/Qu%C3%ADmica%20para%20Ingenier%C3%ADa/4%20Termoqu%C3%ADmica.%20Energ%C3%ADa%20y%20Quim%C3%ADca/attachments/Pasted%20image%2020250324085610.png)
La línea punteada es equilibrio líquido-vapor
### Capacidad calorífica de un gas ideal
Udualmente en tablas de compuestos puros, se muestran datos en forma de correlación para $C^{ig}_{P}$, entregando parámetros para una función polinomial de la temperatura y normalizados con $R$.
$$
C^{ig}_{P}=a_{0}+a_{1}T+a_{2}T^{2}+a_{3}T^{3}+a_{4}T^{4}
$$
## Interpretación
Los valores de $C_{V}$ y $C_{P}$ son distintos ya que si no se mantiene el volumen constante, se va a perder energía (trabajo) en la expansión.
![Pasted image 20250324085414.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/Qu%C3%ADmica%20para%20Ingenier%C3%ADa/4%20Termoqu%C3%ADmica.%20Energ%C3%ADa%20y%20Quim%C3%ADca/attachments/Pasted%20image%2020250324085414.png)

# Calor específico

Así se logra definir al calor específico ($q$) como:

$$
q=C·\Delta T·m
$$
# Calor sensible y latente
**Calor sensible:** Se cuantifican con capacidad calorífica, se agrega energía cinética a la moléculas, solo cambiando rotación y traslación.
**Calor latente:** Representa un cambio notable donde se rompen enlaces. Se usa la entalpía de vaporización $\Delta H^{vap}$. 
## Calor latente (de vaporización)
$$\Delta H^{v a p}=H^{V}-H^{L}=(U^{V}-U^{L})+P^{s a t}(V^{V}-V^{L})$$
![Pasted image 20250324090430.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/Qu%C3%ADmica%20para%20Ingenier%C3%ADa/4%20Termoqu%C3%ADmica.%20Energ%C3%ADa%20y%20Quim%C3%ADca/attachments/Pasted%20image%2020250324090430.png)
Finalmente, para llegar de temperatura $T_{A}$ a $T_{B}$, se debe dividir en 3 partes:
$$\Delta H_{A B}=\int_{T_{A}}^{T_{s a t}}C_{p}^{l i q}d T+\Delta H_{v a p}+\int_{T{s a t}}^{T_{B}}C_{P}^{v a p}d T$$
# Ejemplo
Calcule el calor necesario para llevar 2 kg de acetona desde 40°C ($313K$) hasta 100°C ($373K$) a presión constante
1. Verificar punto de fusión o ebullición de la acetona
![Pasted image 20250324091338.png|1000](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/Qu%C3%ADmica%20para%20Ingenier%C3%ADa/4%20Termoqu%C3%ADmica.%20Energ%C3%ADa%20y%20Quim%C3%ADca/attachments/Pasted%20image%2020250324091338.png)
Como $313K<T_{eb}<373K$, se debe hacer el cálculo en tres partes.
$$
H_{1}=\int_{313K}^{329.3K} C_{P,l} \, dT 
$$
$$
H_{2}=\int_{329K}^{373K} C_{P,v} \, dT 
$$
