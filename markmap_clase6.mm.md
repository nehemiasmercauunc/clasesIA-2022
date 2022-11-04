# Redes Neuronales Artificales - 15/09/22

- Configuración media o lenta: significa que para armar el modelo en base al cual se diseña el algoritmo de inteligencia artificial tiene posibilidades de actualizarse (la config) automaticamente mas lento durante el proceso de aprendizaje.
- Son redes neuronales artificiales. Se inspiran en sistemas que no tienen que ver con computer science, sino emulando el funcionamiento del cerebro humano
- Las neuronas son elementos bobos, que pueden conectarse con otras. Esto permite la inteligencia, la CONEXIÓN de neuronas. 
- Las redes neuronales tienen capacidad de aprender, por ende tienen la capacidad de entrenar, por lo que tienen capacidad de evolucionar, por lo que tienen la capacidad de actualizar sus conexiones. 
- La inteligencia viene dada por los pesos sinápticos (parámetros). 
- La conectividad es una RESTRICCIÓN. 
- Las neuronas, son los elemento necesarios para satisfacer la restricción.
- CAJA NEGRA: Las redes neuronales es siempre un modelo de CAJA NEGRA, porque en su resultado nunca entrega la explicación de su desición de selección.
- Son muy eficientes en proporcionar el resultado, no en explicarlo
- Si es variable continua: redes neuronales que tienen regresión
- Si es variable discreta: redes neuronales que son CLASIFICADORES (no son binarios).
- Aprendizaje: No se programan, se entrenan.
- Autonomía: se refiere a que tenga capacidad de aprender a los largo se su ciclo de vida
- Inteligencia artificial Débil o Fuerte:
    - Débil: el agente autónomo tiene capacidad de seguir aprendiendo frente a los ejemplos que se le presentan.
    - Fuerte: el agente autónomo tiene capacidad para seguir aprendiendo, en su dominio o en otro.
- Arquitectura paralela, distribuida y adaptativa.
    - Paralela: las conexiones trabajan en paralelo
    - Distribuido: el procesamiento es distribuido
    - Adaptativa: la config es adaptativa
- "Degradación Elegante" frente al error. Robustas al ruido en entornos borrosos.
- Generalizan a partir de ejemplos.

## Regresión Lineal
- Es la función de activación para redes neuronales
- La regresión va tras la búsqueda del modelo que explica la solución del problema.
- *Regresión por mínimos cuadrados*
    - *Análisis de la tendencia*: Predecir valores de la variable dependiente -interpolar o extrapolar-
    - *Prueba de hipótesis*: Validad un modelo matemático existente con los resultados experimentales o adecuar el modelo a los datos

### Descenso por el Gradiente
- Se usa para encontrar los parámetros (o inteligencia).
- Se buscan los coeficientes que hacen mínima la expresión de coste. 

## Tipos de aprendizaje automatizado
- Aprendizaje Supervisado
    - Tiene atributo target, realiza el aprendizaje en base al atributo sobre el que se trabaja
- Aprendizaje No Supervisado
    - Significa que no tiene atributo target, todos son input. 
    - El resultado es casi siempre NO EXPLICABLE. Para explicarlo se usa sobre la salida, un aprendizaje supervisado (árboles). Se descubren las reglas que hacen que el target pertenezca a ese grupo.

- Aprendizaje Refuerzo (reinforcement)
    - Pueden existir algoritmos que tengan atributo target. Conocen el atributo target pero no se lo proporciona en el entrenamiento de forma previa. Sino que se lo premia o castiga en base a cuanto se acerque o cuanto se aleje a lo que debería ser.

## Redes Neuronales Artificiales
- Inspiradas en como lo hace el cerebro humano: CONEXIONISTAS
- Su dinámica de actualización de su configuración es media o lenta.
- Aprendizaje: No se programan, se entrenan.
- Hay un algoritmo de entrenamiento y uno de ejecución (este último sirve para el testeo, validación y generalización).
- Arquitectura paralela, distribuida, adaptativa.
- Frente a nuevos ejemplos, todavia se va a probando el algoritmo, sigue entrenando.
- El despliegue total, se adquiere cuando realmente el agente adquiere capacidades para generalizar en el dominio donde se estaba entrenando previamiente, y entrenando luego.
- En ese momento, el agente puede ser autónomo o no (autonomía significa, que tenga la capacidad de seguir aprendiendo a lo largo de su ciclo de vida).
- "Degradación elegante" frente al error. Robustas al ruido en entornos borrosos.
- Generalizan a partir de ejemplos.
