# Regresión Lineal a Descenso por el Gradiente en IA (11/08/22)

- En el ajuste polinómico con polinomios de grado alto (mayor a 5) son altamente inestables
- En estadística casi siempre importa, la bondad de ajuste.
- En IA se desprecia la bondad de ajuste, porque el overfiting produce consecuencias negativas para los objetivos de generalizar, y descubrir patrones para predecir.
- En el ajuste por regresión se define a priori un modelo matemático. 
- En Metodos numericos, era un único atributo independiente (eje x) y una única variable target (eje y)
- La regresión es la función de activación del aprendizaje automático
- Es una parte del algoritmo de aprendizaje automático 


## Regresión Lineal Univariada

- Basada en una nube de puntos, es prácticamente imposible que todos los puntos se ajusten a una recta.
- En la regresión se calculaban los errores del valor real con su predicción (que es el punto sobre la recta), este error se llama dispersión. 
A la dispersión se la eleva al cuadrado, se realiza una sumatoria y después se busca el mínimo de esa sumatoria. 
Esto representa una función de 2do grado, que es la sumatoria cuadrática de las dispersiones o una expresión de una varianza. 
    - Para buscar el mínimo, se deriva esa expresión y se iguala a cero, buscando las ecuaciones normales (sist de ecuaciones algebráicas lineales). 
    - Esto se realiza para buscar de todas las rectas posibles, cuál es la que mejor ajusta (la que tiene el menor error)
    - La recta que mejor ajusta, es aquella que tiene el costo MÍNIMO.  
    - Esto es REGRESIÓN POR MÍNIMOS CUADRADOS
    - Los coeficientes son los parámetros inteligentes.

## Descenso por el Gradiente

- Es un proceso ITERATIVO.
- Se tienen hipótesis, para cada hipótesis, se tiene un valor (theta0 y theta1).
- Para una hipótesis dada, se tienen parámetros (theta0 y theta1)
- Se propone una función de coste (en función de los parámetros)
- Objetivo: minimizar la función de coste, mediante iteraciones.

## Regresión Lineal Múltiple

- La diferencia con la Regresión Lineal Simple, es que tiene más de una variable independiente.
- Se espera que se obtenga siempre la recta que mejor ajusta.
- Mide cuánto mejor ajusta la regresión lineal respecto de la peor representación que se puede hacer de cualquier modelo, que es la función constante.

