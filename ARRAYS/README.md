1. Describa el por qué y para qué se utiliza.

**ARRAYS EN KOTLIN**

 **¿Qué son los arrays?**

Un **array** es una estructura de datos que permite **almacenar múltiples valores del mismo tipo** (por ejemplo, solo enteros, solo cadenas, etc.) en una sola variable. Es decir, en lugar de crear variables individuales para cada valor, puedes guardar todos esos datos dentro de un mismo array, organizados por posiciones llamadas **índices**.

Cada valor en un array está asociado a una posición numérica, que comienza en **0**. Esto significa que el primer elemento está en la posición `0`, el segundo en la `1`, y así sucesivamente.


 **¿Para qué se utilizan los arrays?**

Los arrays se utilizan cuando:

* Necesitas manejar **varios datos del mismo tipo juntos**, como nombres de estudiantes, calificaciones, o estados de conexión.
* Requieres **acceder rápidamente** a ciertos elementos mediante su **índice**.
* Quieres **modificar elementos** directamente sin recorrer toda la colección.
* El número de elementos es **conocido y fijo** (para colecciones variables, se usa `List` o `MutableList`).

Por ejemplo, en una aplicación escolar, podrías usar un array para almacenar los nombres de los estudiantes de un curso.



 **Cómo se declaran los arrays en Kotlin**

Kotlin proporciona una forma sencilla de declarar arrays mediante la función `arrayOf()`:

kotlin
val numeros: Array<Int> = arrayOf(1, 2, 3, 4, 5)       // Array de enteros
val nombres: Array<String> = arrayOf("Ana", "Luis", "Pedro")  // Array de cadenas
val estados: Array<Boolean> = arrayOf(true, false, true)      // Array de valores booleanos


Cada array es un **objeto en sí mismo**, con propiedades y funciones útiles como `size`, `get()`, `set()`, etc.



 **Operaciones comunes con arrays**

Una vez que tienes un array, puedes hacer varias operaciones con él:

kotlin
// Acceder a un valor por índice
println(nombres[0])  // Resultado: Ana

// Cambiar el valor de un elemento
nombres[1] = "Lucía"
println(nombres[1])  // Resultado: Lucía

// Obtener el número total de elementos
println(nombres.size)  // Resultado: 3

**Este código imprime:**


Primer estudiante: Carlos
Nombre actualizado: Marta
Total de estudiantes: 3

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/q8JLfKDgT)

Utilice un editor de código para lograrlo.

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/ARRAYS/ARRAYS.mp3).

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/ARRAYS/arrays.png)

Escribe una nota del cómo funciona la estructura

// Ejemplo completo de cómo funcionan los arrays en Kotlin

fun main() {

    // -------------------------------
    // 🔹 CREACIÓN DE ARRAYS
    // -------------------------------

    // Usando arrayOf() - para cualquier tipo de datos
    val numeros = arrayOf(1, 2, 3, 4, 5)
    val palabras = arrayOf("hola", "mundo")

    // Usando IntArray - para arrays de enteros (valores por defecto: 0)
    val edades = IntArray(3)  // [0, 0, 0]

    // Usando función de inicialización con índice
    val cuadrados = IntArray(5) { i -> i * i }  // [0, 1, 4, 9, 16]

    // -------------------------------
    // 🔹 ACCESO Y MODIFICACIÓN
    // -------------------------------

    val colores = arrayOf("rojo", "verde", "azul")

    // Acceder a un elemento por índice
    println("Color en posición 1: ${colores[1]}")  // verde

    // Modificar un elemento por índice
    colores[1] = "amarillo"
    println("Nuevo color en posición 1: ${colores[1]}")  // amarillo

    // -------------------------------
    // 🔹 RECORRER UN ARRAY
    // -------------------------------

    println("\nRecorrido con for-each:")
    for (color in colores) {
        println(color)
    }

    println("\nRecorrido con índices:")
    for (i in colores.indices) {
        println("Índice $i: ${colores[i]}")
    }

    println("\nRecorrido con forEachIndexed:")
    colores.forEachIndexed { index, valor ->
        println("[$index] = $valor")
    }

    // -------------------------------
    // 🔹 TAMAÑO DEL ARRAY
    // -------------------------------

    println("\nEl array de colores tiene ${colores.size} elementos.")

    // -------------------------------
    // 🔹 LIMITACIONES Y ALTERNATIVA
    // -------------------------------

    // Los arrays tienen tamaño fijo, no se puede agregar ni eliminar elementos.
    // Para una estructura más flexible se usa MutableList:
    val lista = mutableListOf("uno", "dos")
    lista.add("tres")  // Ahora lista contiene: ["uno", "dos", "tres"]
    println("\nLista mutable: $lista")
}

