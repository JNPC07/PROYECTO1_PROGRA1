# AHORCADO - PROYECTO No. 1 
#### Integrantes .-
##### Betancourt Sergio
##### Chuquimarca William
##### Granda Cristina
##### Pacheco Jael

------------------------------------------------------------------------------------------------------

Este programa se desarrolla principalmente con un **SWITCH** con la finalidad de diferenciar entre dos posibles situaciones, donde el primer caso se desarrollará si y solo si existe un único jugador y el segundo en el cual existen dos. <br>

###### Case 1
Se utiliza un **while principal** con la finalidad de que este bucle se repita una y otra vez mientras nuestra variable booleana **seguirjugando** sea verdadera. <br>
Como se había establecido este caso para un único jugador se utilizó el **random** para escoger del vector anteriormente establecido una palabra aleatoria, la cual después será leída por length y la conformará con "_" <br>
Dentro del **while principal** se utiliza otro **while** que funcionará únicamente cuando los intentos sean mayores que cero y que la palabra establecida sea diferente a la que el jugador ingresa. En este bucle se define datos de salida como entrada. El único valor de entrada denominada **entrada** es filtrada por un for el cual la convertirá en mayúsculas. <br>
Se hace uso de otra variable booleana **entradaValida** para evaluar a la palabra o letra a través de un **for**, y si se haya un caracter especial o número se muestra un mensaje de error. <br>
Si la palabra ingresada es igual a la palabra aleatoria se utiliza **break** para detener el programa, miestras que cuando el jugador no adivina la palabra le sale un mensaje que le informa su derrota, pasa por una muerte instantanea y el dibujo se lo realiza en su totalidad para terminar con un **break**. 




