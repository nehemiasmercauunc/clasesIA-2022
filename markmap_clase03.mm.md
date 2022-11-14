# Regresiones y Clasificaciones (18/08/22)

- El modelo que se  llama regresion lineal, es una regresion para machine learning. No se trabaja con regresion lineal univariada. Se trabaja con *multi-variables independientes*.

## Regresiones

- Se le llama a todo proceso cuyo atributo output (target, etiqueta) sea una variable continua. No importa la condicion de la var continua como numero real.

## Clasificaciones

- Tiene como atributo (target o etiqueta), categorias. Se dividen en 2 grupos.

## Modelos aplicables:
- MLP: modelo de redes nueronales, que dio lugar a que los demas continuen. Los primeros fueron Kunihiko Fukushima con Neocognitron, junto con Yann LeCun con CNN.

- MLP y CNN son 2 modelos o arquitecturas de modelos inteligentes, que son *clasificadores*.
- MLP es versatil y puede ser usado para regresiones: osea, la variable output puede ser en MLP y CNN categorica, y en MLP continua.

- Regresion Logistica (clasificación):
    - Es un clasificador porque los resultados van a ser una etiqueta output con categorias. NO va a ser una variable continua.
- Regresion lineal multivariada:
    - Es un modelo de regresion. Output var continua.
 
## Regresion logistica o Función Sigmoide:
- Politomico (target): catogorias( nivel de estudio de la madre: primario completo, incompleto....). Si se excluyen entre ellas, pueden ser convertida en variable dummy.
- Dicotomico (target): binario. Aprobó: si o no.
- Los atributos input, covariables, tienen que ser dicotómicos, y si son politomicos, convertirlos en variables dummy (dicotómicos). NO se deben aplicar variables dummy a variables conjuntivas (procedencia)

## Clasificadores:
- MLP
- CNN
- Regresión Logística
- Support Vector Machine (SVM)
- Árboles de decisión por inducción (TDIDT)

## Métricas - Performance
- Matriz de confusion
    - Arroja información sobre el TARGET
    - Precisión = 
- Regresion logistica binaria
- Target dicotomico, toma 2 valores. (positivo, negativo)
Los hiperParametros son calibradores que van a ir cambiando el modelo para que las metricas sean lo mejor que se puedan.
Las metricas son el resultado.
Los parametros son la inteligencia (importa en redes neuronales)

