1. Describa el por qué y para qué se utiliza.

**FUNCIONES DE STRINGS Y PRINTING EN KOTLIN**

 **Cadenas en Kotlin (String)**

En Kotlin, una cadena o **String** es una secuencia de caracteres que puedes utilizar para representar texto. Los Strings en Kotlin son **inmutables**, lo que significa que una vez que se crea una cadena, no puedes modificarla directamente. En su lugar, puedes crear nuevas cadenas basadas en operaciones realizadas sobre la original.

**¿Por qué se usan los Strings?**

Los Strings se utilizan cuando necesitas almacenar y manipular texto en tu programa. Esto puede incluir tareas como:

* **Almacenar información textual** como nombres, direcciones, mensajes, etc.
* **Realizar operaciones sobre el texto**: Como concatenación, comparación, búsqueda o reemplazo de caracteres o subcadenas.
* **Combinar texto con variables** de forma sencilla usando la interpolación de cadenas.

**Características principales de los Strings**

* **Definición**: Las cadenas en Kotlin se definen entre comillas dobles (`""`). Por ejemplo, `"Hola Mundo"` es un String.

* **Inmutabilidad**: Los Strings en Kotlin son inmutables. Si quieres cambiar un carácter o parte de la cadena, deberás crear una nueva cadena.

* **Interpolación de variables**: Puedes insertar valores de variables o expresiones dentro de una cadena usando el símbolo `$`. Esto hace que la manipulación de texto sea mucho más fácil y legible.


**Conclusión**

Las cadenas en Kotlin son herramientas muy poderosas y versátiles que permiten almacenar, manipular y mostrar texto de manera eficiente. Con las funciones de Strings y las herramientas de impresión, podemos realizar una amplia variedad de operaciones de forma sencilla y directa.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/yk3pzTqb0)

Utilice un editor de código para lograrlo.

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://tuenlace.com/audio.mp4)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/CADENA/cadena.png)

Escribe una nota del cómo funciona la estructura

// Clase principal que demuestra el uso de funciones de cadenas y técnicas de impresión en Kotlin
class StringsAndPrintingDemo {

    // Propiedades: ejemplos de cadenas
    private val saludo = "¡Hola, Kotlin!"
    private val nombre = "Juan"
    private val fraseLarga = "La programación en Kotlin es divertida y poderosa."

    // Métodos para demostrar operaciones con cadenas
    fun mostrarCadenaOriginal() {
        println("🔹 Cadena original: $saludo")
    }

    fun mostrarConcatenacion() {
        val mensaje = saludo + " Mi nombre es " + nombre
        println("🔹 Concatenación de cadenas: $mensaje")
    }

    fun mostrarInterpolacion() {
        val mensaje = "Mi nombre es $nombre y estoy aprendiendo Kotlin."
        println("🔹 Interpolación de cadenas: $mensaje")
    }

    fun mostrarLongitudYSubcadena() {
        println("\n🔹 Longitud de la cadena '$saludo': ${saludo.length}")
        println("🔹 Subcadena de '$fraseLarga' (0, 10): ${fraseLarga.substring(0, 10)}")
    }

    fun mostrarTransformaciones() {
        println("\n🔹 Convertir a mayúsculas: ${saludo.uppercase()}")
        println("🔹 Convertir a minúsculas: ${saludo.lowercase()}")
        println("🔹 Reemplazar 'Kotlin' por 'Java': ${fraseLarga.replace("Kotlin", "Java")}")
    }

    fun mostrarEspaciosYRecorte() {
        val cadenaConEspacios = "   Kotlin es genial   "
        println("\n🔹 Cadena original con espacios: '$cadenaConEspacios'")
        println("🔹 Recortar espacios: '${cadenaConEspacios.trim()}'")
    }

    fun mostrarComprobaciones() {
        println("\n🔹 Comprobación si la cadena contiene 'Kotlin': ${fraseLarga.contains("Kotlin")}")
        println("🔹 Comprobación si la cadena comienza con 'La': ${fraseLarga.startsWith("La")}")
        println("🔹 Comprobación si la cadena termina con 'poderosa.': ${fraseLarga.endsWith("poderosa.")}")
    }

    fun imprimirCadena() {
        println("\n🔹 Imprimir cadena con println: $saludo")
        print("🔹 Imprimir sin salto de línea con print: ")
        print(saludo)
        println(" - ¡Esto es Kotlin!")
    }
}

// Clase de ejecución
fun main() {
    val demo = StringsAndPrintingDemo()

    println("=== 📚 DEMO DE FUNCIONES DE STRINGS Y PRINTING EN KOTLIN ===\n")
    demo.mostrarCadenaOriginal()
    demo.mostrarConcatenacion()
    demo.mostrarInterpolacion()
    demo.mostrarLongitudYSubcadena()
    demo.mostrarTransformaciones()
    demo.mostrarEspaciosYRecorte()
    demo.mostrarComprobaciones()
    demo.imprimirCadena()
}

Explicación de lo que hace el código:
Concatenación de cadenas: Combina las cadenas usando el operador +.

Interpolación de cadenas: Usa $ para insertar variables directamente dentro de una cadena.

Funciones de longitud y subcadena: length para obtener la longitud de una cadena y substring() para extraer una parte de ella.

Transformaciones de cadenas: Convierte a mayúsculas, minúsculas y reemplaza partes de la cadena.

Recorte de espacios: Usa trim() para eliminar los espacios al principio y al final de la cadena.

Comprobaciones de cadenas: Usa contains(), startsWith(), y endsWith() para realizar búsquedas o comprobaciones dentro de las cadenas.

Impresión: Demuestra el uso de println para imprimir con salto de línea y print para imprimir sin salto.


