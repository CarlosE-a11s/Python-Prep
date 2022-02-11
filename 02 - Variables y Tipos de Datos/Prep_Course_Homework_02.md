## Variables

1. Crear una variable que contenga un elemento del conjunto de números enteros y luego imprimir por pantalla

mi_entero = 17
print('mi_entero')

2. Imprimir el tipo de dato de la constante 8.5

type(8.5)

3. Imprimir el tipo de dato de la variable creada en el punto 1

type('mi_entero')

4. Crear una variable que contenga tu nombre

name = 'Carlos Eduardo'

5. Crear una variable que contenga un número complejo

complex_number = 3 - 2j

6. Mostrar el tipo de dato de la variable creada en el punto 5

type(complex_number)

7. Crear una variable que contenga el valor del número Pi redondeado a 4 decimales

from math import pi
pi_redondeado = round(pi,4)

print(pi_redondeado)

8. Crear una variable que contenga el valor 'True' y otra que contenga el valor True. ¿Se trata de lo mismo?

a= 'True'
b= True

a == b # No se trata de lo mismo, pues a es string y b es boolean

9. Imprimir el tipo de dato correspondientes a las variables creadas en el punto 9

type(a)
type(b)

10. Asignar a una variable, la suma de un número entero y otro decimal

d = 132 + 25.4

11. Realizar una operación de suma de números complejos

d1 = 132 +25,4j
e = -25 +30j

f = d1 + e

12. Realizar una operación de suma de un número real y otro complejo

h = mi_entero + e

13. Realizar una operación de multiplicación

j = 345
k = -13

print(j \* k)

14. Mostrar el resultado de elevar 2 a la octava potencia

print(2\*\*8)

15. Obtener el cociente de la división de 27 entre 4 en una variable y luego mostrarla

coc = 27/4
print(coc)

16. De la división anterior solamente mostrar la parte entera

coc_entero = 27//4
print(coc_entero)

17. De la división de 27 entre 4 mostrar solamente el resto

coc_resto = 27%4
print(27%4)

18. Utilizando como operandos el número 4 y los resultados obtenidos en los puntos 16 y 17. Obtener 27 como resultado

numerador27 = coc_entero\*4 + coc_resto

19. Utilizar el operador "+" en una operación donde intervengan solo variables alfanuméricas

21 = 'Mi '
a22 = 'texto '
a23 = 'concatenado '

print(a21 + a22 + a23)

20. Evaluar si "2" es igual a 2. ¿Por qué ocurre eso?

Print("2" == 2) # False; porque son dartos de diferente tipo

21. Utilizar las funciones de cambio de tipo de dato, para que la validación del punto 20 resulte verdadera

print(int('2')==2)
print('2' == str(2))

22. ¿Por qué arroja error el siguiente cambio de tipo de datos? a = float('3,8')

porque un float se escribe con . (punto)

23. Crear una variable con el valor 3, y utilizar el operador '-=' para modificar su contenido

x = 5
x -= 2

print(x) // 3

24. Realizar la operacion 1 << 2 ¿Por qué da ese resultado? ¿Qué es el sistema de numeración binario?

print(1<<2) // 4, porque esta desplazando cifras a laderecha en lenguajge de maquina (0,1).
El sistema de numeracion binaria es el que muestra las cantidades de cualquier cosa mediante ceros y unos (0,1)

25. Realizar la operación 2 + '2' ¿Por qué no está permitido? ¿Si los dos operandos serían del mismo tipo, siempre arrojaría el mismo resultado?

2 + '2' no se permite porque son datos de diferente tipo

al ser del mismo tipo , logocamente dan diferente resultado, asi:
print('2' + '2') // 22
print(2 + 2) // 4

26. Realizar una operación válida entre valores de tipo entero y string

a = 'Bienvenido !!'
b = 3

print(a\*b) // Bienvenido !!Bienvenido !!Bienvenido !!
