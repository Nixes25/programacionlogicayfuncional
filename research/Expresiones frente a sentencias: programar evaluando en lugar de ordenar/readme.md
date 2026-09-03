### Expresiones frente a sentencias: programar evaluando en lugar de ordenar

En programación, la distinción entre expresiones y sentencias es fundamental para comprender cómo los lenguajes procesan instrucciones. Una expresión es cualquier construcción que puede evaluarse y producir un valor. Por ejemplo, 3 + 5 devuelve 8, y "Hola".upper() devuelve "HOLA". En cambio, una sentencia es una instrucción que el intérprete o compilador ejecuta para realizar una acción, como print("Hola") o if x > 0:.

La diferencia clave es que las expresiones responden a una pregunta (¿qué valor resulta de esto?), mientras que las sentencias dan una orden (haz esto ahora).

## Contexto historico
Los primeros lenguajes como FORTRAN y COBOL estaban dominados por sentencias, reflejando la idea de dar órdenes a la máquina. Con el tiempo, lenguajes como LISP introdujeron un paradigma basado en expresiones, donde todo se evalúa y devuelve un valor. Esta evolución refleja un cambio filosófico: de “ordenar” a la computadora hacia “describir” el problema y dejar que el lenguaje lo resuelva.

## Diferencias principales

| Concepto | **[Expresión](ca://s?q=Que_es_una_expresion_en_programacion)** | **[Sentencia](ca://s?q=Que_es_una_sentencia_en_programacion)** |
| --- | --- | --- |
| **Definición** | Combinación de variables, literales y operadores que se evalúa a un valor. | Unidad mínima de ejecución que realiza una acción en el programa. |
| **Resultado** | Siempre devuelve un valor (ej. ``3 ``+ ``5`` → 8). | No necesariamente devuelve un valor (ej. ``if ``x ``> ``0:``). |
| **Ejemplos** | ``3 ``+ ``5``, ``map(lambda ``x: ``x*x, ``range(10))``, ``[a.x ``for ``a ``in ``iterable]``. | ``print(42)``, ``a ``= ``7``, ``if ``x: ``do_y()``. |
| **Uso** | Se emplean para cálculos, asignaciones, condiciones en línea. | Se emplean para control de flujo, asignaciones, invocaciones de métodos. |
| **Relación** | Una expresión puede ser usada como sentencia. | No todas las sentencias son expresiones. |

## Ejemplos prácticos 
*Expresiones en Python*
```
A[3 + 5        # devuelve 8
"Hola".upper()  # devuelve "HOLA"
x if x > 0 else -x  # condicional en línea
```
*Sentencias en Python*
```
a = 7        # asignación
print("Hola")  # acción de salida
if x > 0:     # control de flujo
    print("positivo")
```
## Evaluar contra ordenar
*Expresiones → Evaluar  
Se centran en calcular y devolver un valor. Son como preguntas al programa: “¿Cuál es el resultado de esto?”  
Ejemplo: resultado = (x + 3) * 2.

*Sentencias → Ordenar  
Son instrucciones que el programa debe ejecutar. Son como órdenes: “Haz esto ahora.”  
Ejemplo: if x > 0: print("positivo").

## Ventajas
*Expresiones*

-Favorecen la claridad y la composición.

-Permiten escribir código más conciso y declarativo.

-Reducen efectos secundarios, lo que facilita pruebas y razonamiento.

*Sentencias*

-Más intuitivas para describir procesos paso a paso.

-Útiles en programación de sistemas y control de flujo complejo.

-Se integran bien con estructuras de control tradicionales.

## Conclusión
Programar “evaluando” con expresiones fomenta un estilo más funcional y declarativo, donde el código describe qué resultado se busca. En cambio, programar con sentencias es más imperativo, indicando paso a paso qué hacer.
Por eso lenguajes como Haskell o Scala se apoyan más en expresiones, mientras que lenguajes como C++ o Java se basan en sentencias para estructurar la ejecución.

