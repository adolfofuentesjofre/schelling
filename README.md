# Clasificación y Regresión con Tensorflow

El artículo “Dynamic Model of Segregation” de Schelling ha sido citado más de 6500 veces de acuerdo con Google Scholar y representa una obra seminal en el campo de teoría de juegos, modelos basados en agentes y simulación del comportamiento humano. Como consecuencia una gran cantidad de disciplinas desde la economía hasta las ciencias sociales computacionales se han referido a este artículo. 


<a name="introducción"></a>
## 1. Introducción

Existen sistemas donde emergen resultados colectivos a partir de mecanismos individuales. En algunos casos incluso cuando las preferencias individuales son débiles o cuando existen incentivos casi imperceptibles, estos, pueden conducir a fenómenos globales completamente distintos y resultados altamente polarizados que emergen a partir de una red de micro interacciones individuales. 
Ese es precisamente el argumento central de Schelling abordado por la pregunta de investigación: ¿Cómo puede emerger la segregación a partir de la interacción de las preferencias individuales? Esta pregunta es relevante debido a que aborda el problema fundamental de como funcionan las sociedades.  

<a name="bibliotecas"></a>
## 2. Modelo

Schelling desarrolló tres modelos: Modelo de distribución lineal, modelo de distribución de área y modelo de vecindario delimitado. Estos modelos son una de las primeras simulaciones basadas en agentes en ciencias sociales (Hatna & Benenson, 2012). En estos modelos, existen agentes que pertenecen a dos grupos distinto de la población y que se mueven en un espacio urbano siguiendo diferentes reglas.
El modelo de distribución lineal considera dos tipos de agentes y los posiciona en una línea que comienza aleatoriamente distribuida. Dado un agente focal se considera como “vecindario” los ocho vecinos más cercanos de este agente. De esta manera se puede medir que agentes están satisfechos o insatisfechos con su vecindario evaluando que fracción de vecinos más cercanos pertenece a su mismo grupo. Los vecinos insatisfechos son aquellos que superan un umbral de satisfacción y tienen un vecindario con una mayor cantidad de personas de otro grupo. Aquellos vecinos insatisfechos podrán cambiarse a una ubicación diferente (Ubareviciene & Tammaru, 2022).
El modelo de distribución de área y el modelo de vecindario delimitado introduce la noción de espacio geográfico, donde una ciudad es modelada teóricamente como un conjunto de pequeños cuadrados similar a un tablero de ajedrez de NxN ubicaciones. Al igual que el modelo lineal ambos grupos (B y R) comienzan aleatoriamente distribuidos, sin embargo, un porcentaje de las ubicaciones (E%) estará vacías. Las reglas de estos modelos son similares al modelo lineal donde cada agente k tiene un parámetro de satisfacción Sk dado por la fracción de vecinos del mismo tipo. Los agentes insatisfechos son aquellos que superan un umbral y tienen un vecindario con una mayor cantidad de personas de otro grupo, aquellos vecinos insatisfechos podrán cambiarse a una ubicación diferente

## 3. Modelo

