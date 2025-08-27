---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/introduccion-a-la-programacion/9-programacion-orientada-a-objetos/clases-y-objetos-en-python/","tags":["I1IIC1103"]}
---

La clase es como un "molde" para crear objetos de un tipo específico. Esto sirve para poder escalar un código de forma correcta y simple

# Métodos
Van con def dentro de una clase, pueden:
- Actualizar atributos
- No actualizarlos
# Ejemplo
Se quiere definir, para cada estudiante un identificador (int), un nombre (str) y sus notas (list).
Para hacer esto se crea la **clase** Estudiante, cada estudiante será un objetos, y cada objeto tendrá atributos (int, str, list)
Se quiere crear la clase, y también crear un método para añadir (agregar) una nota

```Python
class Estudiante:
	def __init__(self, ID, Nombre, notas):
		self.ID = ID
		self.Nombre = Nombre
		self.notas = notas
		self.promedio = sum(notas)/len(notas) #se pueden manejar las entradas para crear atributos
	def agregar_nota(self, nota):
		print("Nota agregada a estudiante",self.Nombre,":",nota)
		self.notas.append(nota)
		self.promedio = sum(self.notas)/len(self.notas) #actualizar el promedio
	
"""
este es el método constructor, es lo que le va a dar la estructura al grupo de elementos.

self puede ser cualquier palabra

Ahora, la sintaxis para crear un objeto Estudiante será la siguiente
"""
est_1 = Estudiante(1,"joseto",[4,4,4,4])
est_2 = Estudiante(2,"benja",[2,2.4,7,4])
Estudiantes = [est_1,est_2]
for e in Estudiantes:
	print(e)
	print(e.ID)
	print(e.Nombre)
	print(e.notas)
	print(e.promedio)

est_1.agregar_nota(1)
print("nuevo promedio:")
print(est_1.promedio)

```
