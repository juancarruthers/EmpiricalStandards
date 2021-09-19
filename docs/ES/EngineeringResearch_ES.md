# Investigación en Ingeniería (Alias Diseño Científico)
<standard name="Engineering Methods">

*Investigación que idea, diseña y evalúa artefactos tecnológicos*

## Aplicación

Este estándar se aplica a estudios que proponen y evalúan artefactos tecnológicos, incluidos algoritmos, modelos, lenguajes, métodos, sistemas, herramientas y otras tecnologías basadas en ciencias de la computación. Este estándar no es apropiado para:

-   Evaluaciones de enfoques de investigación de ingeniería preexistentes (considere el estándar de **Experimentos**)
-   Informes de experiencia de la aplicación de enfoques de investigación de ingeniería preexistentes

## Atributos específicos

### Atributos esenciales
<checklist name="Essential">

<intro>
- [ ]   Describe el artefacto propuesto con suficiente detalle<sup>[1](#myfootnote1)</sup>
- [ ]   Justifica la necesidad, utilidad o relevancia del artefacto propuesto<sup>[2](#myfootnote2)</sup>
- [ ]   Evalúa conceptualmente el artefacto propuesto; analiza sus fortalezas, debilidades y limitaciones<sup>[3](#myfootnote3)</sup>

<method>

- [ ]   Evalúa empíricamente el artefacto propuesto utilizando:
  [Investigación-Acción](https://github.com/juancarruthers/EmpiricalStandards/blob/master/docs/ActionResearch.md), en la que los investigadores intervienen en una organización real utilizando el artefacto,
  Un [Estudio de Caso](https://github.com/juancarruthers/EmpiricalStandards/blob/master/docs/CaseStudy.md) en el que los investigadores observan una organización real que utiliza el artefacto,
  Un [Experimento Controlado](https://github.com/juancarruthers/EmpiricalStandards/blob/master/docs/Experiments.md) en el que los participantes humanos utilizan el artefacto,
  Una [Simulación Cuantitativa](https://github.com/juancarruthers/EmpiricalStandards/blob/master/docs/QuantitativeSimulation.md) en la que se evalúa el artefacto (generalmente contra un artefacto competidor) en un entorno artificial,
  Un [Benchmarking](https://github.com/juancarruthers/EmpiricalStandards/blob/master/docs/Benchmarking.md), en el que el artefacto se evalúa utilizando uno o más parámetros de referencia, u otro método para el que se proporciona una justificación clara y convincente.
- [ ]   Indica claramente cuál de las metodologías empíricas anteriores se utiliza
- [ ]   O BIEN: Discute alternativas del estado del arte (y sus fortalezas, debilidades y limitaciones)
    O: Explica por qué no existen alternativas de estado del arte
    O: Proporciona un argumento convincente de que las comparaciones directas no son prácticas
- [ ]   O BIEN: Compara empíricamente el artefacto con una o más alternativas del estado del arte
    O: Compara empíricamente el artefacto con uno o más valores de referencia (benchmark) del estado del arte
    O: Proporciona una justificación clara y convincente de por qué la evaluación comparativa no es práctica

<results>


<discussion>


<other>

- [ ]   Las suposiciones (si las hay) son explícitas, plausibles y no se contradicen entre sí ni con los objetivos de la contribución.
- [ ]   Usa la notación de manera consistente (si se usa alguna notación)

</checklist>

### Atributos deseables
<checklist name="Desirable">

- [ ]   Proporciona materiales complementarios, incluido el código fuente (si el artefacto es software) o una descripción completa del artefacto (si no es software), y cualquier conjunto de datos de entrada (si corresponde)
- [ ]   Justifica los elementos que faltan en el paquete de replicación basándose en motivos prácticos o éticos
- [ ]   Discute la base teórica del artefacto
- [ ]   Proporciona argumentos de corrección para las contribuciones analíticas y teóricas clave (por ejemplo, teoremas, análisis de complejidad, pruebas matemáticas)
- [ ]   Incluye uno o más ejemplos en ejecución para dilucidar el artefacto
- [ ]   Evalúa el artefacto en un contexto industrial relevante (por ejemplo, proyectos de código abierto ampliamente utilizados, con programadores experimentados)

</checklist>
    
### Atributos extraordinarios
<checklist name="Extraordinary">

- [ ]   Contribuye a nuestra comprensión colectiva de las prácticas o principios de diseño
- [ ]   Presenta innovaciones revolucionarias con obvios beneficios en el mundo real
</checklist>
    
## Criterios generales de calidad

-   Exhaustividad de la descripción del artefacto propuesto
-   Adecuación de los métodos de evaluación a la naturaleza, metas y supuestos de la contribución.
-   Relación de la innovación con la rigurosidad: los artefactos menos innovadores requieren evaluaciones más rigurosas

## Antipatrones

-   Exagera la novedad de la contribución
-   Omite detalles de aspectos conceptuales clave mientras se enfoca exclusivamente en aspectos de implementación incidentales
-   La evaluación consiste *solo* en obtener las opiniones de los usuarios sobre el artefacto.
-   La evaluación consiste *solo* en datos de desempeño cuantitativos que no se comparan con puntos de referencia establecidos o soluciones alternativas (consulte el punto relacionado en "Críticas Inválidas")

## Críticas Inválidas

-   El artículo no presenta un estudio empírico tan ambicioso como otros artículos predominantemente empíricos. Cuanto más innovador sea el artefacto y más completa sea la evaluación conceptual, menos debemos esperar del estudio empírico.
-   Muy pocos sujetos experimentales (por ejemplo, el código fuente utilizado para evaluar una técnica de análisis estático) si hay pocos sujetos disponibles en el dominio de la contribución o la evaluación experimental es parte de una estrategia de validación más completa (por ejemplo, argumentos formales). Otros criterios, como la variedad, el realismo, la disponibilidad y la escala de los temas, también deben considerarse para evaluar la calidad de la evaluación.
-   Ningún paquete de replicación, si existen razones prácticas o éticas claras y convincentes que impidan la divulgación del artefacto.
-   El artefacto no se compara experimentalmente con enfoques relacionados que *no están disponibles públicamente*. En otras palabras, antes de decir “debería haber comparado esto con X, asegúrese de que X esté realmente disponible y sea funcional.
-   Ésta no es la primera solución conocida al problema identificado. La novedad del artículo puede estar en cómo logra escalabilidad, mejor desempeño en clases específicas de problemas, aplicabilidad a sistemas realistas, garantías teóricas más sólidas u otros aspectos de mejora. Los artefactos propuestos deben superar a los artefactos existentes *en una o más dimensiones pero no necesariamente en todas*.
-   La contribución no es técnicamente complicada. Lo que importa es que funciona. La complejidad innecesaria es indeseable.

### Lecturas sugeridas <sup>[4](#myfootnote4)</sup>

Richard Baskerville, Jan Pries-Heje, and John Venable. 2009. Soft design
science methodology. In *Proceedings of the 4th International Conference
on Design Science Research in Information Systems and Technology
(DESRIST '09).* Association for Computing Machinery, New York, NY, USA,
Article 9, 1–11. DOI: 10.1145/1555619.1555631

Carlo Ghezzi. 2020. *Being a researcher - an informatics perspective*.
Springer Nature.

Alan Hevner and Samir Chatterjee. 2010. *Design Research in Information
Systems*. Integrated Series in Information Systems. Springer, 22, (Mar.
2010), 145–156. DOI:
[10.1007/978-1-4419-5653-8_11](https://doi.org/10.1007/978-1-4419-5653-8_11)

Alan R. Hevner, Salvatore T. March, Jinsoo Park and Sudha Ram. 2004.
Design Science in Information Systems Research. *MIS Quarterly*, 28, 1
(Mar. 2004), 75–105. DOI:10.2307/25148625.

Roel Wieringa. 2014. *Design science methodology for information systems
and software engineering.* Springer*.*

## Ejemplares

Kihong Heo, Hakjoo Oh and Hongseok Yang. 2019. Resource-aware Program
Analysis via Online Abstraction Coarsening. In *Proceedings of the 41st
International Conference on Software Engineering.*

Jianhui Chen, Fei He. 2018. Control Flow-Guided SMT Solving for Program
Verification. In *Proceedings of the 33rd International Conference on
Automated Software Engineering*.

Calvin Loncaric, Michael D. Ernst and Emina Torlak. 2018. Generalized
Data Structure Synthesis. In *Proceedings of the 40th International
Conference on Software Engineering.*

Nikolaos Tsantalis, Davood Mazinanian and Shahriar Rostami Dovom. 2017.
Clone Refactoring with Lambda Expressions. In *Proceedings of the 39th
International Conference on Software Engineering.*

August Shi, Suresh Thummalapenta, Shuvendu Lahiri, Nikolaj Bjorner and
Jacek Czerwonka. (2017) Optimizing Test Placement for Module-Level
Regression Testing. In *Proceedings of the 39th International Conference
on Software Engineering.*

Magnus Madsen, Frank Tip, Esben Andreasen, Koushik Sen, and Anders
Møller. 2016. Feedback-Directed Instrumentation for Deployed JavaScript
Applications. In *Proceedings of the 38th International Conference on
Software Engineering.*

---
<footnote><sup>[1](#myfootnote1)</sup> Por ejemplo, ¿describe el documento el flujo de trabajo general de la solución, mostrando cómo las diferentes técnicas funcionan juntas? ¿Se presentan las contribuciones algorítmicas de forma inequívoca? ¿Se presentan explícitamente las partes clave de un modelo formal? ¿Se destacan claramente los componentes novedosos de la solución?</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup> Es decir, ¿el problema que el enfoque propuesto intenta resolver es específico de un determinado dominio? Si es así, ¿por qué? ¿Por qué los otros enfoques o intentos de solución encontrados en el estado del arte no son lo suficientemente buenos para abordar el problema? ¿Cómo puede ser beneficiosa la contribución técnica?</footnote><br>
<footnote><sup>[3](#myfootnote3)</sup> Por ejemplo, complejidad temporal de un algoritmo; teórico.</footnote><br>
<footnote><sup>[4](#myfootnote4)</sup>  Nota: El aprendizaje mediante la construcción de artefactos innovadores se denomina Investigación en Ingeniería. Algunas de las siguientes lecturas se refieren incorrectamente a la Investigación en Ingeniería como "Design Science" porque la comunidad de sistemas de información se apropió indebidamente de ese término alrededor de 2004. El "design sciense" se ha referido al estudio de los diseñadores y sus procesos desde al menos la década de 1940, y todavía lo hace fuera de la comunidad de sistemas de información.</footnote><br>
</standard>