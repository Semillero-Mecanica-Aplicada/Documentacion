---
title: Charla sobre Elasticidad
tags: Charla
---

El concepto de elasticidad se basa en la relación entre esfuerzos y las deformaciones que sufre un elemento sólido. Para entender mejor la relación entre estos dos conceptos se debe empezar por comprender cada uno por aparte.
Esfuerzo se refiere a la fuerza sobre unidad de área aplicada sobre un objeto, que suele tener unidades de Newtons sobre metro cuadrado, o “pascales” (representado usualmente con la letra griega sigma “σ”):

<img src="{{ site.baseurl }}/assets/img/esfuerzo.png" alt="Grafica Esfuerzo" width="600">


Existen 5 tipos de esfuerzos que varían según la manera en que se aplique la fuerza:
-	**Compresión:** La fuerza se aplica de forma axial (dirección longitudinal del objeto) y tiende a comprimir o apisonar el elemento.
-	**Tracción:** Igual que la compresión, pero la fuerza se aplica de tal manera que tiende a estirar el elemento.
-	**Flexión:** Se produce cuando un elemento está apoyado en sus extremos, y se le aplica una carga opuesta en su zona central que ocasiona una curvatura en este de tal manera que una mitad queda sometida a compresión, y la otra a tracción.
-	**Corte:** Se da cuando se aplica una fuerza transversal al área, ocasionando un “corte” en dicha zona.
-	**Torsión:** Se refiere a la aplicación de momentos de giro en sentido opuesto en cada extremo del elemento, que tiende a retorcerlo sobre su eje longitudinal.	

<img src="/assets/img/Tipos-esf.png" alt="Tipos de esfuerzo" width="600">

Por su parte, la deformación se refiere al movimiento relativo entre las partículas del elemento cuando se aplica un esfuerzo. Es decir, si un esfuerzo mueve todas las partículas que componen al elemento (el equivalente a decir que el elemento entero se está desplazando), en este caso no existe movimiento relativo entre ellas, y por lo tanto no habrá deformación.
La forma estándar de medir esta magnitud es a través de la “deformación unitaria” (representado con la letra griega épsilon “ε”), que se calcula como el cambio en la longitud del elemento dividido en la longitud original del mismo (valor adimensional):

<img src="/assets/img/def.png" alt="Deformación" width="600">

A partir de estos dos conceptos, se puede definir una gráfica que relaciona los esfuerzos y las deformaciones que sufre un sólido conocida como “curva de elasticidad”

<img src="/assets/img/curva-esf-def.png" alt="Curva esfuerzo vs deformación" width="600">

Esta gráfica permite entender a fondo el comportamiento del elemento cuando se somete a un esfuerzo dado, dividiéndose en dos secciones principales; la zona elástica, y la zona plástica. La primera se da al comienzo de la aplicación del esfuerzo, y se caracteriza por tener una tendencia lineal donde si se le quita el esfuerzo al elemento este podrá recuperar su forma original, mientras que en la segunda cualquier incremento de esfuerzos provocará una deformación permanente en el elemento, hasta llegar al punto de ruptura donde termina la curva.
De aquí se pueden definir dos parámetros fundamentales en el análisis de elasticidad de sólidos. El primero es el módulo de Young “E”, que viene a ser la pendiente de la zona elástica de la curva de elasticidad, y considerando que el eje “y” corresponde a esfuerzos, y el “x” a deformaciones, la pendiente se definiría como el cambio en esfuerzos sobre el cambio en deformación unitaria, quedando en unidades de pascales.

El segundo parámetro viene a ser el coeficiente de poisson “v”, que se define como la deformación en sentido contrario a la fuerza aplicada, sobre la deformación en el sentido de la fuerza que sufre el elemento, donde el valor máximo que puede alcanzar es de 0,5.

Aparte de estos dos que dependen exclusivamente de esfuerzos axiales (compresión o tracción), se puede establecer un tercero para el caso de esfuerzos cortantes (representado con la letra griega tau) llamado “módulo cortante/de cillazamiento”, que al igual que el módulo de Young relaciona esfuerzos y deformaciones, pero al ser esfuerzos de corte las deformaciones van a ser de carácter angular, las cuales tienden a deformar los ángulos que componen el objeto.

A partir de estos tres parámetros, se pueden establecer algunas ecuaciones que relacionan directamente los esfuerzos axiales y cortantes, con sus respectivas deformaciones en los ejes x, y, o z.