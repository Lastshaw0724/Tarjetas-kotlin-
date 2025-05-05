**ARRAYS EN KOTLIN**

 **¿Qué son los arrays?**

Un **array** es una estructura de datos que permite **almacenar múltiples valores del mismo tipo** (por ejemplo, solo enteros, solo cadenas, etc.) en una sola variable. Es decir, en lugar de crear variables individuales para cada valor, puedes guardar todos esos datos dentro de un mismo array, organizados por posiciones llamadas **índices**.

Cada valor en un array está asociado a una posición numérica, que comienza en **0**. Esto significa que el primer elemento está en la posición `0`, el segundo en la `1`, y así sucesivamente.


 **¿Para qué se utilizan los arrays?**

Los arrays se utilizan cuando:

* Necesitas manejar **varios datos del mismo tipo juntos**, como nombres de estudiantes, calificaciones, o estados de conexión.
* Requieres **acceder rápidamente** a ciertos elementos mediante su **índice**.
* Quieres **modificar elementos** directamente sin recorrer toda la colección.
* El número de elementos es **conocido y fijo** (para colecciones variables, se usa `List` o `MutableList`).

Por ejemplo, en una aplicación escolar, podrías usar un array para almacenar los nombres de los estudiantes de un curso.



 **Cómo se declaran los arrays en Kotlin**

Kotlin proporciona una forma sencilla de declarar arrays mediante la función `arrayOf()`:

kotlin
val numeros: Array<Int> = arrayOf(1, 2, 3, 4, 5)       // Array de enteros
val nombres: Array<String> = arrayOf("Ana", "Luis", "Pedro")  // Array de cadenas
val estados: Array<Boolean> = arrayOf(true, false, true)      // Array de valores booleanos


Cada array es un **objeto en sí mismo**, con propiedades y funciones útiles como `size`, `get()`, `set()`, etc.



 **Operaciones comunes con arrays**

Una vez que tienes un array, puedes hacer varias operaciones con él:

kotlin
// Acceder a un valor por índice
println(nombres[0])  // Resultado: Ana

// Cambiar el valor de un elemento
nombres[1] = "Lucía"
println(nombres[1])  // Resultado: Lucía

// Obtener el número total de elementos
println(nombres.size)  // Resultado: 3




**Ejemplo práctico**

Supongamos que estás desarrollando una app escolar que maneja los nombres de estudiantes. Este código muestra cómo usar un array para ese propósito:

kotlin
fun main() {
    val estudiantes = arrayOf("Carlos", "María", "Andrés")
    
    println("Primer estudiante: ${estudiantes[0]}")
    
    estudiantes[1] = "Marta"
    println("Nombre actualizado: ${estudiantes[1]}")
    
    println("Total de estudiantes: ${estudiantes.size}")
}


**Este código imprime:**


Primer estudiante: Carlos
Nombre actualizado: Marta
Total de estudiantes: 3



**Conclusión**

Los arrays en Kotlin son fundamentales cuando necesitas agrupar y manipular datos homogéneos de forma eficiente. Son ideales en situaciones donde los datos no cambian de tamaño y necesitas acceso rápido a elementos por su posición.


