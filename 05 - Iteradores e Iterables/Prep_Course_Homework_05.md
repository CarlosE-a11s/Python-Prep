## Iteradores e iterables

1) A partir de una lista vacía, utilizar un ciclo while para cargar allí números negativos del -15 al -1
lista_negativos = []
inic = -15
while (inic <= -1):
   lista_negativos.append(inic)
   inic += 1
print(lista_negativos)

2) ¿Con un ciclo while sería posible recorrer la lista para imprimir sólo los números pares?
ind = 0
while (ind < len(lista_negativos)):
   if (lista_negativos[ind] % 2 == 0 ):
      print(lista_negativos[ind])
   ind += 1

3) Resolver el punto anterior sin utilizar un ciclo while
for i in lista_negativos:
   if (lista_negativos[i] % 2 == 0 ):
      print(lista_negativos[i])

4) Utilizar el iterable para recorrer sólo los primeros 3 elementos
for num in lista_negativos[:3]:
   print(num)

5) Utilizar la función **enumerate** para obtener dentro del iterable, tambien el índice al que corresponde el elemento
for i, num in enumerate(lista_negativos[:3]):
   print(i, num)

6) Dada la siguiente lista de números enteros entre 1 y 20, crear un ciclo donde se completen los valores faltantes: 
lista = [1,2,5,7,8,10,13,14,15,17,20]
for num in range(1,21):
   if (not num in lista):
      lista.insert((num-1), num)
print(lista)

7) La sucesión de Fibonacci es un listado de números que sigue la fórmula: <br>
n<sub>0</sub> = 0<br>
n<sub>1</sub> = 1<br>
n<sub>i</sub> = n<sub>i-1</sub> + n<sub>i-2</sub><br>
Crear una lista con los primeros treinta números de la sucesión.<br>
fibo = [0, 1]
for i in range(1, 29):
   fibo.append(fibo[i]+ fibo[i-1])
print(fibo) 

8) Realizar la suma de todos elementos de la lista del punto anterior
print(sum(fibo))

9) La proporción aurea se expresa con una proporción matemática que nace el número irracional Phi= 1,618… que los griegos llamaron número áureo. El cuál se puede aproximar con la sucesión de Fibonacci. Con la lista del ejercicio anterior, imprimir el cociente de los últimos 5 pares de dos números contiguos:<br>
Donde i es la cantidad total de elementos<br>
n<sub>i-1</sub> / n<sub>i</sub><br>
n<sub>i-2</sub> / n<sub>i-1</sub><br>
n<sub>i-3</sub> / n<sub>i-2</sub><br>
n<sub>i-4</sub> / n<sub>i-3</sub><br>
n<sub>i-5</sub> / n<sub>i-4</sub><br>
aurea = []
for j in range(24,29):
   aurea.append(fibo[j-1]/fibo[j])
print(aurea) 

10) A partir de la variable cadena ya dada, mostrar en qué posiciones aparece la letra "n"<br>
cadena = 'Hola Mundo. Esto es una practica del lenguaje de programación Python'
for i, e in enumerate(cadena):
   if (e == 'n'):
      print(i)

11) Crear un diccionario e imprimir sus claves utilizando un iterador
reino_animal = {'Acuatico' : ['delfin', 'cachalote', 'tiburon'], 'Terrestre' : ['caballo', 'elefante', 'llama'], 'Aereo' : ['aguila', 'paloma', 'gaviota']}
for clase in reino_animal:
   print(clase)

12) Convertir en una lista la variable "cadena" del punto 10 y luego recorrerla con un iterador
lista1 = list(cadena)
print(lista1)
caracter = iter(lista1)
for i in range(1, len(lista1)+1):
   print(next(caracter))

13) Crear dos listas y unirlas en una tupla utilizando la función zip
sigla = ['H', 'E', 'N', 'R', 'Y']
significado = ['High', 'Earn', 'Not', 'Rich', 'Yet']
academia = zip(sigla, significado)
print(list(academia))

14) A partir de la siguiente lista de números, crear una nueva sólo si el número es divisible por 7<br>
lis = [18,21,29,32,35,42,56,60,63,71,84,90,91,100]
lis_div7 = []
for i in lis:
   if ((i%7) == 0):
      lis_div7.append(i)
print(lis_div7)

15) A partir de la lista de a continuación, contar la cantidad total de elementos que contiene, teniendo en cuenta que un elemento de la lista podría ser otra lista:<br>
lis = [[1,2,3,4],'rojo','verde',[True,False,False],['uno','dos','tres']]
register = 0
for lista in lis:
   register = register + len(lista)
print(register)

16) Tomar la lista del punto anterior y convertir cada elemento en una lista si no lo es
lis = [[1,2,3,4],'rojo','verde',[True,False,False],['uno','dos','tres']]
lis_convertida = []
for es_lista in lis:
   if (not type(es_lista) == list):
      a = list(es_lista)
      lis_convertida.append(a)
   else:
      lis_convertida.append(es_lista)
print(lis_convertida)
