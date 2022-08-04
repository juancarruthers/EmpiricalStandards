# Simulación (Cuantitativa)
<standard name="Simulation">



*<desc>Un estudio que involucra el desarrollo y uso de un modelo matemático que imita el comportamiento de un sistema del mundo real, que a menudo implica comprensión de problemas, recolección de datos, desarrollo de modelos, verificación, validación, diseño de experimentos, análisis de datos e implementación de resultados.</desc>*
                                                                                                                                                                                                                                                                                                                                     


## Aplicación

El estándar se aplica a los estudios de investigación que utilizan la simulación para comprender, evaluar o mejorar un sistema o proceso y su comportamiento. Utilice este estándar para simulaciones _in silico_, es decir, estudios que representan todo utilizando modelos computacionales. Para simulaciones _in virtuo_, es decir, participantes humanos que manipulan modelos de simulación, utilice el estándar **Experimentos (con participantes humanos)**. Para las simulaciones que se utilizan para evaluar un artefacto tecnológico nuevo o mejorado, considere también el estándar **Investigación en Ingeniería**.

## Atributos Específicos

### Atributos Esenciales
<checklist name="Essential">

<intro>

- [ ] Justifica que la simulación es un método adecuado para investigar el problema (o pregunta de investigación, etc.)

<method>

