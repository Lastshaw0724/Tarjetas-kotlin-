
 **FUNCIONES DE STRINGS Y PRINTING EN KOTLIN**

 **Cadenas en Kotlin (String)**

En Kotlin, una **cadena** o **String** es una secuencia de caracteres que puedes utilizar para representar texto. Los Strings en Kotlin son **inmutables**, lo que significa que una vez que se crea una cadena, no puedes modificarla directamente. En su lugar, puedes crear nuevas cadenas basadas en operaciones realizadas sobre la original.

 **¿Por qué se usan los Strings?**

Los Strings se utilizan cuando necesitas almacenar y manipular **texto** en tu programa. Esto puede incluir tareas como:

* **Almacenar información textual** como nombres, direcciones, mensajes, etc.
* **Realizar operaciones sobre el texto**, como concatenación, comparación, búsqueda o reemplazo de caracteres o subcadenas.
* **Combinar texto con variables** de forma sencilla usando la **interpolación de cadenas**.

---

 **Características principales de los Strings**

* **Definición**: Las cadenas en Kotlin se definen entre comillas dobles (`""`). Por ejemplo, `"Hola Mundo"` es un String.

* **Inmutabilidad**: Los Strings en Kotlin son inmutables. Si quieres cambiar un carácter o parte de la cadena, deberás crear una nueva cadena.

* **Interpolación de variables**: Puedes insertar valores de variables o expresiones dentro de una cadena usando el símbolo `$`. Esto hace que la manipulación de texto sea mucho más fácil y legible.

---

**Funciones útiles de String**

Kotlin proporciona una amplia variedad de funciones para manipular y trabajar con Strings. Algunas de las más comunes son:

* **`length`**: Devuelve la cantidad de caracteres en el String.

  ```kotlin
  val texto = "Hola"
  println(texto.length)  // Imprime: 4
  ```

* **`uppercase()`**: Convierte la cadena a mayúsculas.

  ```kotlin
  val saludo = "hola"
  println(saludo.uppercase())  // Imprime: HOLA
  ```

**`lowercase()`**: Convierte la cadena a minúsculas.

  ```kotlin
  val saludo = "HOLA"
  println(saludo.lowercase())  // Imprime: hola
  ```
 **`replace()`**: Reemplaza un texto o subcadena por otro dentro de la cadena.

  ```kotlin
  val frase = "Hola Mundo"
  println(frase.replace("Mundo", "Kotlin"))  // Imprime: Hola Kotlin
  ```

 **`substring()`**: Devuelve una subcadena de un String, empezando desde una posición específica.

  ```kotlin
  val mensaje = "Bienvenido"
  println(mensaje.substring(0, 4))  // Imprime: Bien
  ```

 **`contains()`**: Verifica si una cadena contiene otra cadena o carácter.

  ```kotlin
  val frase = "Kotlin es genial"
  println(frase.contains("genial"))  // Imprime: true
  ```



**Función de impresión: `println()` y `print()`**

En Kotlin, puedes mostrar texto en la consola utilizando las funciones `println()` o `print()`:

 **`println()`**: Muestra un mensaje seguido de un salto de línea.

  ```kotlin
  println("Hola Mundo")
  ```

 **`print()`**: Muestra un mensaje sin agregar un salto de línea al final.

  ```kotlin
  print("Hola ")
  print("Mundo")
  // Imprime: Hola Mundo
  ```



**Ejemplo práctico: Uso de Strings e impresión**

Supongamos que queremos crear un programa que salude a un usuario y le diga la longitud de su nombre:

```kotlin
fun main() {
    val nombre = "Carlos"
    
    // Interpolación de cadenas
    println("Hola, $nombre. Tu nombre tiene ${nombre.length} caracteres.")
    
    // Convertir a mayúsculas y mostrarlo
    println("En mayúsculas: ${nombre.uppercase()}")
    
    // Reemplazar una letra y mostrarlo
    println("Reemplazando 'a' por 'o': ${nombre.replace("a", "o")}")
}


Este código imprimirá:

Hola, Carlos. Tu nombre tiene 6 caracteres.
En mayúsculas: CARLOS
Reemplazando 'a' por 'o': Corlos



**Conclusión**

Las cadenas de texto en Kotlin son herramientas poderosas e indispensables para cualquier programa que necesite manejar o mostrar texto. Las funciones de Strings y las herramientas de impresión permiten realizar operaciones complejas de forma sencilla y eficiente.
