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
### Operadores logicos y de comparacion
- and para comparar si dos valores son verdaderos.
- or para comparar si dos valores son falsos.
- not para invertir el valor booleano.
- == Compara dos valores y te dice si son iguales o no.
- != Compara dos valores y te dice sin son diferentes o no.
- -> Compara si es mayor que otro valor.
- -> Compara si es menor que otro valor.
- >= igual o mayor que el valor a comparar.
- <= igual o menor que el valor a comparar.

## Programa conversor de monedas
```py
def exchanges(moneda,cantidad):
    result = 0
    # Moneda chilena
    if moneda == 1:
        result = cantidad * 0.0013
        print(f'Los {cantidad} pesos chilenos equivalen a {result} dolares')
    # Moneda colombiana
    elif moneda == 2:
        result = cantidad * 0.00027
        print(f'Los {cantidad} pesos colombianos equivalen a {result} dolares')
    # Moneda Argentina
    elif moneda == 3:
        result = cantidad * 0.014
        print(f'Los {cantidad} pesos argentinos equivalen a {result} dolares')
    # Moneda mexicana
    elif moneda == 4:
        result = cantidad * 0.044
        print(f'Los {cantidad} pesos mexicanos equivalen a {result} dolares')
    # Otro
    else:
        print('Ingresa solo un numero de la lista')


if __name__ == '__main__':
    try:
        moneda = int(input('''
        Ingresa el indice de la moneda que quieres convertira  dolar:
            [1] Moneda chilena a Dolar
            [2] Moneda colombiana a Dolar
            [3] Moneda argentida a Dolar
            [4] Moneda mexicana a Dolar
        Selecciona: '''))
        print('********************************')
        cantidad = int(input('Ingresa la cantidad que quieres convertir: '))
        exchanges(moneda,cantidad)
    except:
        print('* * * * * * E R R O R * * * * * *')
        print('Por favor, Ingresa solo valores numericos')
```
### condicionales
- if
(Si) se usa para la condición principal.

- elif
(Si no) en caso de que la condición principal o anterior no se cumpla, se puede utilizar para agregar otra condición.

- else
(Sino) en caso de que la(s) condición(es) anterior(es) no se cumplan, se ejecuta como alternativa sin condicional.
```py
nacionalidad = input("¿Eres peruano? (Responde sí o no) ")
if nacionalidad == "sí":
    cambio_a_soles = 3.9865
    dolares = str(round(float(input("¿Cuántos soles tienes? "))/cambio_a_soles, 2))
    print("Entonces tienes " + dolares + " dólares.")
elif nacionalidad == "no":
    cambio_a_dolares = 0.25298
    soles = str(round(float(input("Bienvenido a Perú. ¿Cuántos dólares tienes? "))/cambio_a_dolares, 2))
    print("Entonces tienes " + soles + " soles.")
else:
    print("Escribe sólo sí o no, por favor. ")

```
```py
numero = input('Escribe un número: ')
numero = float(numero)

if numero > 5:
  print('Es mayor a cinco.')
elif numero == 5:
  print('Es igual a cinco.')
else:
  print('Es menor a cinco.')
  ```
  - convirtiendo con opciones
```py
from tkinter import Menu


Menu = """
Bienvenido al conversor de monedas
1.- Soles peruanos
2.- Pesos argentinos
3.- Pesos colombianos

Choose a option: """

opcion = int(input(Menu))
if opcion == 1:
    soles = input("¿Cuantos soles tienes?:")
    soles = float(soles)
    valor_dolar = 3.875
    dolares = soles/valor_dolar
    dolares = str(dolares)
    print("Tienes:"+dolares+"dolares")
elif opcion == 2:
    pesos = input("¿Cuantos pesos tienes?:")
    pesos = float(pesos)
    valor_dolar = 3.875
    dolares = pesos/valor_dolar
    print("Tienes"+dolares+"dolares")
else:
    print('Ingresa un numero correcto')
  ```
- ![Inicio](src/3.png)

### Aprendiendo a no repetir código con funciones
- Las funciones ayudan a optimizar el código. Es decir, utilizar la menor cantidad de líneas dentro del código y evitar escribir acciones repetitivas.

- Esto nos sirve para entregar un código más limpio y con buenas prácticas, que no desperdicia recursos innecesariamente. En Python, para definir funciones empleamos def.

- Gracias a def, podemos “definir” funciones que emplearemos más tarde. Una función, en programación, es un grupo de instrucciones con un objetivo en particular y que se ejecuta cuando es “invocada”.
```py
def conversacion(opcion):
    print('Hola')
    print('Cómo estás')
    print('Elegiste la opcion: ' + str(opcion))
    print('Adiós')

opcion = int(input('Ingrese una opción (1, 2, 3): '))

if opcion == 1:
    conversacion(opcion)

elif opcion == 2:
    conversacion(opcion)

elif opcion == 3:
    conversacion(opcion)

else:
    print('Escribe una opción correcta.')

```

