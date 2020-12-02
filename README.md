# Tema5
Curso: Modelos Probabilisticos de Señales y Sistemas 
Laboratorio 5
Nombre: Josué Bonilla Marenco
Carné: B71200

Este laboratorio es un complemento del tema de Cadenas de Markov. 
El laboratorio brinda un ejemplo con su respectivo código para un sistema M/M/1 donde se simula un servidor. 
Como asignación se pide determinar el valor de "nu" para que el sistema no se encuentre vacío por más de un 10 % del tiempo. 
El código del ejemplo se ha modificado en una celda de código abajo de la asignación para realizar el desarrollo del laboratorio.
Para que se tenga una cantidad considerable de personas en la cola del servidor se elige un parametro P = 3 y lam permanece igual, lam = 2.
Con estos parámetros se obtiene la relación: v^3 = lam^3 / 0.1, considerando que se busca que el servidor no esté vacío por mas de un 10 % del tiempo.
El valor de "nu" calculado es nu = 4.30
Estos parámetros se cambiaron en el código y posterioremente se modificó algunos bucles que contiene el código para determinar si en la simulación se cumple con los requerimientos.
Los cambios realizados estan comentados en el código pero en resumen se ha cambiando  el bucle de recorrido del vector temporal y conteo de clientes (estado n) en el cual se invirtió el sentido de la comparacion de Xt[i] con P porque en el caso anterior se queria que el servidor tuviese 4 o menos personas durante un determinado tiempo mientras que en este caso una o mas personas durante un 90% del tiempo, por esto mismo se cambió la comparación que determina si en la simulación se cumple con los requerimientos por una condición en la que el servidor permanece un 90% del tiempo o mas con al menos una solicitud. 
Los resultados muestran que para el valor de "nu" determinado se tiene almenos una soliditud un 96 % del tiempo de la simulación, con lo cual se comprueba el cumplimiento de las especificaciones. 
