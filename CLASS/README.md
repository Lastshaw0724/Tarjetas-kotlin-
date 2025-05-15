1.Describa el por qué y para qué se utiliza.

¿Por qué se utiliza?

Las clases en Kotlin se utilizan para representar entidades u objetos del mundo real o lógico dentro de un programa. Permiten organizar y encapsular datos (propiedades) junto con comportamientos (funciones o métodos) en una sola unidad. Esto sigue el principio de la programación orientada a objetos (POO), facilitando la reutilización de código, la modularidad y el mantenimiento del software.

¿Para qué se utiliza?

Se utiliza para definir nuevos tipos de datos personalizados que combinan atributos y comportamientos. Una clase puede servir para modelar cualquier cosa: desde un usuario, un producto, hasta conceptos más abstractos como un proceso o un evento. A partir de una clase, se pueden crear múltiples objetos o instancias con características individuales.

2. Genere un ejemplo internamente en el recuadro.

Utilice un editor de código para lograrlo.

[LINK DE CÓDIGO](https://pl.kotl.in/lMbP4-IVC)

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/CLASS/CLASS.mp3)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/CLASS/class.png)

Escribe una nota del cómo funciona la estructura

// Clase principal que demuestra el funcionamiento de los arrays en Kotlin
class ArrayDemo {

    // Propiedades de la clase
    private val colores = arrayOf("rojo", "verde", "azul")
    private val numeros = arrayOf(1, 2, 3, 4, 5)
    private val edades = IntArray(3)
    private val cuadrados = IntArray(5) { i -> i * i }

    // Método para mostrar arrays básicos
    fun mostrarArraysBasicos() {
        println("Array de colores: ${colores.joinToString()}")
        println("Array de números: ${numeros.joinToString()}")
        println("Array de edades (valores por defecto): ${edades.joinToString()}")
        println("Array de cuadrados: ${cuadrados.joinToString()}")
    }

    // Método para demostrar acceso y modificación
    fun accesoYModificacion() {
        println("\nColor original en posición 1: ${colores[1]}")
        colores[1] = "amarillo"
        println("Color modificado en posición 1: ${colores[1]}")
    }

    // Método para recorrer el array
    fun recorrerArray() {
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
    }

    // Método para mostrar el tamaño del array
    fun mostrarTamaño() {
        println("\nTamaño del array de colores: ${colores.size}")
    }

    // Método para demostrar una alternativa flexible: MutableList
    fun mostrarListaFlexible() {
        val lista = mutableListOf("uno", "dos")
        lista.add("tres")
        println("\nLista mutable (MutableList): $lista")
    }
}

// Clase de ejecución
fun main() {
    val demo = ArrayDemo()

    println("🔹 MOSTRAR ARRAYS BÁSICOS")
    demo.mostrarArraysBasicos()

    println("\n🔹 ACCESO Y MODIFICACIÓN")
    demo.accesoYModificacion()

    println("\n🔹 RECORRER ARRAY")
    demo.recorrerArray()

    println("\n🔹 TAMAÑO DEL ARRAY")
    demo.mostrarTamaño()

    println("\n🔹 ALTERNATIVA CON LISTA MUTABLE")
    demo.mostrarListaFlexible()
}
