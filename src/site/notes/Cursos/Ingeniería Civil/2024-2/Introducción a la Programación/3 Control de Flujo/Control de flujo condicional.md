---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/introduccion-a-la-programacion/3-control-de-flujo/control-de-flujo-condicional/","tags":["I1IIC1103"]}
---

# Ejemplo
## Calendario
```Python
evaluaciones = [
				["0310","Interrogación 1"],
				["1311","Interrogación 2"], 
				["0512","Examen"]
				]
dia = "2222"
hay = 0
for x in evaluaciones:
	if dia == x[0]:
		print("Tienes",x[1])
		hay = hay + 1
		break
if hay != 1:
	print("No tienes evaluaciones")
```