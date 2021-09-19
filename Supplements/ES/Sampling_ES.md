# Muestreo
Un estudio empírico en el que se seleccionan algunos de muchos elementos posibles.

## Aplicación

Este estándar se aplica a la investigación empírica en la que el investigador selecciona grupos más pequeños de elementos para estudiar (una _muestra_) de un grupo más grande de elementos de interés (la _población_) utilizando una lista de población generalmente imperfecta (el _marco de muestreo_). Los elementos comunes en la investigación de Ingeniería de Software incluyen personas (por ejemplo, desarrolladores de software), artefactos de código (por ejemplo, archivos de código fuente) y artefactos que no son código (por ejemplo, discusiones en línea, historias de usuarios).

## Atributos Específicos

### Atributos Esenciales
- [ ] Explica el objetivo del muestreo (por ejemplo, buscando la representatividad, identificando casos excepcionales)
- [ ] Explica la estrategia de muestreo, en particular los diferentes pasos de filtrado involucrados o las razones para seleccionar ciertos objetos
- [ ] Explica por qué la estrategia de muestreo es razonable (no necesariamente óptima) para el objetivo de muestreo
- [ ] Explica el razonamiento detrás de la selección de objetos de estudio (especialmente estudios cualitativos)
- [ ] Informa el tamaño de la muestra
 
#### Esencial solo si la representatividad es un objetivo 
- [ ] Establece la población teórica (¿a qué le gustaría generalizar al investigador?)
- [ ] Presenta una descripción algorítmica, concisa y replicable de cómo otros investigadores podrían obtener la misma muestra
- [ ] Argumenta explícitamente a favor de la representatividad (por ejemplo, compara los parámetros de la muestra y la población, proporciona un intervalo de confianza y un nivel de confianza para el tamaño de la muestra)
- [ ] Explica cómo la muestra podría estar sesgada a lo largo de los pasos de muestreo

### Atributos Deseables
- [ ] Informa los tamaños aproximados o exactos de las poblaciones y los marcos de muestreo
- [ ] Proporciona la muestra, el marco de muestreo y los scripts de muestreo como material complementario (sujeto a los datos recopilados que contienen información confidencial o protegida).
- [ ] Utiliza estrategias de muestreo más sofisticadas cuando corresponde, por ejemplo:

    - Investigación exploratoria: uso de muestreo deliberado en lugar de por conveniencia para la unidad de análisis
    - Estudio de caso: uso de muestreo deliberado en lugar de por conveniencia para la selección del sitio
    - Minería de repositorios: usando probabilidad en lugar de conveniencia o muestreo deliberado (si hay un marco de muestreo disponible)
    - Encuesta en línea: se utiliza un muestreo dirigido por encuestados en lugar de un muestreo de bola de nieve.
    - Estudio con estratos identificables: utilizando un muestreo aleatorio estratificado en lugar de un muestreo aleatorio simple
    - Construcción de teorías: utilizando un muestreo teórico en lugar de un muestreo por conveniencia

## Ejemplos de Desviaciones Aceptables

- Omitir una descripción detallada de la estrategia de muestreo porque se explica en trabajos anteriores utilizando el mismo conjunto de datos
- Utilizar una estrategia de muestreo muy simple en circunstancias excepcionales en las que la conveniencia supera la representatividad (por ejemplo, la investigación durante un desastre)

## Antipatrones

- Hacer afirmaciones sobre una población, basadas en una muestra, sin proporcionar un argumento a favor de la representatividad
- Afirmar que una muestra es representativa de una población porque se seleccionó al azar de un marco de muestreo, sin considerar el sesgo en el marco de muestreo.
- Llevar a cabo una investigación con poca potencia; es decir.:
    - Investigación cuantitativa con un tamaño de muestra insuficiente para detectar efectos del tamaño esperado<sup>[1](#myfootnote1)</sup>
    - Investigación cualitativa con muy pocos datos para una saturación plausible
- Justificar la selección de elementos simplemente indicando que provienen de un contexto del &quot;mundo real&quot;, sin proporcionar un razonamiento adicional por qué los elementos seleccionados son adecuados para el contexto del estudio

## Críticas Inválidas

- complaining about lack of representativeness or low external validity in studies where representativeness is not a goal
- abstractly criticizing generalizability rather than pointing to best practices, e.g.:
- invalid: &#39;as most respondents work in app development, the results may not generalize to other settings&#39;
- valid: &#39;the researchers should have sent participation reminders to mitigate response bias&#39;
- for qualitative research, claiming that the sample size is too small without considering how the items were selected (e.g. theoretical sampling) or the authors&#39; argument for saturation.

- Quejarse de la falta de representatividad o baja validez externa en estudios donde la representatividad no es un objetivo
- Criticar de forma abstracta la generalización en lugar de apuntar a las mejores prácticas, por ejemplo:
- Inválido: &#39;dado que la mayoría de los encuestados trabaja en el desarrollo de aplicaciones, es posible que los resultados no se generalicen a otras configuraciones&#39;
- Válido: &#39;los investigadores deberían haber enviado recordatorios de participación para mitigar el sesgo de respuesta&#39;
- Para la investigación cualitativa, alegar que el tamaño de la muestra es demasiado pequeño sin tener en cuenta cómo se seleccionaron los elementos (por ejemplo, muestreo teórico) o el argumento de los autores a favor de la saturación.

## Lecturas Sugeridas

Sebastian Baltes and Paul Ralph. 2020. Sampling in Software Engineering Research: A Critical Review and Guidelines. _arXiv_. [https://arxiv.org/abs/2002.07764](https://arxiv.org/abs/2002.07764)

William G. Cochran. 2007. Sampling techniques. _Wiley_.

Steve Easterbrook, Janice Singer, Margaret-Anne Storey, and Daniela Damian. 2008. Selecting Empirical Methods for Software Engineering Research. In _Guide to Advanced Empirical Software Engineering_. 285-311.

Barbara Kitchenham and Shari Lawrence Pfleeger. 2002. Principles of survey research: part 5: populations and samples. SIGSOFT Softw. Eng. Notes 27, 5 (September 2002), 17–20. DOI:10.1145/571681.571686

Gary T. Henry. 1990. _Practical sampling._ Sage 21.

Meiyappan Nagappan, Thomas Zimmermann, and Christian Bird. 2013. Diversity in software engineering research. In _Proceedings of the 2013 9th Joint Meeting on Foundations of Software Engineering (ESEC/FSE 2013)_. Association for Computing Machinery, New York, NY, USA, 466–476. DOI:10.1145/2491411.2491415

---
<sup>[1](#myfootnote1)</sup> Los effect size esperados deben ser plausibles. Por ejemplo, esperar que un solo factor (por ejemplo, lenguaje de programación) explique el 50% de la variación en el éxito del proyecto de software no es plausible.

