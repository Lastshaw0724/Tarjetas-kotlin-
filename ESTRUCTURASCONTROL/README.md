1. Describa el por qué y para qué se utiliza.

¿Por qué y para qué se utiliza el control de flujo en Kotlin?

En Kotlin, las estructuras de decisión, control y manejo de errores son fundamentales para controlar el flujo de ejecución de un programa y asegurarse de que se realicen las acciones adecuadas dependiendo de las condiciones del programa. Estas estructuras permiten a un programa tomar decisiones, repetir acciones o manejar excepciones para que no se produzcan fallos inesperados en tiempo de ejecución.

1. Estructuras de Decisión (Condicionales)
   
Las estructuras de decisión permiten que el programa elija entre distintas opciones según una condición. Kotlin proporciona varias formas de hacer esto:

if: Evaluación de una condición y ejecución de bloques de código según el resultado.

when: Se utiliza para hacer comparaciones más legibles y de múltiples condiciones (similar al switch de otros lenguajes).

2. Estructuras de Control (Bucles)
   
Las estructuras de control permiten que el programa repita una serie de instrucciones varias veces:

for: Se utiliza para iterar sobre rangos, colecciones u objetos iterables.

while y do while: Ejecutan un bloque de código mientras se cumpla una condición.

3. Manejo de Errores (Excepciones)
   
El manejo de errores permite que el programa maneje situaciones excepcionales sin que se detenga por completo. Kotlin proporciona:

try-catch: Para capturar excepciones y manejar errores.

throw: Para lanzar excepciones personalizadas.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/bkqtjrm9Y)

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/ESTRUCTURASCONTROL/ESTRUCTURAS-DE-CONTROL.mp3)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/ESTRUCTURASCONTROL/estructura.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra las estructuras de control en Kotlin
class EstructurasDeControl {

    // Condicionales simples: if / else
    fun condicionalIf() {
        val temperatura = 30
        println("🔹 IF / ELSE:")
        if (temperatura > 25) {
            println("  Hace calor")
        } else {
            println("  Hace frío")
        }
    }

    // Condicional múltiple: when
    fun condicionalWhen() {
        val nota = 4
        println("\n🔹 WHEN:")
        when (nota) {
            0 -> println("  Reprobado")
            1, 2, 3 -> println("  Muy bajo")
            4, 5 -> println("  Aprobado")
            in 6..10 -> println("  Excelente")
            else -> println("  Nota inválida")
        }
    }

    // Bucle FOR
    fun bucleFor() {
        println("\n🔹 FOR (del 1 al 5):")
        for (i in 1..5) {
            println("  i = $i")
        }
    }

    // Bucle WHILE
    fun bucleWhile() {
        println("\n🔹 WHILE:")
        var contador = 3
        while (contador > 0) {
            println("  Contador: $contador")
            contador--
        }
    }

    // Bucle DO-WHILE
    fun bucleDoWhile() {
        println("\n🔹 DO-WHILE:")
        var numero = 1
        do {
            println("  Número: $numero")
            numero++
        } while (numero <= 3)
    }

    // Uso de break y continue
    fun breakYContinue() {
        println("\n🔹 BREAK y CONTINUE:")
        for (i in 1..5) {
            if (i == 2) {
                println("  Salta el 2 (continue)")
                continue
            }
            if (i == 4) {
                println("  Rompe en 4 (break)")
                break
            }
            println("  i = $i")
        }
    }
}

// Función main para ejecutar todas las demostraciones
fun main() {
    val demo = EstructurasDeControl()

    println("=== 🔧 DEMOSTRACIÓN DE ESTRUCTURAS DE CONTROL EN KOTLIN ===")
    demo.condicionalIf()
    demo.condicionalWhen()
    demo.bucleFor()
    demo.bucleWhile()
    demo.bucleDoWhile()
    demo.breakYContinue()
}
