## Funciones

1) Crear una función que reciba un número como parámetro y devuelva si True si es primo y False si no lo es
def es_num_primo(num):
   sup = num//2 + 1
   es_primo = True
   for n in range(2, sup):
      if ( num % n == 0 ):
         es_primo = False
         break
   return es_primo
print(es_num_primo(33))

2) Utilizando la función del punto 1, realizar otra función que reciba de parámetro una lista de números y devuelva sólo aquellos que son primos en otra lista
lis = [3,7,12, 15, 21, 19, 25, 29, 37,45]   
lis_primos = []
def lista_solo_primos(x):
   for n in range(0, len(x)):
      if (es_num_primo(x[n]) == True ):
         lis_primos.append(x[n])
   return lis_primos
print(lista_solo_primos(lis))

3) Crear una función que al recibir una lista de números, devuelva el que más se repite y cuántas veces lo hace. Si hay más de un "más repetido", que devuelva cualquiera

4) A la función del punto 3, agregar un parámetro más, que permita elegir si se requiere el menor o el mayor de los mas repetidos.

5) Crear una función que convierta entre grados Celsius, Farenheit y Kelvin<br>
Fórmula 1	: (°C × 9/5) + 32 = °F<br>
Fórmula 2	: °C + 273.15 = °K<br>
Debe recibir 3 parámetros: el valor, la medida de orígen y la medida de destino


6) Iterando una lista con los tres valores posibles de temperatura que recibe la función del punto 5, hacer un print para cada combinación de los mismos:

7) Armar una función que devuelva el factorial de un número. Tener en cuenta que el usuario puede equivocarse y enviar de parámetro un número no entero o negativo
