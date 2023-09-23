<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->


Actividad: Repositorio local de ejercicios de estructuras de control iterativas. (Trabajo individual)
Crea un repositorio local y resuelve los siguientes ejercicios para practicar bucles while y for:

Ejercicios con bucle while:

Solicita al usuario que ingrese una lista de números y encuentra el número mayor y el menor.
Solicita al usuario un número e imprime la suma de los números pares entre 1 y ese número.
Solicita al usuario una cadena e imprime cuántas vocales contiene.
Solicita al usuario un número y muestra su tabla de potencias desde 1 hasta 10.
Solicita al usuario una lista de números y calcula la media aritmética.
Ejercicios con bucle for:

Solicita al usuario una lista de números y calcula la suma de sus elementos.
Solicita al usuario una lista de números e imprime cuántos de ellos son pares.
Solicita al usuario un número y muestra su tabla de multiplicar usando range().
Solicita al usuario un número e imprime los números pares desde 2 hasta ese número.
Solicita al usuario un número y muestra la secuencia de números pares desde 2 hasta ese número.
Acciones en el repositorio local:

Captura de pantalla de la configuración inicial del repositorio.
Hacer commit por cada ejercicio.
Captura de pantalla del comando git log.
Captura de pantalla del comando git diff.
Nota: Incluir las captura de pantalla en el repositorio local.








https://colab.research.google.com/drive/1RRKbSqwGum_hHmWe848vzQDrknKL5-ty?usp=sharing#scrollTo=kRzrAIElTr59


```python 

lista



numeros = [1, 2, 3, 4, 5, 5, 6, 7, 8, 9, 10]
print(numeros)
numeros.sort()
print(numeros)
numeros.sort(reverse=True)
print(numeros)
numero_menor = min(numeros)
print("El número más pequeño en la lista es:", numero_menor)
numero_mayor = max(numeros)
print("El número más grande en la lista es:", numero_mayor)
numero_a_contar = 5
cantidad = numeros.count(numero_a_contar)
print(f"El número {numero_a_contar} aparece {cantidad} veces en la lista.")
numero_a_eliminar = 5
while numero_a_eliminar in numeros:
    numeros.remove(numero_a_eliminar)
print("Lista después de eliminar el número", numero_a_eliminar, ":", numeros)
numero_a_agregar = 11
numeros.extend([numero_a_agregar])
numero_a_agregar = 11
print("Lista después de agregar el número", numero_a_agregar, ":", numeros)
numeros.sort()
print("Lista actualizada en orden:", numeros)
```


```python 

conjuntos

conjunto_numeros = set(range(1, 11))
print(conjunto_numeros)
numero_a_agregar = 11
conjunto_numeros.add(numero_a_agregar)
print(conjunto_numeros)
numero_a_eliminar = 5
conjunto_numeros.remove(numero_a_eliminar)
print(conjunto_numeros)
cantidad_elementos = len(conjunto_numeros)
print("El conjunto tiene", cantidad_elementos, "elementos.")
numero_a_buscar = 5
if numero_a_buscar in conjunto_numeros:
    print(f"El número {numero_a_buscar} está en el conjunto.")
else:
    print(f"El número {numero_a_buscar} no está en el conjunto.")
numero_a_buscar = 11
if numero_a_buscar in conjunto_numeros:
    print(f"El número {numero_a_buscar} está en el conjunto.")
else:
    print(f"El número {numero_a_buscar} no está en el conjunto.")
conjunto_palabras = {"Hola", "mundo", "Python"}
print(conjunto_palabras)
palabra_a_buscar = "Hola"
if palabra_a_buscar in conjunto_palabras:
    print(f"La palabra '{palabra_a_buscar}' está en el conjunto.")
else:
    print(f"La palabra '{palabra_a_buscar}' no está en el conjunto.")

palabra_a_buscar = "mundo"
if palabra_a_buscar in conjunto_palabras:
    print(f"La palabra '{palabra_a_buscar}' está en el conjunto.")
else:
    print(f"La palabra '{palabra_a_buscar}' no está en el conjunto.")

```

```python
diccionario


dias_semana = {
    "Lunes": 1,
    "Martes": 2,
    "Miércoles": 3,
    "Jueves": 4,
    "Viernes": 5,
    "Sábado": 6,
    "Domingo": 7
}

print(dias_semana)
numero_lunes = dias_semana["Lunes"]
print(f"El número correspondiente al día 'Lunes' es: {numero_lunes}")
numero_a_buscar = 2
for dia, numero in dias_semana.items():
    if numero == numero_a_buscar:
        dia_correspondiente = dia
        break
else:
    dia_correspondiente = "No encontrado"
print(f"El día de la semana correspondiente al número {numero_a_buscar} es: {dia_correspondiente}")
if "Lunes" in dias_semana:
    dias_semana.pop("Lunes")
print(dias_semana)
dias_semana = {
    "Lunes": 1,
    "Martes": 2,
    "Miércoles": 3,
    "Jueves": 4,
    "Viernes": 5,
    "Sábado": 6,
    "Domingo": 7
}
print(dias_semana)

```





