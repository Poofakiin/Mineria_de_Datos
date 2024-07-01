# Curso de Minería de Datos

Este repositorio contiene el material relacionado con el curso de Minería de Datos de la Universidad de Chile. El repositorio está organizado en dos secciones: los laboratorios del curso y el proyecto del curso.

## Contenido

### Laboratorios del Curso
Esta sección incluye todos los laboratorios asignados durante el curso. Los laboratorios tienen un carácter tanto formativo como evaluativo, y están diseñados para ayudar a los estudiantes a comprender y aplicar los conceptos y técnicas de la minería de datos.

### Proyecto del Curso
**Descripción:**  
El proyecto del curso es un proyecto de clasificación de género de canciones basado en dos enfoques:

1. **Clasificación por Características de la Canción:**  
   Utilizando características como valencia, duración, entre otras, se busca desarrollar un modelo que pueda predecir el género de una canción.

2. **Clasificación por Letras de las Canciones:**  
   En este enfoque, se utilizarán las letras de las canciones para desarrollar un modelo que clasifique el género musical.

## Estructura del Repositorio

- `laboratorios/`: Código y documentos relacionados con los laboratorios del curso.
- `proyecto/`: Código y documentos relacionados con el proyecto del curso.
- `README.md`: Este archivo.

## Proyecto de Clasificación y Análisis de Canciones
Introducción

La música es una forma esencial de expresión humana que ha evolucionado significativamente en su distribución, especialmente con el crecimiento de los servicios de streaming. Este proyecto se centra en el análisis y clasificación de canciones disponibles en Spotify, abarcando un periodo de setenta años (1950-2019). La clasificación de las canciones según su género musical es de particular interés, ya que puede mejorar los algoritmos de recomendación utilizados en diversas aplicaciones, como la generación automática de listas de reproducción, la detección de canciones y la selección de bandas sonoras.
Conjunto de Datos

El conjunto de datos utilizado en este proyecto está disponible en Kaggle y contiene 28,372 canciones. Cada canción incluye atributos técnicos y emocionales:

    Atributos técnicos (numéricos): 'danceability' (bailabilidad), 'loudness' (volumen), 'acousticness' (acústica), 'instrumentalness' (instrumentalidad), 'valence' (valencia), 'energy' (energía).
    Atributo emocional (texto): 'lyrics' (letra).
    Otras variables: 'genre' (género), 'track_name' (nombre), 'release_date' (año), entre otras.

El conjunto de datos está limpio y no contiene valores nulos.
Análisis de Género

El género musical es la principal variable a analizar. Se busca evaluar si las canciones se pueden clasificar correctamente según su género utilizando tanto aspectos técnicos (sonido) como emocionales (letras).
Propuestas Experimentales
Clasificación Basada en Aspectos Técnicos

    Balanceo de datos: Aplicar técnicas de subsampling u oversampling para equilibrar las clases de géneros.
    Modelado: Generar modelos de clasificación con SVC, Decision Tree y KNN, utilizando un modelo de entrenamiento 25/75. Aplicar GridSearchCV para encontrar los hiperparámetros óptimos.
    Evaluación: Evaluar los modelos usando precision, recall y f1-score.
    Comparación: Comparar el desempeño de los modelos para determinar si el mejor modelo clasifica correctamente las canciones basándose en sus aspectos técnicos.

Clasificación Basada en Letras de Canciones

    Conversión de letras: Convertir las letras en datos numéricos.
    Balanceo de datos: Aplicar técnicas de balanceo.
    Modelado: Generar modelos de clasificación con Decision Tree, KNN y SVC, utilizando un modelo de entrenamiento 25/75.
    Evaluación: Evaluar los modelos usando precision, recall y f1-score.
    Comparación: Comparar el desempeño de los modelos para determinar si el mejor modelo clasifica correctamente las canciones basándose en sus letras.

Clustering

    Modelado de clustering: Generar modelos de clustering con K-Means, DBSCAN y clustering aglomerativo, utilizando 7 clusters (correspondientes a los géneros).
    Representación visual: Graficar la representación PCA de los datos originales y comparar con la distribución PCA de los clusters.
    Evaluación externa: Evaluar los modelos de clustering usando la etiqueta de género conocida.
    Comparación: Comparar el desempeño de los modelos para determinar si predicen correctamente el género de las canciones.

Conclusiones

El proyecto busca identificar el método más eficaz para clasificar canciones según su género, utilizando tanto aspectos técnicos como emocionales. Los resultados obtenidos pueden contribuir al desarrollo de algoritmos de recomendación más precisos y personalizados.
