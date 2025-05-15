1. Describa el por qué y para qué se utiliza.

¿Por qué se utiliza un Looper en Kotlin?
Los loopers se utilizan en aplicaciones Android o en entornos donde hay hilos múltiples que necesitan ejecutar tareas de manera ordenada y controlada. Se garantiza que las operaciones en segundo plano no afecten el rendimiento o la interacción del usuario, ya que el Looper se encarga de gestionar las colas de mensajes y las tareas en segundo plano.

En Kotlin, el Looper trabaja en conjunto con los Handler para manejar las tareas dentro de los hilos. Se asocia con un hilo específico y puede ejecutar tareas de manera secuencial.

¿Para qué se utiliza un Looper?
Los loopers se utilizan principalmente en dos situaciones:

Gestión de la cola de mensajes: El Looper mantiene y procesa los mensajes (o tareas) que se agregan a la cola. Esto es común en aplicaciones Android, donde las tareas UI se gestionan en el hilo principal y otras operaciones en hilos secundarios.

Evitar el bloqueo del hilo principal: En aplicaciones que realizan operaciones en segundo plano, se usan loopers para mantener la UI interactiva mientras se gestionan los procesos en segundo plano.

2. Genere un ejemplo internamente en el recuadro.

🔗 [LINK DE CÓDIGO](https://pl.kotl.in/-i749olvs)


EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/LOOPERS/LOOPERS.mp3)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/LOOPERS/Captura%20de%20pantalla%202025-05-05%20162025.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra el uso de bucles (loopers) en Kotlin
class LoopersDemo {

    // Bucle FOR: recorre un rango
    fun bucleFor() {
        println("🔹 Bucle FOR (1 hasta 5):")
        for (i in 1..5) {
            println("  Iteración $i")
        }
    }

    // Bucle FOR con paso (step): recorre con un paso específico
    fun bucleForConPaso() {
        println("\n🔹 Bucle FOR con paso (de 0 a 10 con paso 2):")
        for (i in 0..10 step 2) {
            println("  $i")
        }
    }

    // Bucle FOR: recorre una lista
    fun bucleForEnLista() {
        val frutas = listOf("manzana", "banana", "cereza")
        println("\n🔹 Bucle FOR recorriendo lista:")
        for (fruta in frutas) {
            println("  Fruta: $fruta")
        }
    }

    // Bucle WHILE: continúa mientras se cumpla una condición
    fun bucleWhile() {
        var contador = 0
        println("\n🔹 Bucle WHILE (se detiene cuando contador > 3):")
        while (contador <= 3) {
            println("  Contador: $contador")
            contador++
        }
    }

    // Bucle DO-WHILE: se ejecuta al menos una vez
    fun bucleDoWhile() {
        var numero = 1
        println("\n🔹 Bucle DO-WHILE (se ejecuta al menos una vez):")
        do {
            println("  Número: $numero")
            numero++
        } while (numero <= 3)
    }

    // Uso de BREAK y CONTINUE en un bucle FOR
    fun breakYContinue() {
        println("\n🔹 Uso de BREAK y CONTINUE en un bucle FOR:")
        for (i in 1..5) {
            if (i == 3) {
                println("  Salta el número 3 (continue)")
                continue
            }
            if (i == 5) {
                println("  Rompe el bucle en el 5 (break)")
                break
            }
            println("  Iteración $i")
        }
    }

    // Método que ejecuta todas las demostraciones de bucles
    fun ejecutarDemostraciones() {
        bucleFor()
        bucleForConPaso()
        bucleForEnLista()
        bucleWhile()
        bucleDoWhile()
        breakYContinue()
    }
}

// Función main que ejecuta todas las demostraciones
fun main() {
    val demo = LoopersDemo()

    println("=== 🔄 DEMOSTRACIÓN DE BUCLES (LOOPERS) EN KOTLIN ===")
    demo.ejecutarDemostraciones()
}
