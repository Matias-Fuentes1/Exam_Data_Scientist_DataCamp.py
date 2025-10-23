# RealAgents - Prediccion del precio de venta

Descripcion general
- RealAgents es una agencia inmobiliaria que opera en una misma área metropolitana y se especializa en la venta de distintos tipos de viviendas.
- Ante la variabilidad en la velocidad de venta, la empresa busca optimizar los precios de sus propiedades mediante la predicción del precio de venta según las características de cada casa, con el objetivo de reducir el tiempo en el mercado y mantener su competitividad.

Objetivo del proyecto
Desarrollar un modelo predictivo que estime el precio de venta de una casa en función de sus características estructurales y de ubicación (como el área, el tipo de vivienda, la ciudad, y la fecha de venta).
Lo que permite:
· Anticipar el rango de precios razonable para cada propiedad.
· Detectar viviendas sobrevaluadas o subvaluadas.
· Mejorar la eficiencia del proceso de venta.

Modelo predictivo
Se entrenó un modelo de regresión Ridge, utilizando variables categóricas transformadas en dummies y un conjunto de entrenamiento con información histórica de ventas.
El modelo genera predicciones de precios para un conjunto de validación (validation.csv) que contiene 300 viviendas.

Hallazgos
* Se observó una amplia variabilidad de precios, con viviendas que van desde aproximadamente 120.000 hasta más de 380.000 unidades monetarias.
* Las predicciones permiten identificar los rangos de precios esperados según la ciudad, el tamaño y el tipo de vivienda, lo cual puede ser usado por RealAgents para definir estrategias de venta más competitivas.

# Analisis complementario - Importancia de variables

Como análisis adicional, se calculó la importancia de las variables del modelo Ridge para identificar cuáles influyen más en la estimación del precio.

Hallazgos 
* Las ciudades Teasdale y Silvertown están asociadas con precios de venta más altos, mientras que Riverford muestra una relación negativa con el precio.
* El tipo de vivienda influye en el valor: las casas Terraced y Semi-detached tienden a ser menos costosas.
* El área construida presenta una relación positiva con el precio, confirmando que las propiedades más grandes alcanzan valores más elevados.
