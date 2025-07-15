---
title: Integración FEM parte 2 - Abordando las Condiciones de Frontera Periódicas
tags: Acta
---
**Grupo Miércoles**

## Problema
La geometría del material que obtenemos a partir de la traducción de las imágenes binarias en propiedades mecánicas es tan solo una celda unitaria que al ser teselada en las dos direcciones del espacio 2D conforma un material periódico en una escala superior. Considerando esto, requerimos de una herramienta o algún método que permita imponer condiciones de frontera periódicas en nuestra celda unitaria al momento de resolver con FEM para así tener congruencia con el modelo material que estamos simulando.

## Desarrollo de la reunión

- Se propone como solución explorar el uso de *Multi-Point* o *Multi-Freedom Constraints*, las cuales consisten en ecuaciones adicionales que se añaden al sistema matricial del problema elástico. Recordemos que este sistema inicialmente lo podemos escribir de la siguiente manera:

$$ [K] \{U\} = \{F\} $$

Donde $[K]$ es la matriz de rigidez del sistema, $\{U\}$ es el vector de desplazamientos y $\{F\}$ el vector de fuerzas. Utilizaremos elementos de tipo barra para las simulaciones FEM, por lo que cada uno de los nodos de nuestra malla tiene asociados 2 grados de libertad (ó DoF por sus siglas en inglés); uno en la dirección $x$ y otro en la dirección $y$. Pra nuestro caso particular, esto implica que si realizamos el análisis FEM para una geometría con 64x64 elementos, el número de nodos en cada una de las direcciones del material sería de 65 (uno más que el número de elementos en cada dirección) y el número de DoF globales sería de $65*2=130$. 

Las condiciones de restricción adicionales a este sistema se usan para dar coherencia a la condición de periodicidad del problema. Lo que hacemos con estas condiciones es, por ejemplo, asociar los grados de libertad de la pared izquierda de nuestro material con los grados de libertad de la pared derecha, de modo que imponemos que el desplazamiento de este conjunto de nodos sea igual (o con una constante adicional, $\varphi$ de diferencia). Esta asociación de grados de libertad también se impone sobre los nodos inferiores y superiores, al igual que entre el nodo de la esquina inferior izquierda y el de la esquina superior derecha. 

Esto anterior es ejemplificado más claramente con la siguiente imagen:

*Imagen*

En últimas, estas ecuaciones adicionales causan la reducción del sistema matricial, donde se puede utilizar un solucionador lineal para hallar nuestro nuevo vector de desplazamientos reducido, $\{ U_R \}$. El nuevo sistema se ve así:

$$ [T] [K] [T^T] \{U_R \} = [T] \{F\} $$

Donde $[T]$ será la matriz 

## Compromisos Futuros
- Escribir la rutina en Python que permite calcular la matriz $[T]$ de nuestro problema, con base en unas condiciones de frontera periódicas establecidas.
- Considerando que estamos trabajando con un material compuesto, donde debemos elegir dos materiales que lo forman ¿Cuáles serán las propiedades mecánicas que emplearemos para dichos materiales?
