---
layout: post
title: Generación de imagenes parte 2
date: 2025-05-05
---
**Grupo Lunes**
## Problema
En esta etapa del proyecto, el principal problema a resolver fue el desarrollo de un algoritmo capaz de generar imágenes binarias aleatorias. Este paso era fundamental para suplir la falta de una base de datos real, permitiendo así contar con un conjunto de datos artificial, pero confiable, para las siguientes fases del proyecto.
## Desarrollo de la reunión
- Durante la reunión se revisó el funcionamiento del algoritmo desarrollado en Python para la generación de imágenes binarias. Se confirmó que este produce imágenes aleatorias válidas, que se almacenan correctamente y que es posible repetir el proceso gracias al uso de una semilla y al guardado del estado interno del generador aleatorio.
- Una vez validado el funcionamiento del algoritmo, se implementó un mecanismo de verificación para asegurar que no hubiera imágenes repetidas. Para ello, se utilizó una función hash aplicada sobre cada imagen, lo que permitió comprobar que todas eran únicas.
- Un hash es el resultado de aplicar una función matemática (llamada función hash) que toma una entrada de cualquier tamaño (como una imagen, un archivo o un texto) y la transforma en una secuencia corta de longitud fija, generalmente representada como un número o una cadena de caracteres. 


## Compromisos Futuros
- Discutir el uso de las imágenes generadas para entrenamiento.
- Evaluar posibles configuraciones de redes neuronales convolucionales.
- Definir una estrategia inicial para el diseño y pruebas del modelo.
