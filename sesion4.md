<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

Actividad: Resolver utilizando funciones en Python
Calculadora Básica: Crea una función llamada calculadora que tome tres argumentos: dos números y un operador (+, -, *, /). La función debe realizar la operación indicada en los dos números y devolver el resultado.
Ejemplo de uso:

resultado = calculadora(5, 3, '+')  # Debe devolver 8

Conteo de Vocales: Crea una función llamada contar_vocales que tome una cadena como argumento y devuelva el número de vocales (a, e, i, o, u) que contiene la cadena.
Ejemplo de uso:

num_vocales = contar_vocales("Hola, mundo!")  # Debe devolver 4

Primo o No Primo: Escribe una función llamada es_primo que tome un número entero positivo como argumento y determine si es un número primo (es decir, solo es divisible por 1 y por sí mismo). La función debe devolver True si es primo y False si no lo es.
Ejemplo de uso:

resultado = es_primo(17)  # Debe devolver True

Contador de Palabras: Escribe una función llamada contar_palabras que tome una cadena como argumento y devuelva el número de palabras en esa cadena. Supón que las palabras están separadas por espacios.
Ejemplo de uso:

num_palabras = contar_palabras("Hola, este es un ejemplo.")  # Debe devolver 5

Cálculo de Potencia: Escribe una función llamada potencia que tome dos números enteros como argumentos, uno como base y otro como exponente, y devuelva el resultado de elevar la base al exponente.
Ejemplo de uso:

resultado = potencia(2, 3)  # Debe devolver 8 (2^3 = 2 * 2 * 2)



https://colab.research.google.com/drive/19RFwJv5iYuIQfJtqdgWtGD0Lltpu2OT2?usp=sharing



calculadora
```python
def calculadora(num1, num2, operador):
    if operador == '+':
        resultado = num1 + num2
    elif operador == '-':
        resultado = num1 - num2
    elif operador == '*':
        resultado = num1 * num2
    elif operador == '/':
        if num2 != 0:
            resultado = num1 / num2
        else:
            return "Error: No se puede dividir entre cero"
    else:
        return "Operador no válido"
    return resultado


resultado = calculadora(5, 3, '-')
print(resultado)
```


contador de vocales
```python
def contar_vocales(cadena):

    contador = 0


    for letra in cadena:

        if letra.lower() in 'aeiou':
            contador += 1

    return contador

# Ejemplo de uso:
cadena = "joce"
resultado = contar_vocales(cadena)
print(resultado)
```



numero primo o no

```python
def es_primo(numero):

    if numero <= 1:
        return False

    for divisor in range(2, int(numero ** 0.5) + 1):
        if numero % divisor == 0:
            return False

    return True


numero = 18
resultado = es_primo(numero)
print(resultado)

```


contador de palabras:

```python

def contar_letras(cadena):

    cadena_sin_espacios = cadena.replace(" ", "")

    cantidad_letras = len(cadena_sin_espacios)
    return cantidad_letras


cadena = "prueba cuatro"
resultado = contar_letras(cadena)
print(resultado)
```


calculo de potencia

```python
def potencia(base, exponente):
    resultado = base ** exponente
    return resultado

# Ejemplo de uso:
base = 2
exponente = 3
resultado = potencia(base, exponente)
print(resultado)
```