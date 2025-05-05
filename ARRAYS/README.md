ARRAYS EN KOTLIN

En Kotlin, los arrays son estructuras que permiten almacenar múltiples elementos del mismo tipo en una sola variable. Son muy útiles cuando necesitas manejar listas de datos fijos y acceder a ellos por su posición.

¿Por qué se usan?

-Para agrupar datos relacionados bajo una sola variable.

-Para acceder rápidamente a elementos usando un índice.

-Para modificar valores en posiciones específicas.

¿Cómo se declaran?

-Array de enteros: val numeros: Array<Int> = arrayOf(1, 2, 3, 4, 5)

-Array de strings: val nombres: Array<String> = arrayOf("Ana", "Luis", "Pedro")

-Array de booleanos: val estados: Array<Boolean> = arrayOf(true, false, true)

Operaciones comunes

-Acceder a un elemento: println(nombres[0])  // Imprime: Ana

-Modificar un valor: nombres[1] = "Lucía" println(nombres[1])  // Imprime: Lucía

-Obtener el tamaño: println(nombres.size)  // Imprime: 3
