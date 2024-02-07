# Clase-1--Matriz-de-confusi-n
Clasificación números escritos a mano, para lo cual se usan los archivos mnist_train.csv y mnist_test.csv

El objetivo de este ejercicio es clasificar números escritos a mano, para lo cual se usan los archivos mnist_train.csv y mnist_test.csv. Una vez que se tengan las características que interesen hay que crear el modelo, entrenarlo y evaluarlo; para la evaluación lo ideal es usar la matriz de confusión de sklearn, la misma que hay que dibujarla e interpretarla.

DESARROLLO

Se adjunta el documento en formato Jupyter Notebook (.ipynb).

La matriz de confusión que se genera es:
 

Un "Symmetry Indicator" de 0.12 indica que aproximadamente el 12% de las entradas en la matriz de confusión son iguales a sus correspondientes entradas en la matriz transpuesta.

Esto significa que hay una ligera simetría en la matriz de confusión, pero no es muy pronunciada. En otras palabras, algunas clases pueden estar siendo correctamente clasificadas en ambos sentidos (como verdaderos positivos y verdaderos negativos), pero no ocurre con frecuencia en todas las clases.

Existen métricas como:

Exactitud. 

Se utiliza para determinar el rendimiento de la matriz de confusión, es decir, identificar del total de predicciones hechas cuantas fueron predicciones correctas. Este valor va entre 0 y 1 donde 0 significa que no hizo ninguna predicción correcta y 1 que todas las predicciones fueron correctas.
En este caso el valor de exactitud es 0.9450333333333333 lo cual quiere decir que es bastante acertado, sin embargo, no existe un umbral aceptable de exactitud ya que esto puede depender de varios factores como el contexto u objetivos del estudio donde se requiera más o menos exactitud por ejemplo en temas médicos la exactitud debería ser muy alta.

Precisión. 

Class 0: Precision = 0.97
Class 1: Precision = 0.96
Class 2: Precision = 0.93
Class 3: Precision = 0.93
Class 4: Precision = 0.94
Class 5: Precision = 0.94
Class 6: Precision = 0.96
Class 7: Precision = 0.96
Class 8: Precision = 0.93
Class 9: Precision = 0.93

Se refiere a lo cerca del resultado sobre la predicción del valor verdadero, es decir la medida de que tan preciso es nuestro modelo en clasificar las instancias positivas.
Para nuestra matriz tenemos: Clase 0 con una precisión del 0.97 lo que significa que el 97% de las instancias predichas como clase 0 son verdaderos positivos, mientras desde la Clase 1 a la Clase 9 las precisiones varían entre 0.93 y 0.96, indicando que entre el 93% y el 96% de las instancias predichas como cada una de estas clases son verdaderos positivos. En general el modelo tiene un buen rendimiento en términos de precisión, es decir tiene una baja tasa de falso positivos.

Sensibilidad.

Class 0: Sensitivity = 0.97
Class 1: Sensitivity = 0.97
Class 2: Sensitivity = 0.95
Class 3: Sensitivity = 0.92
Class 4: Sensitivity = 0.95
Class 5: Sensitivity = 0.93
Class 6: Sensitivity = 0.97
Class 7: Sensitivity = 0.95
Class 8: Sensitivity = 0.91
Class 9: Sensitivity = 0.92

 Cuanto más alto sea el valor de sensibilidad para una clase, mejor es el rendimiento del clasificador para identificar correctamente las instancias positivas de esa clase. Una sensibilidad del 100% significaría que el clasificador identifica correctamente todas las instancias positivas de esa clase, mientras que una sensibilidad del 0% significaría que no identifica ninguna instancia positiva de esa clase. Desde la Clase 1 – 9 tiene una sensibilidad entre 92% -  97%, lo que significa que identifica correctamente como positivas.

Especificidad.

Class 0: Specificity = 1.00
Class 1: Specificity = 0.99
Class 2: Specificity = 0.99
Class 3: Specificity = 0.99
Class 4: Specificity = 0.99
Class 5: Specificity = 0.99
Class 6: Specificity = 1.00
Class 7: Specificity = 0.99
Class 8: Specificity = 0.99
Class 9: Specificity = 0.99 

Se expresa como un número entre 0 y 1, donde 1 significa una especificidad perfecta y 0 significa una especificidad nula (tasa de verdaderos negativos). Una especificidad más alta indica que el clasificador es mejor para predecir correctamente las muestras negativas para esa clase. Para nuestro modelo la especificidad esta entre 0.99 y 1.00; con estos valores es muy difícil obtener falsos positivos.

