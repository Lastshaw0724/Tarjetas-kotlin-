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

Escribe una nota del cómo funciona la estructura

//fun main {

class Persona(
    var nombre: String,
    var edad: Int,
    var altura: Double,
    var esEstudiante: Boolean,
    val pais: String,
    val pi: Float
) {
    fun mostrarDatos() {
        println("Nombre: $nombre")
        println("Edad: $edad años")
        println("Altura: $altura metros")
        println("Es estudiante: $esEstudiante")
        println("País: $pais")
        println("Valor de pi: $pi")
    }
    
    fun actualizarDatos(nuevoNombre: String, nuevaEdad: Int) {
        nombre = nuevoNombre
        edad = nuevaEdad
        println("Nuevo nombre: $nombre")
        println("Nueva edad: $edad años")
    }
}
