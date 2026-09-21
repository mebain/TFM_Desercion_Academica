# Predicción del riesgo de deserción académica en estudiantes universitarios a través de modelos de  aprendizaje supervisado

Este repositorio contiene el desarrollo inicial del Trabajo Final de Máster orientado a la predicción del riesgo de deserción académica en estudiantes universitarios mediante 
técnicas de aprendizaje supervisado.

El trabajo busca identificar qué características presentan mayor relevancia predictiva en relación con el riesgo de deserción y analizar posibles diferencias entre áreas disciplinares.

## Dataset
Se utiliza el conjunto de datos **Predict Students' Dropout and Academic Success**, disponible en el UCI Machine Learning Repository.

El dataset contiene información académica, demográfica y socioeconómica de estudiantes de una institución portuguesa de educación superior.

La variable objetivo original tiene 3 valores posibles

- 'Graduate'
- 'Dropout'
- 'Enrolled'

Para el modelado predictivo se consideran los casos correspondientes a 'Graduate' y 'Dropout, asignando: 

- 0 = Graduate
- 1 = Dropout

Fuente: https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success

## Metodología

El desarrollo se organiza siguiendo las  etapas de CRISP-DM:

- Comprensión del problema de intervención.
- Comprensión de los datos.
- Preparación de los datos.
- Modelado.
- Evaluación.

Durante la preparación de los datos se realizan transformaciones y agrupaciones de variables categóricas, codificación mediante One-Hot Encoding y estandarización de las variables 
numéricas cuando el algoritmo lo requiere.

## Modelos utilizados

Se entrenan y comparan tres modelos de clasificación supervisada:

- Regresión Logística.
- Random Forest.
- Support Vector Machine (SVM).

Los modelos son evaluados mediante Accuracy, Precision, Recall y F1-score. También se utiliza validación cruzada para analizar la estabilidad de los resultados.

## Análisis de variables

Para explorar la relevancia predictiva de las características se analizan:

- los coeficientes de la Regresión Logística;
- las importancias de variables del modelo Random Forest.

Los primeros resultados muestran una presencia destacada de variables vinculadas con el desempeño académico y con la situación económico-financiera del estudiante.

## Archivos

- `TFM_Bain_12-sep.ipynb`: notebook principal con el desarrollo del análisis.

## Estado del trabajo

Trabajo en desarrollo.