### funciones
- Una función es un bloque de código que realiza alguna operación. Una función puede definir opcionalmente parámetros de entrada que permiten a los llamadores pasar argumentos a la función. Una función también puede devolver un valor como salida.
```PY
from tkinter import Menu
def conversor(tipo_pesos, valor_dolar):
    pesos = input("cuantos pesos" + tipo_pesos + "tienes?:")
    pesos = float(pesos)
    valor_dolar = 3.384
    dolares = pesos/valor_dolar
    dolares = str(dolares)
    print("Tienes $" + dolares + "dolares")
menu = """
Bienvenido al conversor de monedas
1.- Soles peruanos
2.- Pesos argentinos
3.- Pesos colombianos
Elige una opcion:"""
opcion = int(input(menu))

if opcion == 1:
    conversor("colombianos",3.789)
else:
    print("ELIGE UNA OPCION CORRECTA")
```
### Trabajando con texto: cadenas de caracteres
- Para trabajar con cadenas de texto en Python, vamos a aplicar una serie de métodos a las variables que hayamos creado anteriormente.
Método: es una función especial, que existe para un tipo de dato en particular. Por ejemplo, si queremos que el texto ingresado se transforme en mayúsculas.
- Métodos para trabajar con texto en Python:
  - variable.strip(): El método strip eliminará todos los caracteres vacíos que pueda contener la variable

  - variable.lower(): El método lower convertirá a las letras en minúsculas.

  - variable.upper(): El método upper convertirá a las letras en mayúsculas.

  - variable.capitalize(): El método capitalize convertirá a la primera letra de la cadena de caracteres en mayúscula.

  - variable.replace (‘o’, ‘a’): El método replace remplazará un caracterer por otro. En este caso remplazará todas las ‘o’ por el caracter ‘a’.

  - len(variable): Te indica la longitud de la cadena de texto dentro de la variable en ese momento.
  ```py
  >>> nombre = input ("writte your name: ")
  writte your name: jonathan
  >>> nombre
  'jonathan'
  >>> nombre.upper()
  'JONATHAN'
  >>> nombre.lower()
  'jonathan'
  >>> nombre.strip()
  'jonathan'
  >>> nombre.capitalize()
  'Jonathan'
  ```
### Trabajando con texto: slices
- En Python, los slices, traducidos al español como “rebanadas”, nos permiten dividir los caracteres de un string de múltiples formas. A continuación, realizaremos un ejemplo cómo utilizarlos:
```py
>>> nombre = "Francisco"
>>> nombre
>>> "Francisco"
>>> nombre[0 : 3]
El resultado sería
"Fra"
```
### Bucles
- Un bucle es un ciclo continuo en todos los lenguajes de programación que nos permite iterar sobre nuestros pasos: magina un contador cíclico (1,2,3,4,5,6…) donde puedes agregar un paso más sobre tu programa principal.
- Ejemplo de bucle en la vida real
  - Despertar
  - Estudiar en Platzi
  - Comer
  - Dormir
  ```py
    >>> def potencia(numero):
    
    potencia = 1

    while (potencia <= 10):
        
        result = numero ** potencia
        print('Potencia de {} elevado a la {} es {}'.format(numero, potencia, result))
        potencia += 1
        

    >>>  def run():
    numero = int(input('Escribe el numero al cual quieres averiguarle la potencia: '))
    potencia(numero)


    if __name__ == "__main__":
        run()

  ```
- Nos va salir 10 resultados
### bucle while
- Un bucle while permite repetir la ejecución de un grupo de instrucciones mientras se cumpla una condición (es decir, mientras la condición tenga el valor True).

- La sintaxis del bucle while es la siguiente:

  ```py
    def run():
    LIMITE = 1000000
    contador = 0
    potencia_2 = 2**contador
    while potencia_2 < LIMITE:
        print('2 elevado a ' + str(contador) +
              ' es igual a: ' + str(potencia_2))
        contador = contador + 1
        potencia_2 = 2**contador

    if __name__ == "__main__":
        run()

    ```

    ```py
        contador = 1
        print(contador)
        while contador < 1000:
            contador = contador + 1
            print(contador)
    ```
- cuenta del 1 a 1000
### for
- El ciclo for es un tipo de bucle usado cuando se conozcan la cantidad de veces a iterar.

- Un contador es una variable que se encarga de contener valores que irán incrementando o decrementando cada vez que se ejecuta una acción que lo contenga. El incremento o decremento es llamado paso del contador y es siempre constante.