- [ ] Describe el modelo de simulación (niveles conceptual, de implementación o de abstracción híbrida), incluidos los parámetros de entrada y las variables de respuesta
- [ ] Describe el enfoque de simulación subyacente<sup>[1](#myfootnote1)</sup>
- [ ] Describe los paquetes de simulación o las herramientas que se utilizan para desarrollar y ejecutar el modelo de simulación, incluidos los números de versión y los entornos computacionales
- [ ] Describe los datos utilizados para la calibración del modelo, los procedimientos de calibración y la información contextual
- [ ] Describe cómo se verificó y validó el modelo de simulación en diferentes niveles de abstracción<sup>[2](#myfootnote2)</sup>
- [ ] Describe el protocolo del estudio, incluidas las variables independientes, los escenarios, el número de ejecuciones por escenario (en caso de utilizar simulación estocástica) y las condiciones de estado estable o de terminación
- [ ] Analiza las amenazas de validez considerando los datos de respaldo y el modelo de simulación<sup>[3](#myfootnote3)</sup>
- [ ] Explica claramente los supuestos del modelo de simulación

<results>

<discussion>

<other>    

</checklist>
    
### Atributos Deseables
<checklist name="Desirable">

- [ ] Proporciona materiales complementarios que incluyen los datos brutos (para datos reales) o el mecanismo de generación (para datos sintéticos) utilizados para la calibración del modelo, todos los modelos de simulación y código fuente, scripts de análisis
- [ ] Caracteriza comportamientos de referencia para la definición de escenarios de simulación con valores representativos y conocidos o distribuciones de probabilidad para parámetros de entrada<sup>[4](#myfootnote4)</sup>
- [ ] Separa los niveles conceptual y de implementación del modelo de simulación
- [ ] Informa el análisis de sensibilidad para parámetros o factores de entrada
- [ ] Distingue claramente los resultados basados en evidencia de las interpretaciones y especulaciones<sup>[5](#myfootnote5)</sup>
</checklist>
    
### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Describe cómo las partes interesadas participaron en el desarrollo y la validación del modelo de simulación<sup>[6](#myfootnote6)</sup>
- [ ] Proporciona una vista modular del modelo de simulación, lo que permite su reutilización en diferentes contextos<sup>[7](#myfootnote7)</sup>
</checklist>

## Criterios Generales de Calidad

Validez de la conclusión, validez de constructo, validez interna (si se examinan las relaciones causales), validez externa y reproducibilidad.

## Antipatrones

- Sobreajuste<sup>[8](#myfootnote8)</sup>
el modelo de simulación para reproducir un comportamiento de referencia.
- Uso de diseños experimentales no estándar<sup>[9](#myfootnote9)</sup>
sin justificación.
- Uso de una sola ejecución en lugar de múltiples ejecuciones para experimentar con modelos estocásticos.

## Ejemplos de Desviaciones Aceptables

- Si los datos disponibles son insuficientes (o son demasiado costosos de recopilar) para calibrar el modelo, se pueden utilizar supuestos para implementar partes del modelo. Sin embargo, estos supuestos deben explicarse y justificarse.
- Cuando la traducción de un modelo conceptual a un modelo de implementación es sencilla, los autores pueden presentarlos juntos.
- Si el enfoque de simulación utilizado es muy común en la Ingeniería del Software (por ejemplo, simulación de eventos discretos, dinámica de sistemas), es suficiente indicar qué enfoque se utiliza, citando referencias apropiadas, en lugar de explicar en su totalidad cómo funciona el enfoque.

## Críticas Inválidas

- La mera presencia de supuestos en el modelo no es una base válida para la crítica _siempre que_ los supuestos estén documentados y justificados, y sus implicaciones para la validez de la simulación estén suficientemente abordadas. Todos los modelos hacen suposiciones.
- Afirmar que el modelo es demasiado abstracto sin explicar por qué el nivel de abstracción es inadecuado para los propósitos del estudio.
- Afirmar que el estudio no es válido porque utiliza datos generados, datos secundarios o aproximaciones basadas en la opinión de expertos, _cuando no se dispone de datos primarios adecuados_.

## Lecturas Sugeridas

Nauman Bin Ali, Kai Petersen. A consolidated process for software process simulation: State of the art and industry experience. In: _38th Euromicro Conference on Software Engineering and Advanced Applications_, 2012, IEEE, pp 327–336.  

Nauman Bin Ali, Kai Petersen, Claes Wohlin. A systematic literature review on the industrial use of software process simulation. _Journal of Systems and Software_, 97, 2014, 65–85.  

Dietmar Pfahl. Process Simulation: A Tool for Software Project Managers? In: Günther Ruhe, Claes Wohlin (Eds.) _Software Project Management in a Changing World._ Springer-Verlag Berlin Heidelberg, 2014, 425-446.  

Ivo Babuska, and J. Tinsley Oden. Verification and validation in computational engineering and science: basic concepts. _Computer methods in applied mechanics and engineering_, 193, 36, 2004, 4057–4066.  

Breno Bernard Nicolau de França, Nauman Bin Ali. The Role of Simulation-Based Studies in Software Engineering Research. In: Felderer M., Travassos G. (eds) _Contemporary Empirical Methods in Software Engineering_. Springer, Cham. 2020. https://doi.org/10.1007/978-3-030-32489-6\_10.  

Breno Bernard Nicolau de França, Guilherme Horta Travassos. Experimentation with dynamic simulation models in software engineering: planning and reporting guidelines. _Empirical Software Engineering_, 21, 3, 2016, 1302–1345.  

Breno Bernard Nicolau de França, Guilherme Horta Travassos. (2015). Simulation Based Studies in Software Engineering: A Matter of Validity. _CLEI Electronic Journal_, 18(1), 5.  

Houston DX, Ferreira S, Collofello JS, Montgomery DC, Mackulak GT, Shunk DL. Behavioral characterization: finding and using the influential factors in software process simulation models. _Journal of Systems and Software_, 59, 3, 2001, 259– 270, DOI https://doi.org/10.1016/S0164-1212(01)00067-X.  

Kleijnen JPC, Sanchez SM, Lucas TW, Cioppa TM. State-of-the-art review: A user&#39;s guide to the brave new world of designing simulation experiments. _INFORMS Journal on Computing_, 17, 3, 2005, 263–289. DOI 10.1287/ijoc.1050.0136.  

Law AM. _Simulation modeling and analysis_. 5th ed., 2015, McGraw-Hill, New York.  

Madachy RJ. _Software Process Dynamics_, 2008, Wiley-IEEE Press.

## Ejemplares

Ali NB, Petersen K, de França BBN (2015) Evaluation of simulation-assisted value stream mapping for software product development: Two industrial cases. _Information &amp; Software Technology_ 68:45–61 [an example of a simulation-based study in industrial settings].  

Concas, Giulio, Maria Ilaria Lunesu, Michele Marchesi, and Hongyu Zhang. &quot;Simulation of software maintenance process, with and without a work‐in‐process limit.&quot; _Journal of software: Evolution and Process_ 25, no. 12 (2013): 1225-1248. [an example of model description and discussion of threats to validity].  

Garousi V, Khosrovian K, Pfahl D (2009) A customizable pattern-based software process simulation model: design, calibration, and application. _Software Process: Improvement and Practice_ 14(3):165–180, DOI 10.1002/spip.411. [an example of a complete report of a simulation-based study].  

Smith, Neil, Andrea Capiluppi, and Juan F. Ramil. &quot;A study of open source software evolution data using qualitative simulation.&quot; _Software Process: Improvement and Practice_ 10, no. 3 (2005): 287-300. [an example of a simulation study using a unusual simulation approach: qualitative simulation].  

---
<footnote><sup>[1](#myfootnote1)</sup> Por ejemplo, simulación de eventos discretos, dinámica de sistemas, simulación basada en agentes</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup> Algunos procedimientos de verificación y validación pueden aplicarse al modelo a nivel conceptual (por ejemplo, validando variables y relaciones) hasta un nivel de implementación (por ejemplo, usando pruebas, reproduciendo comportamientos de referencia o realizando experimentos simulados).</footnote><br>
<footnote><sup>[3](#myfootnote3)</sup> Los estudios de simulación son propensos a varias amenazas de validez, incluidos escenarios de simulación no representativos, verificación y validación insuficientes, uso de diferentes conjuntos de datos (contextos) para la calibración y experimentación de modelos, y otros (de França and Travassos, 2015).</footnote><br>
<footnote><sup>[4](#myfootnote4)</sup> Los comportamientos de referencia representan un modelo del mundo real (a menudo basado en la medición real de un sistema o proceso), que se caracteriza por la distribución de datos o una serie de variables del modelo. Por lo general, estos modelos se utilizan para validar los resultados de la simulación. Por ejemplo, una línea de base de esfuerzo y cronograma para la simulación de proyectos software.</footnote><br>
<footnote><sup>[5](#myfootnote5)</sup> Por lo general, basta con separar los resultados y la discusión en diferentes secciones. Sin especulaciones en la sección de resultados.</footnote><br>
<footnote><sup>[6](#myfootnote6)</sup> Además de los desarrolladores del modelo de simulación, las partes interesadas podrían ser proveedores de datos (para la calibración del modelo), expertos en el dominio (que pueden tener hipótesis sobre las relaciones causales entre las variables del modelo) y usuarios del modelo de simulación. Todas estas partes interesadas podrían, por ejemplo, participar en la verificación de la plausibilidad del resultado del modelo (verificación de validez aparente).</footnote><br>
<footnote><sup>[7](#myfootnote7)</sup> Entendiendo los modelos de simulación como software, pueden volverse demasiado grandes y difíciles de entender en una sola vista. Entonces, la idea es tener un modelo compuesto, en el que cada módulo se refiera a un conjunto particular de variables. El siguiente libro presenta un modelo completo sobre proyectos software en una perspectiva modular: Abdel-Hamid, T. and Madnick, S.E., 1991. Software project dynamics: an integrated approach. Prentice-Hall, Inc.</footnote><br>
<footnote><sup>[8](#myfootnote8)</sup> Por ejemplo, implementar un modelo específico capaz de producir solo los resultados deseados.</footnote><br>
<footnote><sup>[9](#myfootnote9)</sup> Houston et al. (2001) analiza algunos diseños experimentales habituales para la simulación de procesos software, como los diseños factoriales (fraccionarios). Para obtener una visión más general de los diseños experimentales para simulación, sugerimos Kleijnen et al. (2005).</footnote><br>

</standard>
