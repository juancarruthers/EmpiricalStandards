# Visualización de la Información

Diagramas que asignan valores cuantitativos a objetos visuales y a sus atributos visuales para ayudar a la comprensión

## Aplicación

Esta guía transversal se aplica a las visualizaciones de datos cuantitativos. La visualización gráfica consiste en diagramas que asignan valores cuantitativos a objetos visuales (por ejemplo, segmentos, puntos, círculos) y a sus atributos visuales (por ejemplo, longitud, posición, tamaño, color). Su objetivo es ayudar al lector en una tarea de comprensión de datos. No aplica a:

-   Visualización de software, como mostrar la estructura o arquitectura de un producto de software.
-   Diagramas que no codifican valores cuantitativos, p. Ej. Diagramas de actividad UML, diagramas BPMN, diagramas de flujo.
-   Tablas que codifican datos en formato textual.

## Atributos

- [ ]   Proporcionalidad
    -   los valores/medidas se informan de manera uniformemente proporcional:
        la relación de dos valores es igual a la relación geométrica en papel (o pantalla) de los atributos visuales correspondientes (longitud, área, pendiente, etc.) \[factor de mentira\]
    -   los atributos visuales proporcionan una percepción precisa de la proporción, según el ranking de atributos:
        -   posición en una escala común
        -   position en escalas idénticas
        -   largo
        -   ángulo/pendiente
        -   área
    -   los diagramas se renderizan en 2D y se abstienen de perspectivas 3D que podrían alterar la percepción de las dimensiones
    -   la codificación de medidas ordinales a través de colores usa la saturación y la luminosidad y evita las paletas de arcoíris


- [ ]   Utilidad

     - todos los elementos del diagrama transmiten información útil o ayudan a la claridad
     - el diagrama no contiene elementos gráficos o sobre-diseñados que interfieren con la percepción o la comprensión
     - los diferentes colores representan la variación de los datos
     - el fondo es claro y uniforme
     - no hay efectos decorativos 3D
     - los colores brillantes y saturados se utilizan únicamente para enfatizar
     - las cuadrículas son ligeras y no oscurecen los datos
     - las anotaciones son menos prominentes que los datos

- [ ]   Claridad

    -   el diseño del diagrama y la anotación de texto apoyan la comprensión de los datos y hacen que la visualización sea lo más autónoma posible
        -   el título (o la leyenda de la figura) transmite de manera concisa cuál es el contenido de la visualización y el mensaje deseado
        -   las anotaciones de texto guían al lector a comprender el mensaje
    -   se utiliza el etiquetado directo en lugar de una leyenda separada, especialmente cuando hay más de dos códigos de color
    -   la codificación de colores de las medidas categóricas se limita a un máximo de 5 niveles distintos; más colores son demasiado difíciles de discriminar
    -   cuando hay mucha densidad de datos, se aplican las técnicas adecuadas para mitigar la sobreimpresión
    -   los ejes y las marcas de graduación relativas están etiquetadas
    -   el tamaño del texto es lo suficientemente grande para que sea legible
    -   evitar el texto en diagonal o vertical
    -   El formato de imagen es preferentemente vectorial, si se utiliza un formato rasterizado debe tener suficiente resolución.

- [ ]   Diseño del Diagrama

     - el diagrama contiene como máximo dos ejes a menos que una superficie (función de dos variables) sea la representación estándar
     - el uso de escalas logarítmicas se destaca explícitamente
     - los objetos de datos (por ejemplo, barras) se ordenan de forma significativa (por ejemplo, ascendente, descendente o agrupados) para facilitar la comparación
     - la visualización no interactiva debe servir para una única tarea de comprensión
     - el tipo de visualización es apropiado para la tarea de comprensión visual que se pretende apoyar (Tabla 1)
     - el diseño es amigable para los daltónicos - utiliza una paleta segura para los daltónicos para la codificación de colores o una variable visual redundante (por ejemplo, saturación, patrón)
     -*(opcional)* por lo general, varias series de datos deben informarse utilizando varios diagramas pequeños en lugar de un solo diagrama abarrotado

### Tabla 1: Cuándo usar qué visualización

| Tarea de Comprensión | Tipo de Visualización comunmente utilizada                                                            |   
|--------------------|------------------------------------------------------------------------------------------------|
| Comparación         | Gráfico de barras, gráfico de puntos, mapa de calor, gráfico de bandas, isotipo                                               |  
| Correlación        | Gráfico de dispersión, gráfico de burbujas, gráfico de pendiente, diagrama de mancuernas, barras divergentes                         |   
| Desviación          | Gráfico de viñetas, gauge                                                                            |   
| Distribución       | Histograma, polígono de frecuencia, densidad acumulada, gráfico de cuantil-cuantil, gráfico de caja, gráfico de violín |   
| Geo localización       | Mapa coroplético, cartograma                                                                       |   
| Parte de un todo      | Gráfico de barras, barras apiladas, mapa de árbol, diagrama de Waffle, pastel                                                   |  
| Orden           | Gráfico de barras, gráfico de puntos, lollypop                                                                   | 
| Series temporales        | Gráfico de línea, gráfico de barras, gráfico de flujo                                                               | 

## Antipatrones

- Uso de barras truncadas para exagerar las diferencias, comprometiendo la proporcionalidad en lugar de usar otras representaciones (por ejemplo, diagramas de puntos)
- Utilizar gráficos circulares para más de 5 categorías y/o sin etiquetado directo de las porciones
- Uso de escalas verticales duales que son difíciles de leer y se prestan a la ambigüedad debido a la selección arbitraria de rangos de ejes
- Usar cualquier efecto 3D o decoración que pueda alterar la percepción
- Uso de gráficos de líneas para mostrar variables no ordenadas

## Lecturas Sugeridas

Colin Ware. 2000. Information Visualization: Perception for Design.
Morgan Kaufmann Publishers, Inc., San Francisco, California.

David Borland and R. M. Taylor Ii. 2007. Rainbow Color Map (Still)
Considered Harmful. *IEEE Computer Graphics and Applications*. 27, 2,
14–17.

Financial Times Visual Journalism Team. Visual Vocabulary. Retrieved
July 12, 2020 from <https://ft.com/vocabulary>

Claus O. Wilke. Fundamentals of Data Visualization, O'Reilly, 2019.
Retrieved July 12, 2020 from <https://serialmentor.com/dataviz/>

Simon Fear. Publication quality tables in LATEX. 2020. Retrieved July
12, 2020 from
<http://mirrors.ctan.org/macros/latex/contrib/booktabs/booktabs.pdf>
