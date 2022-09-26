# CRISP-DM - Modelo o metodología de Minería de Datos (8/9/22)
## Características
- Cross Industry Standard Process for Data Mining
- Modelo estándar abierto del proceso que describe los enfoques comunes que utilizan los expertos en minería de datos. 
- Es el modelo analítico más usado.
## Reglas de Comportamiento:
### Modelo de Machine Learning: TOP DOWN INDUCTION DECISION TREE (TDIDT)
- *ID3*
- *C 4.5*
- *C 5.0*
- *CART*
- *RANDOM FOREST*: 
        - Es una mejora del algoritmo TDIDT, porque tiene incorporada técnicas de regularización.
        - Tiene el metodo de buscar los atributos mas importantes
        - Son los que intervinieron en la desición de las particiones en los nodos interiores.
        - NO ES UNA RELACIÓN CAUSAL.
### Proceso: Descubrimiento de Grupos (Clustering)
- Clustering: asociar a los elementos en función de su similitudes.
- Cuando se alimenta al algoritmo, se lo alimenta con una métrica que el analista considera válida. 
El algoritmo toma las métricas como distancias geométricas y las trata de forma igualitaria. CUIDADO CON LAS INTERPRETACIONES DE LOS DATOS.
- SOM: algoritmo de Redes neuronales
- No tienen atributos target, no tienen etiquetas. No clasifican. Todos son atributos inputs.
- El algoritmo agrupa los datos según las asociaciones y similitudes que encuentra, una vez convertidos los atributos en geometría.
- Todos son variables continuas

### Proceso: Descubrimiento de Atributos Significativos o Interdependencia

- Modelo de Machine Learning: Redes Bayesianas

### Proceso: Descubrimiento de Reglas de Pertenencia a los Grupos
- Es una combinaciones de los procesos anteriores
- Se descubren las etiquetas que indican a que cluster pertenece cada ejemplo
- Esa etiqueta, se toma como atributo *target* de los algoritmos TDIDT

## Mapas AutoOrganizados o Clustering
### K-MEANS (Algoritmo)
- Permite calibrar rápidamente, cuál es el número de cluster óptimo para el dataset a tratar
- Tiene incorporado, la curva ELBOW: mide en función del número de clusters, la inercia.
- Mientras las masas esten mas cercanas, la inercia es menor. Esto tiene que ver con la similitud de los datos respecto a los atributos.
- La cantidad de clusters a elegir, tiene que ver con la curva ELBOW.
- Cada cluster, tiene un centroide.

### HAC (Algoritmo jerárquico)
- Jerarquía entre los distintos niveles, determinando la cantidad de clusters por agrupación en cada nivel.
- 2 Tipos de agrupaciones:
        - Aglomerativa: De abajo hacia arriba. 
        - Divisiva: De arriba hacia abajo
- En el nivel mas bajo la similitud es 100% y en el nivel mas alto, la similitud es 0%.
- Aglomerativa: Un conjunto de clusters anidados, organizados como un árbol jerárquico, con único cluster arriba, agrupando todos los individuos y clusters con un solo elemeto abajo.
- El algoritmo es comparativamente mas lento y no escala bien apra grandes conjuntos de datos
- El algoritmo HAC es sensible a valores atípicos


### SOM - KOHONEN
- Capas de red, conectadas con sinapsis (pesos sinaṕticos)
- Aprendizaje NO supervisado. 
- Aprende a agrupar los ejemplos según las similitudes que descubre entre ellos.
- No usa descenso por el gradiente

## K-MEANS - CLUSTERING
- Obtendremos Centroides y Conjuntos o agreupamientos de los ejemplos a los que se enfrente el algoritmo
- Al finalizar, el algoritmo ha etiquetado automáticamente los datos asignándoles una partición o cluster