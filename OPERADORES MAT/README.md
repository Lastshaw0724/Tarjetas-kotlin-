1. Describa el por qué y para qué se utiliza.

**OPERADORES EN KOTLIN**

 **Operadores Matemáticos**

En Kotlin, los operadores matemáticos permiten realizar operaciones aritméticas con números. A continuación se presentan los operadores más comunes:

* **Suma (+)**: Se usa para sumar dos valores numéricos.
* **Resta (-)**: Se usa para restar un valor de otro.
* **Multiplicación (\*)**: Multiplica dos valores.
* **División (/)**: Divide un valor por otro.
* **Módulo (%)**: Retorna el residuo de una división. Es útil para saber si un número es par, o para ciclos.

 **Operadores de Asignación**

Estos operadores modifican y asignan un valor a una variable de forma más compacta:

* **+=**: Suma y asigna el resultado.
* **-=**: Resta y asigna.
* **\*=**: Multiplica y asigna.
* **/=**: Divide y asigna.
* **% =**: Calcula el módulo y asigna.

**Conclusión**

Los operadores en Kotlin permiten realizar operaciones matemáticas, asignar valores a variables de manera compacta y facilitar la construcción de condiciones dentro del programa. Son herramientas fundamentales para trabajar con números y manipular el flujo de un programa de manera eficiente.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/DSm8Gd9F6)

Utilice un editor de código para lograrlo.

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/OPERADORES%20MAT/operadoresmat.png)

Escribe una nota del cómo funciona la estructura

// Clase que demuestra el uso de operadores matemáticos en Kotlin
class OperadoresMatematicosDemo {

    // Suma
    fun sumar(a: Int, b: Int): Int {
        return a + b
    }

    // Resta
    fun restar(a: Int, b: Int): Int {
        return a - b
    }

    // Multiplicación
    fun multiplicar(a: Int, b: Int): Int {
        return a * b
    }

    // División (con manejo de posible división por cero)
    fun dividir(a: Int, b: Int): Double {
        return if (b != 0) a.toDouble() / b else Double.NaN
    }

    // Modulo (residuo de la división)
    fun modulo(a: Int, b: Int): Int {
        return a % b
    }

    // Incremento y decremento
    fun incrementar(a: Int): Int {
        return a + 1
    }

    fun decrementar(a: Int): Int {
        return a - 1
    }

    // Demostración de los operadores matemáticos
    fun ejecutarDemostraciones() {
        val num1 = 10
        val num2 = 5

        // Suma
        println("🔹 Suma: $num1 + $num2 = ${sumar(num1, num2)}")

        // Resta
        println("🔹 Resta: $num1 - $num2 = ${restar(num1, num2)}")

        // Multiplicación
        println("🔹 Multiplicación: $num1 * $num2 = ${multiplicar(num1, num2)}")

        // División
        println("🔹 División: $num1 / $num2 = ${dividir(num1, num2)}")

        // Módulo
        println("🔹 Módulo: $num1 % $num2 = ${modulo(num1, num2)}")

        // Incremento
        println("🔹 Incremento: ${incrementar(num1)}")

        // Decremento
        println("🔹 Decremento: ${decrementar(num1)}")
    }
}

// Función main que ejecuta todas las demostraciones
fun main() {
    val demo = OperadoresMatematicosDemo()

    println("=== ➗ DEMOSTRACIÓN DE OPERADORES MATEMÁTICOS EN KOTLIN ===")
    demo.ejecutarDemostraciones()
}
