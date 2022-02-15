## Flujos de Control

1. Crear una variable que contenga un elemento del conjunto de números enteros y luego imprimir por pantalla si es mayor o menor a cero
z = -10
if (z > 0):
   print( "El número es mayor que Cero")
elif (z < 0):
   print( "El número es menor que Cero")
else:
   print( "el número es igual a Cero")

2. Crear dos variables y un condicional que informe si son del mismo tipo de dato
j = 2 + 3j
h = "Datascience"
if (type(j) == type(h)):
   print("las variables son del mismo tipo")
else:
   print("las varibles son de diferente tipo")

3. Para los valores enteros del 1 al 20, imprimir por pantalla si es par o impar
for n in range(1,21):
   if (n%2 == 0):
      print(n, " es Par")
   else:
      print(n, " es Impar")

4. En un ciclo for mostrar para los valores entre 0 y 5 el resultado de elevarlo a la potencia igual a 3
for n in range(0,6):
   n_3 = n**3
   print(n, "elevado al cubo es igual a ",n_3)

5. Crear una variable que contenga un número entero y realizar un ciclo for la misma cantidad de ciclos
d = 4
for k in range(0,4):
   pass
print("Total Ciclos ",d)

6. Utilizar un ciclo while para realizar el factorial de un número guardado en una variable, sólo si la variable contiene un número entero mayor a 0
f = 4
if (type(f) == int):
   if (f > 0):
      a = f
      factorial = f
      while(f > 2):
         f -=  1
         factorial = factorial*f
      print("El factorial de ",a, "es ",factorial)
   else:
      print("El dato en la variable no es mayor que cero")
else:
   print("El dato no es un entero")

7. Crear un ciclo for dentro de un ciclo while
cadena = "Henry"
n= 0
while (n < 3):
   print("Ronda WHILE ", n+1)
   for letra in (cadena):
      print(letra)
   print("Fin ronda FOR")
   n += 1

8. Crear un ciclo while dentro de un ciclo for
j=3
for i in range(1,j+1):
   print("Ciclo FOR ", i)
   n=1
   while (n <= j):
      print("ciclo WHILE ", n)
      n +=1
print("Esto es ", j, " 'ciclo while' dentro de ", j, "'ciclo for'")

9. Imprimir los números primos existentes entre 0 y 30
for n in range(1,31): # el cero no se considera primo
   j = 2
   primo = True
   while (j < n):
      if (n % j == 0):
         primo = False
      j += 1
   if (primo):
      print(n, " es primo")

10. ¿Se puede mejorar el proceso del punto 9? Utilizar las sentencias break y/ó continue para tal fin
# En el ciclo 'while' no se necesita recorrer todos los numeros j menores que n para determinar si NO es primo, es suficiente encontrar un numero con resto cero para romper el ciclo con 'break' para mejorar el codigo, asI:
# Nota: con el continue se queda en un bucle sin fin.
for n in range(1,31):
   j = 2
   primo = True
   while (j < n):
      if (n % j == 0):
         primo = False
         break # con este break se mejora u optimiza el código
      j += 1
   if (primo):
      print(n, " es primo") 

11. En los puntos 9 y 10, se diseño un código que encuentra números primos y además se lo optimizó. ¿Es posible saber en qué medida se optimizó?
# Es posible y se verifica con el tiempo de ejecución, en este caso, entre el código del pumto 9 el código del punto 10.

12. Si la cantidad de números que se evalúa es mayor a treinta, esa optimización crece?
# Logicamente. Cada vez que el numero es mayor por cada numero No primo se realiza solo una division de resto Cero con el código optimizado del punto 10.

13. Aplicando continue, armar un ciclo while que solo imprima los valores divisibles por 12, dentro del rango de números de 100 a 300
min = 99
init = 100
max = 300
count = 0
while (min <= max):
   min += 1
   if (min % 12 != 0):
      continue
   print(min, " es divisible por 12.")
   count += 1
print(f'Entre {init} y {max}, hay {count} números divisibles por 12')

14. Utilizar la función **input()** que permite hacer ingresos por teclado, para encontrar números primos y dar la opción al usario de buscar el siguiente
n = 1
sigue = 1
primo = True
while (sigue == 1):
    for div in range(2, n):
        if (n % div == 0):
            primo = False
            break
    if (primo):
        print(n)
        print('¿Desea encontrar el siguiente número primo?')
        if (input() != '1'):
            print('Se finaliza el proceso')
            break
    else:
        primo = True
    n += 1
    # este item se copio del homework resuleto para comprender lo de la función input()

15. Crear un ciclo while que encuentre dentro del rango de 100 a 300 el primer número divisible por 3 y además múltiplo de 6
min = 99
max = 300
while (min <= max):
   min += 1
   if (min % 3 == 0 and min % 6 == 0 ):
      print(min, " es el primer numero divisible por 3 y multiplo de 6 \n en el rango de 100 a 300")
      break

