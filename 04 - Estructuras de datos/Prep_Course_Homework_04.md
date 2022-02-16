## Estructuras de Datos

1) Crear una lista que contenga nombres de ciudades del mundo que contenga más de 5 elementos e imprimir por pantalla
world_cities = ['Bogotá', 'Londres', 'Ciudad de México', 'Singapur', 'Oslo', 'Montreal', 'Ciudad del Cabo', 'El Cairo']
print(world_cities)

2) Imprimir por pantalla el segundo elemento de la lista
print(world_cities[1])

3) Imprimir por pantalla del segundo al cuarto elemento
print(world_cities[1:4])

4) Visualizar el tipo de dato de la lista
print(type(world_cities))

5) Visualizar todos los elementos de la lista a partir del tercero de manera genérica, es decir, sin explicitar la posición del último elemento
print(world_cities[3:])

6) Visualizar los primeros 4 elementos de la lista
print(world_cities[:4])

7) Agregar una ciudad más a la lista que ya exista y otra que no ¿Arroja algún tipo de error?
print(world_cities.append('Bogotá'))
print(world_cities.append('Roma'))
print(world_cities) 
# No se registra ningún tipo de error.

8) Agregar otra ciudad, pero en la cuarta posición
world_cities.insert(3, 'Madrid')
print(world_cities)

9) Concatenar otra lista a la ya creada
more_cities = ['Buenos Aires', 'Brasilia', 'Copenague']
world_cities.extend(more_cities)
print(world_cities)

10) Encontrar el índice de la ciudad que en el punto 7 agregamos duplicada. ¿Se nota alguna particularidad?
print(world_cities.index('Bogotá'))

11) ¿Qué pasa si se busca un elemento que no existe?
print(world_cities.index('New york'))
# nos registra Error, así:
Traceback (most recent call last):
  File "c:\Users\Carlos\prueba_Henry_course.py", line 10, in <module>
    print(world_cities.index('New york'))
ValueError: 'New york' is not in list

12) Eliminar un elemento de la lista
world_cities.remove('Singapur')

13) ¿Qué pasa si el elemento a eliminar no existe?
world_cities.remove('Lisboa')
# Nos registra el siguiente error:
Traceback (most recent call last):
  File "c:\Users\Carlos\prueba_Henry_course.py", line 11, in <module>
    world_cities.remove('Lisboa')
ValueError: list.remove(x): x not in list

14) Extraer el úlimo elemento de la lista, guardarlo en una variable e imprimirlo
last_city = world_cities.pop()
print(last_city)

15) Mostrar la lista multiplicada por 4
print(world_cities * 4)

16) Crear una tupla que contenga los números enteros del 1 al 20
tupla_numerica = (1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20)
print(tupla_numerica)

17) Imprimir desde el índice 10 al 15 de la tupla
print(tupla_numerica[10:15])

18) Evaluar si los números 20 y 30 están dentro de la tupla
print(20 in tupla_numerica) # True
print(30 in tupla_numerica) # False

19) Con la lista creada en el punto 1, validar la existencia del elemento 'París' y si no existe, agregarlo. Utilizar una variable e informar lo sucedido.
ciudad_existe = 'Paris'
if ciudad_existe in world_cities:
   print('la Ciudad ', ciudad_existe, ' ya está en la Lista')
else:
   world_cities.append('Paris')
   print('la Ciudad ', ciudad_existe,' se agrego a la Lista')
   print(world_cities)

20) Mostrar la cantidad de veces que se encuentra un elemento específico dentro de la tupla y de la lista
print(tupla_numerica.count(10))
print(world_cities.count('Bogotá'))

21) Convertir la tupla en una lista
lista_1 = list(tupla_numerica)
print(lista_1)

22) Desempaquetar solo los primeros 3 elementos de la tupla en 3 variables
elem_1, elem_2, elem_3, _, _, _, _, _, _, _, _, _, _, _, _, _, _, _, _, _ = tupla_numerica
print(elem_1) 
print(elem_2)
print(elem_3)

23) Crear un diccionario utilizando la lista crada en el punto 1, asignandole la clave "ciudad". Agregar tambien otras claves, como puede ser "Pais" y "Continente".


24) Imprimir las claves del diccionario

25) Imprimir las ciudades a través de su clave
