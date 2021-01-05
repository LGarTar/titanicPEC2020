# Notebook de análisis del Titanic

Se trata de un notebook en R para llevar a cabo un análisis del Titanic para la asignatura Tipología y ciclo de vida de los datos.

## Nota sobre el uso
**El código está escrito en R.**
**El documento resultante principal es el generado en html, con una estética más cuidada y moderna, adjuntamos también el documento en PDF, con menor tratado estético para maximizar la compatibilidad.**

## Descripción Dataset Titanic
El dataset se compone de los siguientes campos:

* PassengerId: Identificador del pasajero
* Survived: Indica si el pasajero sobrevivió. Si vale 0 entonces no sobrevivión, si vale 1 entonces es un superviviente
* Pclass: Indica la clase en la que viajaba el pasajero (1 = 1st, 2 = 2nd, 3 = 3rd)
* Name: Nombre y apellidos del pasajero
* Sex: Sexo del pasajero
* Age: Edad en años	
* SibSp: Número de hermanos / esposas a bordo del Titanic
* Parch: Número de padres / hijos a bordo del Titanic	
* Ticket: Número de ticket
* Fare: Precio que ha pagado el pasajero por el viaje
* Cabin: Número de la cabina del pasajero	
* Embarked: Puerta de embarque (C = Cherbourg, Q = Queenstown, S = Southampton)

Este dataset es muy relevante porque se refiere a los pasajeros del Titanic, indicando además si el pasajero consiguió sobrevivir o no al naufragio.

A través de este dataset se puede analizar distintos aspectos sobre quiénes sobrevivieron, por ejemplo si las mujeres y los niños se salvaron en relación a los hombres, si el hecho de viajar en una clase u otra podría implicar un mayor o menor ratio de supervivencia.

Este dataset es además un clásico a nivel de formación y ejemplos de estadística y minería de datos.

## Acciones realizadas sobre el dataset

Se han llevado a cabo las siguientes acciones sobre el dataset:
* Integración y selección de los datos de interés a analizar.
* Limpieza de los datos.
* Identificación y tratamiento de valores extremos.
* Análisis de los datos.
* Representación de los resultados a partir de tablas y gráficas.
* Conclusiones.

## Conclusiones una vez analizado dataset

A modo de resumen, hemos visto a lo largo del análisis los siguientes puntos:

* Hay variables como Name y PassengerId que no aportan información a priori al análiis y que hemos decidido eliminar.
* En el caso del tratamiento de valores vacíos, en algunos casos hemos podido eliminar directamente las observaciones al ser pocos casos (embarked), en otros hemos podido aplicar la media (Age) y otros casos se referían a pasajeros que no viajaban en cabina.
* No hemos encontrado outliers fuera de lo normal, estaban dentro del dominio.
* Hemos visto que catplant, la categoría por planta, no afectaba en cuanto a nivel de supervivencia.
* Hemos demostrado mediante contraste de hipótesis que de media los supervivientes son más jóvenes que quienes acabaron muriendo.
* Hemos visto también que hay una relación entre sexo y supervivencia por contraste de hipótesis.
* A través de una regresión lineal hemos visto cierta dependencia entre edad y supervivencia aunque era una dependencia débil.
* Mediante un árbol de decisión, hemos comprobado que se cumple la hipótesis inicial de que había más probabilidad de salvarse si se era mujer o niño y que viajar en tercera clase suponía una mayor probabilidad de morir que en el resto de clases.
* Con las correlaciones hemos visto que el precio del ticket tiene un nivel de relación muy bajo con respecto a la edad.
* Podemos ver por tanto, que la conocida cita de “Mujeres y niños primero”, se cumplía en general, seguida de un fuerte sesgo por clases económicas.
