---
title: Charla sobre FEM
tags: Charla
---

## Reunión Semillero – Charla FEM (Finite Element Method)
En la reunión de semillero se llevó a cabo una breve charla o explicación protagonizada por Estefanía Moreno, Alejandra Botero y Daniel Ospina donde se explicó cuales eran los principios del método de elementos finitos (FEM), aplicaciones y programas que se podrían emplear para aprender con más profundidad.

## FEM (Finite Element Method)
En el mundo matemático de la predicción de comportamiento de objetos o semiespacios ante una situación específica (Imposición de carga, desplazamiento, etc.) existen dos métodos o maneras de hacerlo. Por un lado, están las soluciones analíticas, que son básicamente una ecuación en funciones de una o más variables que es exacta, y te da la respuesta que tendrá el sistema de forma directa, siendo posible conocer el valor exacto de respuesta del elemento. Y por el otro lado se tiene la solución numérica, que también responde a la misma necesidad, pero usando interpolación, en este caso no se cuenta con una ecuación para la obtención del valor exacto de respuesta, sino que se busca calcularla a partir de condiciones de frontera e información con nodos vecino de forma aproximada.

De esta manera, FEM es un método que permite dar respuestas aproximadas numéricamente mediante interpolaciones y datos ya medidos, además de otras condiciones técnicas que se establecen. La principal idea de su funcionamiento consiste en el uso de “elementos finitos”, que son pequeños diferenciales de área o fragmentos del objeto a analizar, y a partir de las condiciones insertadas y el conocimiento de información de las celdas o nodos vecinos, se puede conocer cual sería la aproximación de valor para el elemento en concreto.
Para desarrollar un modelo FEM es importante seguir los siguientes pasos:

1.	**Discretizar:** consiste en fragmentar el elemento total en pequeñas micro divisiones realizadas para predecir la respuesta. Entre más de estas haya, más adecuada es la aproximación. En esta fase se define el número de elementos finitos para el espacio, de tal forma que se obtenga buena precisión, pero sin una carga computacional innecesariamente exagerada, solo se debe buscar donde el error converge. De igual manera, se pueden definir patrones para los datos insertados. ¿Cómo sé cuántos Elementos Finitos son suficientes para mi modelo? A partir de la práctica y criterio ingenieril, se analizan los resultados y se miran sus valores comparativos.

2.	**Pre-Procesamiento:** aquí se definen factores como la geometría, condiciones de frontera o carga y desplazamiento, además de características del material, que serán aquellos datos que le inserten un estado de respuesta al objeto.

3.	**Mallado:** consiste en dividir un objeto o dominio complejo en pequeñas partes llamadas elementos finitos, conectados entre sí por nodos, con el fin de aproximar y resolver numéricamente ecuaciones diferenciales que describen fenómenos físicos. Estos elementos pueden tener distintas formas (como triángulos o tetraedros) y su tamaño y distribución afectan directamente la precisión y el costo computacional del análisis. El mallado permite representar con mayor detalle las zonas críticas del modelo, adaptándose a geometrías irregulares y facilitando el cálculo de variables como esfuerzos, desplazamientos o temperaturas en todo el sistema. La idea es obtener un porcentaje de error en la predicción de la respuesta aceptable.

Con la información y pasos realizados anteriormente, se puede proceder con la predicción de la respuesta. Es importante recalcar que se deben definir todos los espacios de las fronteras, incluso si no tiene ninguna condición o carga, son datos que se emplean para la aplicación del método numérico.

Es importante recalcar que la filosofía del método me dice que no puedo saber todo al mismo tiempo, por ejemplo, en el caso de esfuerzos y deformaciones, usualmente conozco uno de ellos y, mediante métodos numéricos, puedo predecir el valor del otro parámetro, y justo en esto consiste FEM.
Las aplicaciones de FEM son muchas, por ejemplo, se aplica ampliamente en ingeniería y ciencia para analizar y simular el comportamiento físico de sistemas complejos. En ingeniería mecánica y estructural se usa para calcular esfuerzos, deformaciones y fallas en piezas o estructuras; en ingeniería civil permite evaluar edificaciones, túneles, presas y cimentaciones. También es clave en la industria automotriz y aeroespacial para simular choques, vibraciones y condiciones extremas, así como en medicina para modelar huesos, tejidos y dispositivos protésicos. Además, se aplica en estudios térmicos, transferencia de calor y flujo de fluidos, lo que lo convierte en una herramienta esencial para el diseño y optimización de sistemas físicos reales.

Por últimos, algunas de las aplicaciones, programas o códigos que se pueden usar para la aplicación de FEM o integración más directa al método son “SolidsPy” y “Calculix”
