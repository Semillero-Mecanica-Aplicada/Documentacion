---
title: Configuración de la Red Neuronal
tags: Acta
---
**Grupo Lunes**

## Problema

El principal reto en esta etapa del proyecto fue definir y establecer los cambios a implementar en las diferentes pruebas para la red neuronal. Esto implicó planificar las modificaciones necesarias para adaptar la arquitectura y los parámetros de entrenamiento según los objetivos específicos de cada experimento.

## Desarrollo de la reunión

- En primera instancia, se realizó un análisis detallado de la arquitectura de una red neuronal diseñada para procesar imágenes en 3D con un tamaño fijo de 101 píxeles, adecuado para la tarea que queremos realizar, sacada de Three-dimensional convolutional neural network (3D-CNN) for  heterogeneous material homogenization[^1].

[^1]: [https://www.sciencedirect.com/science/article/abs/pii/S0927025620303414](https://www.sciencedirect.com/science/article/abs/pii/S0927025620303414)

<p align="center">
    <img src="{{ site.baseurl }}/assets/img/Red_referencia.png" alt="Red neuronal de referencia" width="800">
</p>
- A partir de este análisis, se definieron los cambios y variaciones que se implementarán en las distintas pruebas a realizar con PyTorch. Estas modificaciones incluyen ajustes en las capas, funciones de activación, parámetros de entrenamiento y otras configuraciones relevantes.
- Esta planificación busca optimizar el rendimiento del modelo y evaluar cómo cada cambio impacta en la capacidad de la red para aprender y generalizar sobre las imágenes binarias generadas.

## Compromisos Futuros

- Ejecutar las pruebas con las diferentes configuraciones establecidas en PyTorch.
- Analizar los resultados obtenidos para determinar la mejor configuración.
- Continuar ajustando la arquitectura en función de los hallazgos y las necesidades del proyecto.
