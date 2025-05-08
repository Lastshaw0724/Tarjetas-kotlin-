1. Describa el por qué y para qué se utiliza.

¿Por qué y para qué se utiliza la POO en Kotlin?
La Programación Orientada a Objetos (POO) en Kotlin se utiliza para:

✅ Organizar el código en torno a objetos que representan entidades del mundo real.

✅ Encapsular datos y comportamientos en clases, lo que hace el código más fácil de entender, mantener y reutilizar.

✅ Promover la reutilización gracias a la herencia y la composición.

✅ Permitir la abstracción y modularidad, dividiendo programas grandes en componentes más pequeños y manejables.

¿Para qué sirve?

🔧 Modela objetos reales (como coches, personas, cuentas bancarias) en código.

🚀 Permite crear sistemas más robustos, escalables y fáciles de probar.

🛠️ Hace más fácil trabajar en equipo, porque cada parte del código está bien definida.

2. Genere un ejemplo internamente en el recuadro.

[LINK DE CÓDIGO](https://pl.kotl.in/nzXKe3Cyw)

Utilice un editor de código para lograrlo.

EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO

Genere el link del audio y el link de GitHub.

[*LINK DEL AUDIO*](https://tuenlace.com/audio.mp4

[🔗 LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/Lastshaw0724/Tarjetas-kotlin-/blob/main/POO/poo.png)

Escribe una nota del cómo funciona la estructura

fun main(){

//class

class Persona(val nombre: String, var edad: Int) {

    fun saludar() {
    
        println("Hola, soy $nombre y tengo $edad años.")
        
    }
    
}

//objeto

val persona = Persona("Juan", 30)

persona.saludar()  // Salida: Hola, soy Juan y tengo 30 años.

//herencia

open class Animal(val nombre: String) {

    open fun sonido() {
    
        println("El animal hace un sonido")
        
    }
    
}

class Perro(nombre: String) : Animal(nombre) {

    override fun sonido() {
    
        println("El perro ladra")
        
    }
    
}

//interface

interface Volador {

    fun volar()
    
}

class Pajaro : Volador {

    override fun volar() {
    
        println("El pájaro vuela")
        
    }
    
}

//encapsulamiento

class CuentaBancaria(private var saldo: Double) {

    fun deposito(cantidad: Double) {
    
        saldo += cantidad

    }

    fun obtenerSaldo(): Double {
    
        return saldo
    }
    
}

//polimorfismo

open class Vehiculo {

    open fun mover() {
    
        println("El vehículo se mueve")
        
    }
    
}

class Coche : Vehiculo() {

    override fun mover() {
    
        println("El coche está conduciendo")
        
    }
    
}

class Bicicleta : Vehiculo() {

    override fun mover() {
    
        println("La bicicleta está pedaleando")
        
    }
    
}

//constructores

class Usuario(val nombre: String, var edad: Int) {

    constructor(nombre: String) : this(nombre, 0)  // Constructor secundario
    
}

}
