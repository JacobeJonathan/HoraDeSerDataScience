# DataScience
![DataScience](src/1.jpg)
- [ Curso Basico de Python](#BasicoPython)
- [Curso de Fundamentos de Álgebra Lineal con Python](#CursodeFundamentosdeÁlgebraLinealconython)
- [Curso de Estadística Computacional con Python](#CursodeEstructurasdeDatosLinealesconPython)
- [Curso Profesional de Python](#CursoProfesionaldePython)
- [Git](#Git)
- [Terminal](#Terminal)
- [Anaconda](#Anaconda)
- [Excel](#Excel)
- [PostgreSQL](#PostgreSQL)
- [SQL Y MYSQL](#SQLYMYSQL)
- [ORACLE DATABASE](#ORACLEDATABASE)
- [LINUX](#LINUX)
- [Pandas](#Pandas)
- [Numpy](#Numpy)
- [DATAWAREHOUSE- ETL - CUBO OLAP - EFESTO](#Datawarehouse)
- [matplotlib](#matplotlib)
- [SeaBorn](#SeaBorn)
- [PowerBi](#PowerBi)
- [mario F triola](#marioFtriola)
- [Algebra](#Algebra)
- [Probabilidad](#Probabilidad)


## BasicoPython
- Python un lenguaje que podemos aprender para iniciarnos en la ingeniería de software. Es utilizado en Drones, Autos autónomos y hasta cohetes, nos rodea por todos lados.

- Razones por iniciarse con Python

  - El lenguaje con mayor crecimiento
  - Es el curso ideal si no tienes ningún contacto con la programación o ya dominas algún lenguaje y quieres aprender más.
  - Su forma de escribir es elegante y simple
  - La programación está en todos lados
  - Programar es darle instrucciones a la computadora para que resuelva un problema.
  - La industria de tecnología es una de las que tienen mayor crecimiento.
- Un algoritmo es una serie de pasos ordenados para resolver un problema. Este es finito, ordenado, y no ambiguo.
- Las características fundamentales que debe cumplir todo algoritmo son:

  - Un algoritmo debe ser preciso e indicar el orden de realización de cada paso.
  - Un algoritmo debe estar definido. Si se sigue un algoritmo dos veces, se debe obtener el mismo resultado cada vez.
  - Un algoritmo debe ser finito. el algoritmo se debe terminar en algún momento; o sea, debe tener un número finito de pasos.
  - Un algoritmo debe ser legible: El texto que lo describe debe ser claro, tal que permita entenderlo y leerlo fácilmente.
- ![Inicio](src/2.png)

### Operaciones Aritmeticos
- Suma: 5 + 5
- Resta: 5 - 5
- Multiplicación: 5 * 5
- División (con decimales): 5 / 5
- División (sin decimales): 21 // 5
- Resto de la división: 21 % 5
- Potencia: 2 ** 2
- Raíz cuadrada:
```py
>>> math.sqrt(9)     
>>> 3.0
>>> math.sqrt(11.11)   
>>> 3.3331666624997918
>>> math.sqrt(Decimal('6.25'))     
>>> 2.5
```
### Que es una variable
- Una variable es un lugar en memoria (una especie de caja) en el que podemos guardar objetos (números, texto, etc). Esta variable posee un identificador o nombre con el cual podemos llamarla más tarde cuando la necesitemos.
- Tipos de variables en Python:
  - a = 28 → int (entero)
  - b = 1.5 → float (decimales)
  - c = “Hello” → str (string o cadena de texto)
  - d = True → boolean (verdadero o falso)
  - e = None → NoneType (Sin valor)
  - f = “5” → str (5 y “5” no son lo mismo. La primera es un entero y la segunda una cadena de texto)
```py
>>> a = 1     
>>> b = 2
>>> c = a + b
>>> print (c)
>>> 
```
- Concatenando se pone entre comillas
```py
>>> a = 'ella'    
>>> b = 'no'
>>> c = 'te ama'
>>> d = a+b+c
>>> print (d)
>>> Ella no te ama
```
### Convertir un dato a un tipo diferente
- int(var) variable a entero
- float(var) variable a flotante
- str(var) variable a texto
- bool(var)variable a booleano
- abs(var) variable a valor absoluto
```py
>>> number1 = int(input("Escribe un numero: "))
Escribe un numero: 100
>>> number2 = int(input("Escribe otro numero: "))
Escribe otro numero: 300
>>> number1 + number2
=> 400
```
- Input("") para pedirle al usuario que introduzca datos.

- int() con datos o variables dentro de parentesis para convertirlo en número entero.

- str() para convertir números tanto decimales como enteros a strings.