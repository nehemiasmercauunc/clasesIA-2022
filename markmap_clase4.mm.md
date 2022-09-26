# Data Mining - KDD (1/9/22) - Machine Learning
## Características
- Descubrimiento automatizado de patrones desconocidos
- Predicción automatizada de tendencia y comportamientos
- KDD: Knowledge Discovery in Databases (Descrubrimiento de Conocimiento en Base de Datos)

### Diferencias con otros metodos
 - En general la gran diferencia al aplicar un modelo de ML en KDD, se esta buscando una asociación entre las caracteristicas (atributos input), que determinan el atributo target. 
- Regresion Logistica
- Regresion Lineal
- SVM

## Árboles de desición
- Para cada nodo interno, hay 2 ramas
- Altura del árbol: longitud del camino mas largo desde la raíz a una hoja
- Entropía y ganancia de información

- La cantidad de estados viene dado por la cantidad de nodos posibles, osea la cantidad de características posibles (candidatos)

- Cantidad de nodos son la cantidad de atributos que participan para describir.


### Aprendizaje Supervisado
#### Como aprenden?
- En el entrenamiento entra un ejemplo que ayuda a elegir cual es el nodo candidato
- Las filas son las que contribuyen a la eleccion del nodo candidato dentro de todas las columnas candidatas.
- En cada época del entrenamiento, el algoritmo inteligente decide cual es el "nodo" (caracteristica) de mayor ganancia de informacion (minima entropía)
- Evoluciona hasta que la entropía alcance la tolerancia fijada (Hiperparámetro)
- Nunca todos los ejemplos quedan completamente representados, la complejidad del problema lo imposibilita
- Para cada época, todos los atributos son candidatos, aunque hayan sido elegidos anteriormente
#### Atributos, tipo
- Los atributos input pueden ser continuos o discretos
- Los atributos target pueden ser categóricos. Dicotómicos o Politómicos.
#### Hojas y Reglas
- Hoja: expresa una categoría del atributo target
- Traza expresa una regla: expresión conjuntiva
- Pueden existir mas de una regla para cada categoría del atributo target
### Modelos TDIDT - Interpretaciones
-  Que sea posible comprender sus resultados a través de una expresión conjuntiva implica que el modelo sea explicable. Sin embargo, el algoritmo inteligente usa, por ejemplo, criterios de entropía para decidir (subsimbolico)
- Mientras mas profundidad (hiperparametro) tenga el arbol, mas denso y exacto resultará (sobreajuste). Un arbol completo (inasible) es aquel en el que todos sus ejemplos estan representados.
- Es necesario encontrar el justo equilibrio entre interpretabilidad y densidad (complejidad) del modelo
- Todos los ejemplos terminan asignándose a alguna de sus hojas, sólo que no quedan completamente repsentados en ellas
### Contenidos TDIDT
- Clasificación
- Regresión  
- Multi-output problems
- CART (Classification and Regression Trees)

#### Modelos TDIDT: CART
- DecisionTreeClassifier: modelos:
    - gini
    - entropy
    - log_loss
- Regression criteria: modelos:
     - Error medio cuadrático
     - Poisson
#### Modelos Random Forest
- Son técnicas de regularización
- Hacen un baggin: distribuyen los ejemplos en distintas "bolsas". 
- Con cada 'bolsa' realizan árboles de desición y con la sumatoria de todos, generan una salida
- Se vota, no se promedia. Esto genera la clase final (ganadora)

