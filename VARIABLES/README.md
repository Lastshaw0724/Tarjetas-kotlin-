1. Describa el por qué y para qué se utiliza.

 **MANEJO DE VARIABLES EN KOTLIN**

 **¿Por qué y para qué se utilizan?**

El manejo de variables en Kotlin es muy importante porque es un lenguaje **fuertemente tipado**, lo que significa que cada variable debe tener un tipo de dato específico. Esto permite que el programa sea más seguro, evitando errores de tipos de datos en tiempo de ejecución y facilitando que el compilador detecte errores desde etapas tempranas.

Las variables se utilizan para **almacenar datos** que el programa necesita manipular, procesar o recordar mientras se ejecuta. Son esenciales para:

* Guardar información de forma temporal o permanente.
* Modificar valores cuando sea necesario.
* Realizar operaciones matemáticas, lógicas o de control.
* Organizar mejor el flujo del programa mediante el manejo de datos de manera estructurada.

**Declaración de variables en Kotlin**

* `val`: Para variables **inmutables** (constantes). No pueden cambiar su valor después de ser asignadas.
* `var`: Para variables **mutables**. Su valor puede cambiar durante la ejecución del programa.

 **Tipos de variables comunes**

* **Int**: Para números enteros.
* **Double**: Para números decimales con mayor precisión.
* **Float**: Para números decimales con menor precisión.
* **Boolean**: Para valores lógicos (`true` o `false`).
* **Char**: Para representar un solo carácter.
* **String**: Para cadenas de texto.

 
2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/h54pJ4pIK)

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/VARIABLES/VARIABLES.mp3)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/VARIABLES/vartyp.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra el uso de variables en Kotlin
class VariablesDemo {

    // Variables inmutables (val) y mutables (var)
    fun mostrarVariables() {
        // Variable inmutable (no se puede cambiar su valor)
        val nombre: String = "Juan"
        // nombre = "Carlos" // Esto causaría un error porque 'val' no permite cambiar el valor.
        println("🔹 Nombre: $nombre")

        // Variable mutable (puede cambiar su valor)
        var edad: Int = 25
        println("🔹 Edad: $edad")

        // Modificación de la variable mutable
        edad = 30
        println("🔹 Edad actualizada: $edad")

        // Variables con inferencia de tipo (Kotlin infiere el tipo automáticamente)
        val ciudad = "Medellín"  // Kotlin infiere que es un String
        var altura = 1.75  // Kotlin infiere que es un Double

        println("🔹 Ciudad: $ciudad")
        println("🔹 Altura: $altura")
    }

    // Variables de tipos básicos
    fun tiposBasicos() {
        // Entero
        val numeroEntero: Int = 42
        println("🔹 Número Entero: $numeroEntero")

        // Flotante (Decimal)
        val numeroDecimal: Double = 3.1416
        println("🔹 Número Decimal: $numeroDecimal")

        // Booleano
        val esKotlinGenial: Boolean = true
        println("🔹 ¿Es Kotlin genial?: $esKotlinGenial")

        // Caracter (Char)
        val letra: Char = 'K'
        println("🔹 Letra: $letra")

        // Cadena (String)
        val saludo: String = "¡Hola, Kotlin!"
        println("🔹 Saludo: $saludo")
    }

    // Uso de variables dentro de una función
    fun ejecutarDemostraciones() {
        mostrarVariables()
        tiposBasicos()
    }
}

// Función main que ejecuta todas las demostraciones
fun main() {
    val demo = VariablesDemo()

    println("=== 🛠️ DEMOSTRACIÓN DE VARIABLES EN KOTLIN ===")
    demo.ejecutarDemostraciones()
}
