# Deep Learning - MNIST y predicción de números escritos a mano
## Julio Antonio Fresneda García
# Resumen:
**Vamos a intentar entrenar una red neuronal completa para el dataset MNIST, el cual se obtiene a través de la propia librería de Tensorflow y Keras. Buscaremos también el learning rate óptimo, e intentar superar el 98% de precisión.**
#### Condiciones adicionales
Para distinguir este ejercicio de otros ya resueltos en internet, añadiremos, además, algunas condiciones adicionales en este ejercicio:

   * Utilizar 3 y 4 capas ocultas
   * Por cada modelo, crear dos versiones con distinto número de neuronas en las capas ocultas
   * Para la mejor red neuronal de 3 capas y la mejor red neuronal de 4 capas, crear dos versiones alternativas con distinto learning rate.
   * Los comentarios tendrán especial peso en esta práctica.
  
# Planteamiento del ejercicio
Este ejercicio es un clásico a la hora de practicar con algoritmos de clasificación. El dataset MNIST representa miles de números del 0 al 9 escritos a mano alzada, los cuales nuestros modelos deberán clasificar correctamente. 
En este caso, usaremos redes neuronales profundas (DNN), en las cuales hay una capa de neuronas de input, otra de output, y entre ellas algunas capas ocultas. Al ser completas, cada una de las neuronas de una capa está conectada con todas las neuronas de la siguiente capa.

Si bien este ejercicio es a priori sencillo, tenemos muchas formas de "complicarlo", o hacerlo más interesante, por ejemplo, probando con distintos hiperparámetros.

Para esquematizar este trabajo, vamos a dividirlo en los siguientes puntos, los cuales se desarrollarán en profundidad a lo largo del notebook:

   * Carga, transformaciones y exploración del dataset
   * Hiperparámetros: Cuáles combinamos, cuáles cambiamos y cuáles dejamos por defecto
   * Declaración de funciones auxiliares
   * Entrenamiento de distintos modelos, comparativas y resultados
   * Conclusiones
