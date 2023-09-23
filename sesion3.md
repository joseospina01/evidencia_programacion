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








https://colab.research.google.com/drive/1DNIIHQMLNffTR733gLWHm-g2N2O1_j1j#scrollTo=DYsU7lsjuqo2


```python 
Lista

lista = [ 1,2,3,4,5,8,7,6,9,10,]

print(lista)

lista.sort()
print(lista)
lista.reverse()
print(lista)
np= min(lista)
print(np)
ng=max(lista)
print(ng)
nc=5
cantidad=lista.count(nc)
print(cantidad)
lista.remove(5)
print(lista)
lista.insert(4, 11)
lista.sort()
print(lista)
```


```python
Tupla

mi_tupla = ("Hola", "mundo", "Python")
print("Tupla original:", mi_tupla)


mi_tupla_ordenada = sorted(mi_tupla)
print("Tupla ordenada:", mi_tupla_ordenada)


primera_palabra = mi_tupla[0]
print("Primera palabra:", primera_palabra)


ultima_palabra = mi_tupla[-1]
print("Última palabra:", ultima_palabra)


numero_de_palabras = len(mi_tupla)
print("Número de palabras:", numero_de_palabras)


mi_tupla_sin_mundo = tuple(word for word in mi_tupla if word != "mundo")
print("Tupla sin 'mundo':", mi_tupla_sin_mundo)

mi_tupla_con_hola = mi_tupla + ("Hola",)
print("Tupla con 'Hola':", mi_tupla_con_hola)

```



```python 
Conjunto

numeros_conjunto = set(range(1, 11))


print("Conjunto de números:", numeros_conjunto)


numeros_conjunto.add(11)


numeros_conjunto.discard(5)

numero_de_elementos = len(numeros_conjunto)
print("Número de elementos:", numero_de_elementos)

esta_cinco = 5 in numeros_conjunto
print("¿El número 5 está en el conjunto?", esta_cinco)


esta_once = 11 in numeros_conjunto
print("¿El número 11 está en el conjunto?", esta_once)

palabras_conjunto = {"Hola", "mundo", "Python"}


print("Conjunto de palabras:", palabras_conjunto)


esta_hola = "Hola" in palabras_conjunto
print("¿La palabra 'Hola' está en el conjunto?", esta_hola)

esta_mundo = "mundo" in palabras_conjunto
print("¿La palabra 'mundo' está en el conjunto?", esta_mundo)

```

```python
diccionario


dias_semana_dict = {
    "Lunes": 1,
    "Martes": 2,
    "Miércoles": 3,
    "Jueves": 4,
    "Viernes": 5,
    "Sábado": 6,
    "Domingo": 7
}
print("Diccionario de días de la semana:", dias_semana_dict)


numero_lunes = dias_semana_dict["Lunes"]
print("Número del día 'Lunes':", numero_lunes)


dia_numero_2 = next((dia for dia, numero in dias_semana_dict.items() if numero == 2), None)
print("Día correspondiente al número 2:", dia_numero_2)


del dias_semana_dict["Lunes"]


print("Diccionario después de eliminar 'Lunes':", dias_semana_dict)

```





