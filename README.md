# AHORCADO - PROYECTO No. 1 
#### Integrantes .-
##### Betancourt Sergio
##### Chuquimarca William
##### Granda Cristina
##### Pacheco Jael

------------------------------------------------------------------------------------------------------

Este programa se desarrolla principalmente con un **SWITCH** con la finalidad de diferenciar entre dos posibles situaciones, donde el primer caso se desarrollará si y solo si existe un único jugador y el segundo en el cual existen dos. <br>

###### Case 1
En el caso para un jugador se utiliza un **while principal** con la finalidad de que este bucle se repita una y otra vez mientras nuestra variable booleana **seguirjugando** sea verdadera. <br>
Como se había establecido este caso para un único jugador se utilizó el **random** para escoger del vector anteriormente establecido una palabra aleatoria, la cual después será leída por length y la conformará con "_" <br>
Dentro del **while principal** se utiliza otro **while** que funcionará únicamente cuando los intentos sean mayores que cero y que la palabra establecida sea diferente a la que el jugador ingresa. En este bucle se define datos de salida como entrada. El único valor de entrada denominada **entrada** es filtrada por un for el cual la convertirá en mayúsculas. <br>
Se hace uso de otra variable booleana **entradaValida** para evaluar a la palabra o letra a través de un **for**, y si se haya un caracter especial o número se muestra un mensaje de error. <br>
Si la palabra ingresada es igual a la palabra aleatoria se utiliza **break** para detener el programa, miestras que cuando el jugador no adivina la palabra le sale un mensaje que le informa su derrota, pasa por una muerte instantanea y el dibujo se lo realiza en su totalidad para terminar con un **break**. <br>
El programa acepta tanto palabras como letras en el momento en que pide ingresar el dato, por lo que si ingresa una letra no ingresa al bucle en el que compara con la palabra total, sino ingresa a un **for** en el cual compara cada una de las letras con la ingresada para verificar si existe alguna coincidencia. Si no halla ninguna coincindecia pierde una vida, la cual será notificada mediante un cout. <br>
Si la palabra ingresada por el usuario es igual a la palabra que el programa escogió aleatoriamente se ingresa en un **if** el cual mostrará un mensaje de felicitaciones y le asignará un puntaje que puede aumentar con futuras rondas. <br>
A través de un if se examina la opción de volver a jugar. Si la respuesta es **Y** vuelve a ingresar en el código anteriormente explicado, mientras que si la respuesta es **N** muestran los créditos del juego. <br>

###### Case 2
En este caso se desarrolla el código para dos jugadores. Este código inicia con un **while** en el cual se pedirá que ingrese el número de rondas que desean jugar, sin embargo se debe evaluar que este número sea par y no contengan decimales, el cual será evaluado por un **for** y un **if**. <br>
Se pide ingresar una palabra la cual será filtrada por un **for** y un **if** para determinar si la "palabra" ingresada no tiene caracteres numéricos. Además se implementó un **else if** para convertir toda la palabra con letras mayúsculas. Una vez evaluadas todas las concideraciones se procede a borrar todo el rastro de la palabra, con el objetivo de que el jugador No. 2 no la pueda observar y continua con la misma lógica que en el caso 1, ya que la palabra será leída por length y la conformará con "_" <br>
Sigue manteniendo las mismas opciones de continuar con el juego, el puntaje, la muerte instantanea entre otros. Esta parte del código fue reutilizada del caso 1.

###### CTurtle
En este proyecto se utiliza la librería `CTurtle.hpp` con la finalidad de incorporar una representación gráfica al juego del ahorcado. Esta librería permite trabajar con una “tortuga” gráfica, la cual puede moverse dentro de una ventana y dibujar líneas según las instrucciones establecidas en el código. <br>
Dentro de la función `main()` se configura inicialmente la parte gráfica del programa. Para ello, se crea una pantalla mediante el objeto `TurtleScreen`, se define un color de fondo oscuro y se crea el objeto `Turtle`, que será el encargado de realizar los trazos del dibujo. Posteriormente, se utiliza la instrucción `hideturtle()` para ocultar la tortuga, de manera que durante la ejecución solo se observe el dibujo del ahorcado y no el cursor que realiza los movimientos. <br>
La parte principal del uso de CTurtle se encuentra en la función `dibujarAhorcado()`. Esta función recibe como parámetros la tortuga y el número de intentos restantes del jugador. Dentro de esta función se configuran algunas características del dibujo, como el color del lápiz, el grosor de la línea y la velocidad. En este caso, se usa un color blanco para que el dibujo resalte sobre el fondo oscuro, se establece un grosor de línea adecuado y se configura una velocidad rápida para que el dibujo aparezca de forma inmediata. <br>
Para construir la figura del ahorcado, se utilizan instrucciones propias de CTurtle como `penup()`, `pendown()` y `goTo()`. La instrucción `penup()` permite mover la tortuga sin dibujar, mientras que `pendown()` vuelve a activar el dibujo. Por su parte, `goTo()` permite trasladar la tortuga hacia coordenadas específicas dentro de la pantalla. Con estas instrucciones se dibuja primero la estructura principal del ahorcado, compuesta por la base, el poste vertical, la parte superior y la cuerda. Esta estructura aparece desde el inicio de cada partida, ya que representa el soporte del juego. <br>
Después de dibujar la base, el programa utiliza condicionales `if` para dibujar progresivamente las partes del cuerpo del ahorcado según la cantidad de intentos restantes. Cuando el jugador comete errores, los intentos disminuyen y se van mostrando nuevas partes del cuerpo. Si quedan cinco intentos, se dibuja la cabeza; si quedan cuatro, se dibuja el torso; si quedan tres, se dibuja un brazo; si quedan dos, se dibuja el otro brazo; si queda un intento, se dibuja una pierna; y cuando los intentos llegan a cero, se dibuja la última pierna, completando así la figura del ahorcado. <br>
Además, al iniciar una nueva partida se utiliza la instrucción `t.reset()`, la cual reinicia el dibujo anterior y limpia la pantalla gráfica. Esto permite que cada ronda comience desde cero, evitando que se mezclen los dibujos de partidas anteriores.

###### Conclusión 
Al finalizar este proyecto se concluye que al integrar la lógica tradicional del juego del ahorcado con elementos propios del lenguaje de programación C++ se reforzó el conocimiento previamente adquirido como los bucles, condicionales, funciones y gráficos básicos.
El resultado final es un programa interactivo que permite jugar de manera individual o entre dos participantes, controlando intentos, puntajes y errores de entrada. Por lo tanto, consideramos que este proyecto nos ayudó a comprender mejor cómo transformar una idea de juego en un programa funcional.







