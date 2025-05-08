1. Describa el por qué y para qué se utiliza.

¿Por qué y para qué se utilizan las funciones paramétricas con colecciones en Kotlin?

Las funciones paramétricas en Kotlin son aquellas funciones que aceptan parámetros para realizar alguna tarea. Al combinar funciones paramétricas con colecciones (como listas, conjuntos y mapas), se obtiene un poder de manipulación y transformación de datos mucho mayor, permitiendo a los programadores crear soluciones flexibles y reutilizables.

¿Por qué se utilizan las funciones paramétricas con colecciones?

Reutilización de código: Las funciones paramétricas permiten que el mismo bloque de código se use con diferentes colecciones y tipos de datos, lo que evita la duplicación de lógica y aumenta la mantenibilidad del programa.

Flexibilidad: Las colecciones en Kotlin son altamente flexibles y se pueden usar con funciones paramétricas para transformar, filtrar, agrupar o mapear elementos de la colección, proporcionando gran versatilidad en la programación.

Mayor expresividad: Al permitir pasar colecciones como parámetros, las funciones se vuelven más expresivas, permitiendo realizar operaciones complejas de manera concisa.

Transformaciones y manipulaciones de datos: Combinando funciones paramétricas con colecciones, es posible realizar operaciones como búsqueda, filtrado, ordenación, etc., sobre los datos de manera eficiente y en una sola línea de código.

¿Para qué se utilizan las funciones paramétricas con colecciones?

Filtrar elementos: Por ejemplo, filtrar una lista de estudiantes que hayan aprobado un examen.

Transformar datos: Como cuando se quiere convertir una lista de enteros en su versión cuadrada.

Realizar cálculos: Como sumar o multiplicar todos los elementos de una colección.

Buscar elementos: Encontrar un elemento específico dentro de una colección, etc.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/0v56nF-4q)

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/FUNCIONESPARAMETRICAS/funparametricas.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra funciones paramétricas en Kotlin
class FuncionesParametricasDemo {

    // Función con un parámetro simple
    fun multiplicarPorDos(numero: Int): Int {
        return numero * 2
    }

    // Función con múltiples parámetros
    fun concatenarStrings(str1: String, str2: String): String {
        return str1 + " " + str2
    }

    // Función con parámetros de diferentes tipos
    fun mostrarInfo(nombre: String, edad: Int): String {
        return "Nombre: $nombre, Edad: $edad años"
    }

    // Función con tipo genérico, que acepta cualquier tipo de parámetro
    fun <T> imprimirValor(valor: T): String {
        return "El valor es: $valor"
    }

    // Función que recibe un parámetro por referencia (tipo mutable)
    fun modificarLista(lista: MutableList<String>) {
        lista.add("Nuevo Elemento")
    }

    // Función que retorna un valor calculado según los parámetros
    fun promedio(a: Double, b: Double): Double {
        return (a + b) / 2
    }

    // Función que muestra el uso de las funciones anteriores
    fun ejecutarDemostraciones() {
        // Uso de funciones simples con parámetros
        println("🔹 Multiplicar 4 por 2: ${multiplicarPorDos(4)}")
        println("🔹 Concatenar 'Hola' y 'Mundo': ${concatenarStrings("Hola", "Mundo")}")
        println("🔹 Mostrar Info: ${mostrarInfo("Carlos", 25)}")
        
        // Uso de función con tipo genérico
        println("🔹 Imprimir valor: ${imprimirValor(123)}")
        println("🔹 Imprimir valor de tipo String: ${imprimirValor("Texto")}")

        // Uso de función que modifica un parámetro (referencia)
        val lista = mutableListOf("Elemento1", "Elemento2")
        println("🔹 Lista original: $lista")
        modificarLista(lista)
        println("🔹 Lista después de modificarla: $lista")

        // Uso de función con retorno de valor calculado
        println("🔹 Promedio de 5.5 y 10.5: ${promedio(5.5, 10.5)}")
    }
}

// Función main que ejecuta todas las funciones paramétricas
fun main() {
    val demo = FuncionesParametricasDemo()

    println("=== ⚙️ DEMOSTRACIÓN DE FUNCIONES PARAMÉTRICAS EN KOTLIN ===")
    demo.ejecutarDemostraciones()
}
