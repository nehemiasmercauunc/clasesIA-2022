# Redes Neuronales - Aprendizaje Supervisado (MLP - Perceptron Multicapa) 6/10/22

## Componentes de un sistema neuronal o conexionista
- Un conjunto de procesadores elementales (neuronas)
- Un patrón de conectividad o arquitectura (dinamica de actualización: media o lenta, no rápida)
- Una dinámica de activaciones (umbral a partir del cual se activa)
- Una regla o dinámica de aprendizaje (potencial post-sinaptico, función de activación y la función que opera sobre la de activación -la de transferencia-). Salvo para algún transfer, la función de transferencia es la función identidad, con lo que la función de activación es la de transferencia.
- El entorno donde opera

## Neurona Artificial
- Dispositivo NO lineal
- Conjunto de entradas
- Pesos sinápticos
- Regla de propagación
- Función de activación
- Función de salida

## Diferencia entre Multicapa y Simple
- Con el simple, esta la capa sensora y la de salida
    - Capa sensora: se representa por señales del entorno (entrada se interpreta como el entorno)
    - Capa de salida: neurona.
- Con el multicapa, hay una capas ocultas, aparte de la sensora y la de salida. 
    - Por lo menos tiene 3 capas.
    - Las capas hidden no se comunican con el exterior:
        - En cada capa se colocan neuronas (ocurre lo del percep. simple)
        - Cada capa recibe de la anterior señales
        - FULL-CONNECTED: todas las neuronas de la capa anterior, se comunican con c/u de las neuronas de la capa siguiente, realizando en cada una el perceptron simple.
    
## Perceptron Multicapa (MLP)
- La capa de entrada se puede representar como: 
    - En un dataset, un ejemplo es una fila, y las neuronas de entrada son las columnas. En fin, toda la fila, representa la capa de entrada.
- La/s capa/s ocultas
- La capa de salida:
    - La señal de salida es el resultado de la red neuronal para esa época.
    - La señal de salida es generar una función de energía para medir el lost (costo, error generalizado), para todos los ejemplos para muchas épocas.
- Las variables a lo largo de la arquitectura de la red, que impactan en la señal de salida, son los pesos sinápticos (todos).
- El target, no es uno, sino que es un vector.
- El número de neuronas por capa, define el vector que se presenta en esa capa.
- Los pesos sinápticos son los que aprenden, evolucionan durantes las épocas.
- Se va a establecer un mecanismo de aprendizaje basado en el descenso por el gradiente, la señal de salida es función de los pesos sinápticos.
- La función de energía debe ser derivable con respecto a los pesos sinápticos (variables).
- La función de energía debe ser para todos los pesos de todas las conexiones de todas las intercapas, hacer la derivadas parciales de todo.
- Para evitar realizas todas las derivadas parciales antes mencionadas, se propone el algoritmo de *BackPropagation*:
    - Se basa en la regla *delta generalizada*
    - Incoporación de momentum: parámetro que permite no caer en mínimos locales y a acelerar el ritmo de aprendizaje
    - Como se conoce el valor esperado de la salida se puede corregir desde la salida hacia atras.
    - Se corrige el error penalizando a los pesos sinápticos de la conexión de la última capa oculta con la capa de salida.
    - Y asi se retrocede en las capas ocultas, penalizando los pesos. 
    - En resumen, toma el único error conocido (el de la salida comparado con lo esperado), y derivando con las capas anteriores, hasta la capa de entrada. 
        - Redistribuye el error cometido en la capa de salida en función de quiene contribuyeron al error desde la capa de entrada.
- Si al MLP en la capa de salida, se representa a la/s neurona/s como una variable continua, puede ser un regresor. Si se representa con varias variables, puede ser un clasificador.
- Capas ocultas: a medida que se aumentan la cantidad de capas ocultas, las capas ocultas de la salida van perdiendo capacidad de aprender con el entrenamiento. Su velocidad es cada vez mas lenta (supresión del gradiente).
- Solución a la Supreción del Gradiente: AUTOENCODER.







//////////////////////////////////////////////////////////////////
(Ver si dejo esto o no)
## Perceptron Multicapa
- Se utiliza TensoFlow con api Keras
- Sirve para (dependiendo la configuración de la neurona): 
    - Regresión 
    - Clasificación

## CNN
- Es un clasificador en imágenes.

## Transfer
- Yolo

//////////////////////////////////////////////////////////////////////