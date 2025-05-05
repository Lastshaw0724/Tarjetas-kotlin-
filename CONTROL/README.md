CONTROL DE FLUJO EN KOTLIN

El control de flujo en Kotlin permite que el programa decida qué instrucciones ejecutar y cuántas veces hacerlo según ciertas condiciones. Es la base para crear programas que puedan tomar decisiones o repetir tareas de manera automática.

¿Por qué se usa?

-Para ejecutar código solo si se cumple una condición.

-Para repetir acciones (loops) sin tener que escribir el mismo código muchas veces.

-Para controlar la ejecución (por ejemplo, salir de un bucle antes de que termine).

CONDICIONALES

Permiten ejecutar código basado en condiciones.

-if / else:

val numero = 10
if (numero > 0) {
    println("El número es positivo")
} else {
    println("El número es negativo o cero")
}

-when: (similar a switch en otros lenguajes)

val dia = 3
when (dia) {
    1 -> println("Lunes")
    2 -> println("Martes")
    3 -> println("Miércoles")
    else -> println("Otro día")
}

 BUCLES (LOOPS)
 
Permiten repetir un bloque de código varias veces.

-for: Recorre una colección o un rango.

for (i in 1..5) {
    println("Número: $i")
}

-while: Repite mientras la condición sea verdadera.

var contador = 1
while (contador <= 3) {
    println("Contador: $contador")
    contador++
}

-do-while: Igual que while, pero se ejecuta al menos una vez.

var x = 5
do {
    println("x: $x")
    x--
} while (x > 0)

 INSTRUCCIONES DE SALTO
 
Permiten alterar el flujo normal de ejecución.

-break: Sale inmediatamente de un bucle.

for (i in 1..5) {
    if (i == 3) break
    println(i)
}
// Salida: 1, 2

-continue: Salta a la siguiente iteración

for (i in 1..5) {
    if (i == 3) continue
    println(i)
}
// Salida: 1, 2, 4, 5}

-return: Sale de la función actual.

fun mensaje() {
    println("Antes del return")
    return
    println("Esto nunca se imprimirá")
}
