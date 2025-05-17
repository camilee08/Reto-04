# Reto-04
Solución al reto 04
--
### Busco resolver los siguientes problemas usando un notebook de python y Vison Studio Code
---
1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.  
 Usando Estructura If
```
n = int(input("Ingrese un numero entero: "))
if n in [97, 101, 105, 111, 117]:  # códigos ASCII de 'a', 'e', 'i', 'o', 'u'
  print(f"El numero {n} corresponde a una vocal minúscula.")
else:
  print(f"El numero {n} NO corresponde a una vocal minúscula.")
```
---
2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.  
Usando estructura if-else
```
c = input("Ingrese una cadena de longitud 1: ")
if len(c) != 1:
  print("Debe ingresar solo un carácter.")
else:
  codigo = ord(c[0])
  if codigo % 2 == 0:
    print(f"El código ASCII de '{c}' es {codigo} y es PAR.")
  else:
    print(f"El código ASCII de '{c}' es {codigo} y es IMPAR.")
```
---
3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.  
Usando Estructura if-else
```
c = input("Ingrese un carácter: ")
if len(c) == 1 and c.isdigit():
  print(f"El carácter '{c}' es un dígito.")
else:
  print(f"El carácter '{c}' NO es un dígito.")
```
---
4. Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.  
Usando Estructura if-elif-else
```
a = float(input("Ingrese el primer número: "))
b = float(input("Ingrese el segundo número: "))
if b == 0:
  print("No se puede dividir por cero.")
elif a % b == 0:
  print(f"{a} es múltiplo de {b}")
else:
  print(f"{a} NO es múltiplo de {b}")
```
---
5. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:
* Positivo: "El número x es positivo"
* Negativo: "El número x es negativo"
* Cero (0): "El número x es el neutro para la suma"  
Usando Estructura if-elif-else
```
x = float(input("Ingrese un número real: "))
if x > 0:
  print(f"El número {x} es positivo")
elif x < 0:
  print(f"El número {x} es negativo")
else:
  print(f"El número {x} es el neutro para la suma")
```
---
6. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.  
Usando Estructura if-elif-else
```
import math

x_c = float(input("Ingrese la coordenada x del centro: "))
y_c = float(input("Ingrese la coordenada y del centro: "))
r = float(input("Ingrese el radio del círculo: "))

x = float(input("Ingrese la coordenada x del punto: "))
y = float(input("Ingrese la coordenada y del punto: "))

distancia = math.sqrt((x - x_c)**2 + (y - y_c)**2)
if distancia < r:
  print("El punto está dentro del círculo.")
elif distancia == r:
  print("El punto está sobre el borde del círculo.")
else:
  print("El punto está fuera del círculo.")
```
---
7. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
Usando if-else
```
a = float(input("Ingrese la primera longitud: "))
b = float(input("Ingrese la segunda longitud: "))
c = float(input("Ingrese la tercera longitud: "))

if a + b > c and a + c > b and b + c > a:
  print("Sí se puede construir un triángulo con esas longitudes.")
else:
  print("NO se puede construir un triángulo con esas longitudes.")
```
---
8. Escriba un programa que reciba el nombre en minúsculas de un país de America y retorne la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado (Utilice match-case).
Usando match-case
```
pais = input("Ingrese el nombre del país (en minúsculas): ")

match pais:
  case "colombia":
    print("Bogotá")
  case "argentina":
    print("Buenos Aires")
  case "mexico":
    print("Ciudad de México")
  case "brasil":
    print("Brasilia")
  case "canada":
    print("Ottawa")
  case "chile":
    print("Santiago")
  case "peru":
    print("Lima")
  case "ecuador":
    print("Quito")
  case "venezuela":
    print("Caracas")
  case "uruguay":
    print("Montevideo")
  case "bolivia":
    print("La Paz / Sucre")
  case "paraguay":
    print("Asunción")
  case "panama":
    print("Ciudad de Panamá")
  case "cuba":
    print("La Habana")
  case _:
    print("País no identificado")
```
---
Eso es todo, gracias por revisar el repo.
