1. Describa el por qué y para qué se utiliza.

¿Por qué y para qué se utilizan las colecciones en Kotlin?

Las colecciones en Kotlin son estructuras de datos que permiten almacenar y manipular grupos de elementos. Se utilizan para organizar y gestionar datos de manera eficiente en aplicaciones.

El uso de colecciones es esencial porque:

Organización y Acceso Rápido a los Datos: Las colecciones permiten almacenar grandes cantidades de datos en una estructura que facilita el acceso rápido a los mismos.

Tipos de Colecciones:

Listas: Son colecciones ordenadas que permiten duplicados. Se pueden acceder a sus elementos por índice.

Conjuntos (Sets): Son colecciones no ordenadas que no permiten duplicados.

Mapas: Son colecciones que almacenan pares clave-valor, permitiendo acceder a los valores a través de las claves.

Facilidad de Manipulación: Kotlin ofrece funciones poderosas y sencillas para manipular colecciones como map(), filter(), reduce(), y forEach(), lo que hace que trabajar con ellas sea más sencillo y expresivo.

Inmutabilidad y Mutabilidad: Kotlin permite trabajar con colecciones inmutables (no puedes cambiar sus elementos después de la creación) y mutables (puedes agregar, quitar o modificar elementos después de la creación). Esto da flexibilidad en cómo se manejan los datos, especialmente en contextos de concurrencia o seguridad de datos.

¿Para qué se utilizan las colecciones en Kotlin?

Se utilizan principalmente para:

Gestionar y procesar datos: Por ejemplo, gestionar una lista de elementos, realizar filtrados, ordenar datos, agrupar información, entre otros.

Simplificar operaciones: Usar colecciones de Kotlin junto con sus métodos integrados permite realizar tareas complejas de forma más sencilla y con menos código.

Optimizar el almacenamiento de datos: Por ejemplo, un Set es útil cuando no queremos almacenar duplicados de datos.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/GYc5pqcns)


EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://tuenlace.com/audio.mp4)

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/COLLECTIONS/collections.png)

Escribe una nota del cómo funciona la estructura

// Clase principal que demuestra el uso de las colecciones en Kotlin
class CollectionsDemo {

    // Propiedades: ejemplos de List, Set y Map
    private val listaInmutable = listOf("manzana", "banana", "cereza")
    private val listaMutable = mutableListOf("perro", "gato")
    
    private val conjuntoInmutable = setOf("rojo", "verde", "azul", "rojo") // "rojo" repetido se ignora
    private val conjuntoMutable = mutableSetOf("lunes", "martes")

    private val mapaInmutable = mapOf(1 to "uno", 2 to "dos", 3 to "tres")
    private val mapaMutable = mutableMapOf("A" to 90, "B" to 80)

    // Métodos para mostrar el contenido de las colecciones
    fun mostrarListas() {
        println("🔹 Lista inmutable: $listaInmutable")
        println("🔹 Lista mutable original: $listaMutable")
        listaMutable.add("loro")
        println("🔹 Lista mutable después de agregar 'loro': $listaMutable")
    }

    fun mostrarConjuntos() {
        println("\n🔹 Conjunto inmutable: $conjuntoInmutable")
        println("🔹 Conjunto mutable original: $conjuntoMutable")
        conjuntoMutable.add("miércoles")
        println("🔹 Conjunto mutable después de agregar 'miércoles': $conjuntoMutable")
    }

    fun mostrarMapas() {
        println("\n🔹 Mapa inmutable:")
        for ((clave, valor) in mapaInmutable) {
            println("  Clave: $clave, Valor: $valor")
        }

        println("🔹 Mapa mutable original: $mapaMutable")
        mapaMutable["C"] = 70
        println("🔹 Mapa mutable después de agregar ('C' to 70): $mapaMutable")
    }

    fun recorrerColecciones() {
        println("\n🔹 Recorrido de lista con forEach:")
        listaInmutable.forEach { println("  - $it") }

        println("\n🔹 Recorrido de conjunto con for:")
        for (dia in conjuntoMutable) {
            println("  - $dia")
        }

        println("\n🔹 Recorrido de mapa con entries:")
        for ((k, v) in mapaMutable.entries) {
            println("  [$k] = $v")
        }
    }

    fun mostrarTamaños() {
        println("\n🔹 Tamaños:")
        println("  Lista mutable: ${listaMutable.size}")
        println("  Conjunto mutable: ${conjuntoMutable.size}")
        println("  Mapa mutable: ${mapaMutable.size}")
    }
}

// Clase de ejecución
fun main() {
    val demo = CollectionsDemo()

    println("=== 📚 DEMO DE COLECCIONES EN KOTLIN ===\n")
    demo.mostrarListas()
    demo.mostrarConjuntos()
    demo.mostrarMapas()
    demo.recorrerColecciones()
    demo.mostrarTamaños()
}
