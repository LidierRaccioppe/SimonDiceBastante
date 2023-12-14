# Simon Dice

## Imagenes

![caputura1](./captura.png)

![caputura2](./captura2.png)

![caputura3](./captura3.png)

## Clase DatosSingleton

Los datos que se necesitan para el funcionamiento del juego se guardan en esta clase.

#### Variables

- ronda Int que indica la ronda en la que estamos
- secuencia List<Int> que contiene la secuencia de colores que se van a mostrar
- secuenciaUsuario List<Int> que contiene la secuencia de colores que ha introducido el usuario
- record Int que indica el record del juego
- estado Enum que indica el estado del juego
- tag String que indica la etiqueta a usar para los logs
- colorAux Color que indica el color que se ha pulsado
- numeroDeColores Colores que indica el numero de colores que se van a usar en el juego
- listaColores List<Color> que contiene los colores que se van a usar en el juego

Luego una enum class que tiene los estados del juego.

Son: `INICIO`, `SECUENCIA`, `ENTRADA`, `COMPROBANDO`

Y luego otra enum class que tiene los colores que se van a usar en el juego.

Donde cada uno es un color mutable

## Clase MyViewModel

Esta clase es la que se encarga de la logica del juego.

#### Funcionesclass MyViewModel : ViewModel() {
class MyViewModel : ViewModel() {

    - Genera un número aleatorio entre 0 y el numeroLimiteSuperior
    fun generarNumeroAleatorio(numeroLimiteSuperior: Int): Int {
        - ...
    }

    - Añade un color a la secuencia del usuario
    fun anadirColorSecuenciaUsuario(color: Int) {
        - ...
    }

    - Aumenta la ronda en la que estamos en 1
    fun aumentarRonda() {
        - ...
    }

    - Reinicia la ronda en la que estamos
    fun reiniciarRonda() {
        - ...
    }

    - Añade un color a la secuencia
    fun anadirColorSecuencia(color: Int) {
        - ...
    }

    - Aumenta la secuencia de colores y muestra al usuario la secuencia de colores
    fun aumentarSecuenciaMaquina() {
        - ...
    }

    - Aumentar la secuencia de colores del usuario
    fun aumentarSecuenciaUsuario(color: Int) {
        - ...
    }

    - Obtiene el último elemento de la secuencia del usuario
    fun getUltimoElementoSecuenciaUsuario(): Int {
        - ...
    }

    - Comprueba si la secuencia del usuario es correcta
    fun comprobarSecuenciaUsuario(): Boolean {
        - ...
    }

    - Muestra la secuencia de colores del usuario
    fun getSecuenciaUsuario(): MutableList<Int> {
        - ...
    }

    - Getter de la secuencia de colores
    fun getSecuenciaColores(): MutableList<Int> {
        - ...
    }

    - Getter de la secuencia de colores del usuario
    fun getSecuenciaColoresUsuario(): MutableList<Int> {
        - ...
    }

    - Muestra la secuencia de colores y hace un log.d de la secuencia
    fun getSecuenciaMaquina(): MutableList<Int> {
        - ...
    }

    - Muestra la secuencia de colores del usuario y hace un log.d de la secuencia
    fun mostrarSecuenciaUsuario(): MutableList<Int> {
        - ...
    }

    - Reinicia la secuencia
    fun reiniciarSecuencia() {
        - ...
    }

    - Reinicia la secuencia del usuario
    fun reiniciarSecuenciaUsuario() {
        - ...
    }

    - Reinicia el estado del juego
    fun reiniciarEstado() {
        - ...
    }

    - Reinicia el record del juego
    fun reiniciarRecord() {
        - ...
    }

    - Obtiene el último elemento de la secuencia de la máquina
    fun getUltimoElementoSecuenciaMaquina(): Int {
        - ...
    }

    - Reinicia el juego
    fun reiniciarJuego() {
        - ...
    }

    - Comprueba si el record se ha superado
    fun comprobarRecord(): Boolean {
        - ...
    }

    - Actualiza el record
    fun actualizarRecord() {
        - ...
    }

    - Devuelve la ronda actual
    fun getRonda(): Int {
        - ...
    }

    - Comprueba si la secuencia del usuario es correcta
    fun comprobarSecuencia(): Boolean {
        - ...
    }

    - Oscurece el color
    fun tintinearOscurecimiento(color: Color, factor: Float): Color {
        - ...
    }

    - Muestra la secuencia de colores de la máquina con un retraso entre colores
    fun mostrarSecuenciaMaquina(time: Long) {
        - ...
    }

    - Muestra la secuencia de colores de la máquina y ejecuta la función en un hilo bloqueante
    fun mostrarSecuenciaMaquinaEjecutar(time: Long) = runBlocking {
        - ...
    }

    - Tintinea el color de un usuario para resaltar la selección
    fun tintineaUsuarioBlancoMostrar(numColor: Int) = runBlocking {
        - ...
    }

    - Tintinea el color de un usuario para resaltar la selección
    fun tintineaUsuarioBlanco(color: Int) {
        - ...
    }

    - Obtiene el estado del juego
    fun getEstado(): Estado {
        - ...
    }

    - Establece el estado del juego
    fun setEstado(estado: Estado) {
        - ...
    }
}





