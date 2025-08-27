---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/introduccion-a-la-programacion/2-variables-expresiones/tipos-de-datos-en-python/","tags":["I1IIC1103"]}
---

# Datos numéricos
## Int (int)

Números enteros (integers)

## Float (float)

Puntos flotantes, todos los números racionales con los límites de computación

## Strings (str)

Comillas letras "hola :)"

## Booleano (bool)

True or False

Con T y F mayúscula

# Tipos de datos en Python

Python reconoce los tipos de datos de forma automática, pero se pueden forzar con funciones tales como `int(3)`

```Python
import micropip
await micropip.install('numpy')  
import numpy as np
a = int(3)
b = float(3.4)
c = str("tito")
d = bool(False)
print(a)
print(b)
print(c)
print(d)
```

Además estas funciones pueden convertir tipos de datos

```Python
print("float(1) = "+str(float(1)))
print("int(3.4) = "+str(int(3.4)))
print("int(True) = "+str(int(True)))
print("int(False) = "+str(int(False)))
```
