1. Describa el por qué y para qué se utiliza.

¿Por qué y para qué se utilizan las funciones en Kotlin?

En Kotlin, las funciones son bloques de código reutilizables que se pueden invocar para realizar tareas específicas. Las funciones se utilizan por varias razones importantes:

Reutilización de código:

Las funciones permiten escribir un conjunto de instrucciones una sola vez y luego reutilizarlas en diferentes partes del código. Esto evita la repetición de código, lo que mejora la legibilidad y el mantenimiento.

Modularidad:

Las funciones permiten dividir el código en partes más pequeñas, modulares y manejables. Cada función puede tener una responsabilidad clara y bien definida, lo que facilita el entendimiento del programa.

Abstracción:

Las funciones permiten ocultar los detalles de implementación, lo que facilita el trabajo con código complejo. Los usuarios de una función no necesitan saber cómo está implementada, solo cómo usarla.

Composición de funciones:

En Kotlin, las funciones pueden ser utilizadas para componer operaciones más complejas a partir de funciones más simples, lo que resulta en un código más limpio y flexible.


Soporte para funciones de orden superior:
Kotlin permite usar funciones como parámetros y devolver funciones desde otras funciones, lo que facilita la programación funcional.

¿Para qué se utilizan las funciones en Kotlin?

Las funciones se utilizan principalmente para:

Realizar tareas específicas o acciones dentro de un programa.

Mejorar la legibilidad y mantenibilidad del código, encapsulando lógicas en unidades más pequeñas.

Reducir la duplicación de código al permitir reutilización.

Facilitar la depuración y la prueba de unidades de código.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/-M_dJUoZ7)


EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/FUNCIONES/funciones.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra diferentes tipos de funciones en Kotlin
class FuncionesDemo {

    // Función simple que no recibe parámetros ni retorna valor
    fun saludar() {
        println("🔹 Hola, bienvenido a Kotlin!")
    }

    // Función con parámetros
    fun mostrarNombre(nombre: String) {
        println("🔹 Tu nombre es: $nombre")
    }

    // Función que retorna un valor
    fun sumar(a: Int, b: Int): Int {
        return a + b
    }

    // Función con parámetros por defecto
    fun saludarConEdad(nombre: String = "Invitado", edad: Int = 0) {
        println("🔹 Hola, $nombre. Tienes $edad años.")
    }

    // Función de una sola línea (inline)
    fun cuadrado(x: Int): Int = x * x

    // Función privada solo accesible dentro de esta clase
    private fun funcionPrivada() {
        println("🔹 Esta función es privada y no puede ser llamada desde fuera.")
    }

    // Método que demuestra el uso de las funciones anteriores
    fun ejecutarDemostraciones() {
        saludar()
        mostrarNombre("Laura")
        println("🔹 Suma de 5 + 3 = ${sumar(5, 3)}")
        saludarConEdad("Carlos", 20)
        saludarConEdad() // Usa valores por defecto
        println("🔹 El cuadrado de 6 es: ${cuadrado(6)}")

        // Llamada a función privada desde dentro de la clase
        funcionPrivada()
    }
}

// Función main que ejecuta la demo de funciones
fun main() {
    val demo = FuncionesDemo()

    println("=== 🧩 DEMOSTRACIÓN DE FUNCIONES EN KOTLIN ===")
    demo.ejecutarDemostraciones()
}
