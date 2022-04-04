# Evaluación 1

La evaluación 1 consiste en la resolución de un cuestionario. Para resolverlo, tendrá que poner en práctica los conocimientos y herramientas aprendidas durante el curso de las unidades 1 y 2.

La fecha límite de entrega es el día jueves 21-04-2022. Realice la entrega al email diabbluis@gmail.com, con asunto **evaluación 1 de minería de datos - nombre y apellidos**. Para el formato del entregable tiene dos opciones: escribir un informe y entregarlo en pdf, o escribir un notebook (jupiter, colab, kaggle, etc). En ambos casos, el entregable debe contener la respuesta a las preguntas planteadas, el código usado para contestarlas y sus resultados (output). 

## Cuestionario

El cuestionario completo consta de 6 puntos, más un bonus de 0,5 puntos. Para resolver este cuestionario, deberá emplear el dataset [earthquakes.csv](earthquakes.csv), que es un registro de sismos ocurridos alrededor del mundo, recopilados del Servicio Geológico de los Estados Unidos.


### Diccionario de datos

| Columna | Tipo | Comentario |
| ------- | ---- | ---------- |
| id | String | El nombre único de cada sismo. |
| impact.gap | Float | En general, mientras más pequeño sea este número, más confiable es la posición horizontal calculada del sismo. Específicamente, esto significa la mayor brecha azimutal entre estaciones azimutalmente adyacentes (en grados). Las ubicaciones de terremotos en las que la brecha azimutal supera los 180 grados suelen tener grandes incertidumbres de ubicación y profundidad. Varía entre 0 y 180. |
| impact.magnitude | Float | La magnitud del sismo es una medida del tamaño de un sismo en su origen. Es una medida logarítmica de base 10. Típicamente varía desde -1 (0.1, muy pequeño) a 10 (increíblemente poderoso). |
| impact.significance | Integer | Un número que describe cuán significativo es un evento. Números grandes indican un evento más significativo. Varía entre 0 y 1000. |
| location.depth | Float | Profundidad del evento en kilómetros. |
| location.distance | Float | La distancia aproximada entre la fuente del sismo y la estación que lo reporta, medida en grados. 1 grado equivale aproximadamente a 111.2 kilómetros. En general, mientras más pequeño es este número, más confiables la profundidad calculada del sismo. En general, este número varía entre 0.4 y 7.1. |
| location.full | String | El nombre completo de la ubicación. |
| location.latitude | Float | Grados decimales de latitud (hacia arriba y abajo en el globo). Tiene valores negativos para latitudes del hemisferio sur. Varía entre -90 y 90. |
| location.longitude | Float | Grados decimales de longitud (hacia este y oeste en el globo). Tiene valores negativos para el oeste. Varía entre -180 y 180. |
| location.name | String | Una mejor suposición para el nombre del estado (o país, en algunos casos) en el que se informó este sismo. |
| time.full | String | La representación fecha/tiempo completa para cuando ocurrió el sismo. |
| deaths | String | Número de fallecimientos producto del sismo. |

### Ejercicio 1 (2 puntos)

1. Importe y describa el dataset. ¿Qué observaciones puede realizar? (**1 punto**)
2. Analice y dé tratamiento a los datos faltantes, outliers e incoherencias. Justifique el tratamiento que dé (o que no dé). (**1 punto**)

### Ejercicio 2 (4 puntos)

1. Explore las variables. ¿Cuáles considera más importantes para el Servicio Geológico de los Estados Unidos?, ¿por qué? (**0,5 puntos**)
2. Analice gráficamente las distribuciones de las 3 variables más importantes, ¿qué propiedades y características tienen? (**1 punto**)
3. Transforme las variables analizadas y analice su nueva representación. ¿Qué propiedades y características tienen? (**1 punto**)
4. Compare los sismos entre México y Chile. ¿Son los sismos en Chile más intensos que en México? Utilice herramientas descriptivas e inferenciales. (**1,5 puntos**)

### Bonus (0,5 puntos)

Proponga un proyecto para la Oficina Nacional de Emergencia del Ministerio del Interior (ONEMI) cuyo input sean estos datos de sismos. Describa brevemente, ¿qué herramientas, de las aprendidas en la asignatura, utilizaría para llevar a cabo este proyecto?