- Ejemplo: El marcador de un partido de fútbol, cada vez que un equipo anote un gol, aumenta su marcador en una unidad.
- Su sintaxis es:
  - variable = variable + constante(al incrementar)
  - variable = variable - constante(al decrementar)

- o de manera resumida:

  - variable += constante
  - variable -= constante
    ```py
    for i in range(10):
        print(i)
    ```
### Proyecto final generador de contraseñas
```py
    import random
import string

def generate_password():
    # capitalize = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','Y','X','Y','Z']
    # lowercase = [letter.lower() for letter in capitalize] 
    # symbols = ['?','¡','¿','%','&','$','#','/','!','+','[']
    # numbers = ['1','2','3','4','5','6','7','8','9','10']

    # characters = capitalize + lowercase + symbols + numbers

    characters = string.ascii_lowercase + string.ascii_uppercase + string.digits + string.punctuation

    password = []

    for i in range(15):
        character_random = random.choice(characters)
        password.append(character_random)

    password = "".join(password)

    return password



def run ():
    password = generate_password()
    print('Your new password is: ' + password)

if __name__ == '__main__':
    run()
```
## CursodeFundamentosdeÁlgebraLinealconython
- El álgebra lineal es una rama de las matemáticas que estudia conceptos tales como vectores, matrices, espacio dual, sistemas de ecuaciones lineales y en su enfoque de manera más formal, espacios vectoriales y sus transformaciones lineales.
- Por qué Python para Data Science:
  - Si ya conoces el lenguaje Python no hace falta que te cuente porque es el elegido en la industria para dar vida a los proyectos de Data Science. Pero si no estás familiarizado con Python estas son algunas de sus características:

   - Es poderoso y sencillo
   - Tiene múltiples paquetes estadísticos y de aprendizaje automático, listos para usar
   - Una comunidad muy activa a la que siempre puedes consultar
- Por qué Anaconda:
  - Anaconda nos provee de una plataforma muy completa para poder desarrollar nuestros proyectos de Data Science, simplifica la tarea de instalación y configuración de las distintas aplicaciones que necesitaremos usar en nuestro viaje. Podemos utilizarlo tanto por terminal como por interfaz gráfica (GUI). Por el momento avancemos con la segunda opción, es más amigable para quien no está acostumbrado a la línea de comandos.
  - Instalacion:
  - Ir a https://www.anaconda.com/distribution/
  - Selecciona tu versión de Sistema Operativo: Windows - macOS - Linux
  - Haz click en Descargar/Download “Python 3.7 version” (o click en la versión adecuada para tu CPU 64-bit o 32-bit)
- Iniciando Anaconda
Una vez que finalizada la instalación debes abrir el programa Anaconda Navigator para que podamos crear el entorno en cual estaremos estudiando y actualizar los paquetes.

- Haz click en Environments y despues click en +Create. Se abrirá una ventana para crear un nuevo entorno.
- ![Inicio](src/4.webp)
- Llena los siguientes campos:
- ![Inicio](src/5.webp)
- Name: jacob - FundamentosAL
- Packages: tilde en Python y del menú desplegable selecciona 3.7
- ![Inicio](src/6.webp)
- momento para configurar el nuevo entorno y actualizarlo. Cuando termine verás una pantalla similar a esta
- ![Inicio](src/7.webp)
- Los paquetes que ves son los que están instalados por defecto, necesitas instalar varios más. Haz click en installed y cambiarlo a not installed.
- ![Inicio](src/8.webp)
- En el recuadro de search packages pon:

   - Jupyter Notebook
   - scipy (tambien instalará numpy)
   - pillow (libreria para manejo de imágenes)
   - imageio (lectura / escritura de imágenes)
   - matplotlib (para graficar)
   - seaborn (visualizaciones estadísticas)
   - scikit-learn (aprendizaje automático - lo usaremos para un ejemplo de PCA)
- EJERCICIO
 - Instala el paquete seaborn. Es un paquete para visualizar datos.
   - 1 - Desde Anaconda Navigator, haz click en Environments
   - 2 - Selecciona el entorno donde quieres instalar el paquete (Jacob - FundamentosAL)
   - 3 - Selecciona en el menú desplegable Not Installed
   - 4 - Escribe en el recuadro de búsqueda seaborn
   - 5 - Haz click en el paquete seaborn
   - 6 - Haz click en Apply
   - 7 - Haz click en Apply, pero esta vez en el pop up que aparece para aceptar todas las dependencias.
- copia el siguiente codigo:
    ```js
        import seaborn as sns
        vuelos = sns.load_dataset("flights")
        vuelos = vuelos.pivot("month", "year", "passengers")
        ax = sns.heatmap(vuelos)
    ```
- A los que no les aparezcan los paquetes en “Not Installed”, sólo tienen que darle a “Update index…”.
