# Minado de Repositorios
<standard name="Repository Mining">   



*<desc>Un estudio que analiza cuantitativamente un conjunto de datos extraído de una plataforma que aloja texto estructurado o semiestructurado (por ejemplo, un repositorio de código fuente)</desc>*    
                                                                                                                                                                                               
                                                                                                                                                                                                
    
## Aplicación    
    
El estándar se aplica a los estudios de ingeniería de software que:
    - Utilizan técnicas automatizadas para extraer datos de repositorios de datos a gran escala, como repositorios de código fuente, archivos de listas de correo, sistemas de seguimiento de bugs, foros de preguntas y respuestas, y plataformas de comunicación por chat
    - Analizan cuantitativamente los contenidos extraídos de los repositorios

Si el estudio se centra en el modelado predictivo (p. ej., aprendizaje automático), considere el **Estándar de Ciencia de Datos**. Si los sujetos (sistemas) son unos pocos repositorios ricos en contexto, considere el **Estándar de estudio de caso**. Si el análisis es predominantemente cualitativo, consulte las pautas metodológicas para el análisis de contenido cualitativo o el análisis del discurso (estándar por determinar).     

## Atributos Específicos

### Atributos Esenciales
<checklist name="Essential">
    
<intro>

- [ ] Explica porque el minado de repositorios es apropiado para el problema propuesto

<method>
    
- [ ] Define unidad(es) de análisis u observación
- [ ] Describe y justifica las fuentes de datos (por ejemplo, GitHub, StackOverflow)
    - (Si las fuentes de datos seleccionadas son opacas) explica en detalle por qué son apropiadas para los objetivos del estudio (p. ej., considere la cantidad de repositorios, la calidad de los datos, los términos y condiciones que pueden limitar el acceso a la información)
- [ ] Describe y justifica cómo se seleccionan los repositorios de las fuentes de datos (por ejemplo, criterios de selección, uso de herramientas de terceros, APIs, lenguajes de programación de elección)
- [ ] Describe cómo se validaron los criterios de inclusión y exclusión (p. ej., inspeccionando manualmente los resultados de la búsqueda automática)
- [ ] Describe los repositorios seleccionados
- [ ] Describe el procedimiento para la adquisición (por ejemplo, primero seleccionando repositorios y luego descargando, o completando todos juntos)
- [ ] Si los datos obtenidos son demasiado grandes para ser procesados en su totalidad
    - Explica por qué (por ejemplo, inviabilidad de un estudio manual, limitaciones de procesamiento, limitaciones de alcance)
    - Explica la estrategia de muestreo (consulte el [Suplemento de muestreo](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/Sampling.md))
- [ ] Describe las características del conjunto de datos, incluido el tamaño de los repositorios seleccionados y los atributos del conjunto de datos relevantes para el estudio en cuestión (p. ej., número de commits)
- [ ] Describe los pasos de preprocesamiento de datos
- [ ] Si se realizan anotaciones manuales:
    - Utiliza múltiples anotadores; informa el número de anotadores
    - Describe los anotadores (por ejemplo, datos demográficos, experiencia, formación),
    - Describe en detalle el procedimiento de anotación (por ejemplo, qué tipo de preguntas se hicieron a los anotadores),
    - Evalúa la confiabilidad entre evaluadores (consulte el Suplemento de confiabilidad entre evaluadores)
- [ ] Describe y justifica las medidas o métricas utilizadas
- [ ] SI: utiliza medidas previamente validadas, O BIEN: evalúa la validez del constructo

- [ ] Si se usa modelado predictivo, cumple con el [Estandar de ciencia de datos](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/DataScience.md)    

<results>
    
<discussion>
    
- [ ] Analiza las amenazas a la validez externa (por ejemplo, ocasionados por la selección de fuentes de datos y repositorios, criterios de selección o cadenas de búsqueda)

<other>

</checklist>

### Atributos Deseables
<checklist name="Desirable">

- [ ] Proporciona materiales complementarios (p. ej., conjunto de datos completo, herramientas utilizadas para descargar, seleccionar, pre-procesar y post-procesar los repositorios seleccionados)
- [ ] Utiliza el muestreo probabilístico (consulte el [Suplemento de muestreo](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/Sampling.md))
- [ ] Sugiere trabajo futuro que valide o use la misma muestra
- [ ] Evalúa cuantitativamente la validez del constructo (p. ej., utilizando el análisis factorial)
- [ ] Triangula a través de fuentes de datos, informantes o investigadores
- [ ] Los anotadores reflexionan sobre sus propios posibles sesgos
- [ ] Análisis cualitativo de escenarios en los que las herramientas de recopilación o análisis de datos fueron ineficaces
- [ ] Realiza pruebas (por ejemplo, pruebas unitarias) para evitar bugs en la herramienta propuesta
- [ ] Construye, prueba o amplía la teoría
- [ ] Prueba hipótesis formales
- [ ] Analiza cuestiones éticas en el minado de repositorios de software<sup>[1](#footnote1)</sup> (p. ej., privacidad de datos)  
    
</checklist>

### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Establece causalidad, por ejemplo, usando análisis longitudinal

</checklist>

## Criterios Generales de Calidad
Validez interna, validez externa, validez del constructo, fiabilidad.

## Ejemplos de Desviaciones Aceptables
- Estudios que se centran en ecosistemas específicos (como Apache) pueden elegir repositorios específicos
- Ocultar algunos detalles del conjunto de datos debido a preocupaciones éticas

## Antipatrones
- Limitar un estudio a la descripción cuantitativa; no probar, construir o extender la teoría
- Operacionalización unidimensional de construcciones multidimensionales no validadas (por ejemplo, usar estrellas de github como proxy de popularidad)
- Usar repositorios de código abierto sin ningún criterio de filtrado; es decir, muestreo por conveniencia<sup>[2](#footnote2)</sup>.
- En un estudio donde se deben analizar *todos* los commits de un proyecto, solo se considera el repositorio de GitHub; un repositorio de GitHub no contiene necesariamente todos los commits de un proyecto<sup>[3](#footnote3)</sup>.
- Las conclusiones deben derivarse en el contexto de los repositorios seleccionados; derivar conclusiones genéricas aplicables a los repositorios seleccionados pero necesariamente a un conjunto genérico más grande es un antipatrón
- Detalles insuficientes sobre los pasos de procesamiento aplicados a los repositorios seleccionados

## Críticas Inválidas
- Se requieren más datos, fuentes o repositorios sin la justificación adecuada
- El estudio no utiliza análisis o datos cualitativos
- Se debería haber utilizado una fuente diferente cuando las fuentes seleccionadas están justificadas
- Quejarse de la ocultación intencional de los detalles del repositorio para proteger las identidades de los participantes
- En los estudios manuales, exigir la divulgación del tiempo necesario para su realización


## Lecturas Sugeridas
- Daniel Barros, Flavio Horita, Igor Wiese, and Kanan Silva. 2021. A Mining Software Repository Extended Cookbook: Lessons learned from a literature review. In Brazilian Symposium on Software Engineering (SBES '21).
- Weiyi Shang, Bram Adams, and Ahmed E. Hassan. 2010. An experience report on scaling tools for mining software repositories using MapReduce. In Proceedings of the IEEE/ACM international conference on Automated software engineering (ASE '10).
- V. Cosentino, J. L. C. Izquierdo and J. Cabot, "Findings from GitHub: Methods, Datasets and Limitations," 2016 IEEE/ACM 13th Working Conference on Mining Software Repositories (MSR), 2016, pp. 137-141.
- Munaiah, N., Kroh, S., Cabrey, C. et al. Curating GitHub for engineered software projects. Empir Software Eng 22, 3219–3253 (2017).
- Sebastian Baltes, Paul Ralph. 2021. Sampling in Software Engineering Research: A Critical Review and Guidelines. arXiv eprint 2002.07764.
- Eirini Kalliamvakou, Georgios Gousios, Kelly Blincoe, Leif Singer, Daniel M. German, and Daniela Damian. 2014. The promises and perils of mining GitHub. In Proceedings of the 11th Working Conference on Mining Software Repositories (MSR 2014).
- A. E. Hassan, "The road ahead for Mining Software Repositories," 2008 Frontiers of Software Maintenance, 2008, pp. 48-57.
- V. Thakur, M. Kessentini and T. Sharma, "QScored: An Open Platform for Code Quality Ranking and Visualization," 2020 IEEE International Conference on Software Maintenance and Evolution (ICSME), 2020, pp. 818-821.
- Georgios Gousios. 2013. The GHTorent dataset and tool suite. In Proceedings of the 10th Working Conference on Mining Software Repositories (MSR '13). IEEE Press, 233–236.
- Gold, N.E., Krinke, J. Ethics in the mining of software repositories. Empirical Software Engineering 27, 17 (2022). https://doi.org/10.1007/s10664-021-10057-7
- Vidoni, M., A Systematic Process for Mining Software Repositories: Results From a Systematic Literature Review. Information and Software Technology 144 (2022). https://doi.org/10.1016/j.infsof.2021.106791

## Ejemplares
- M. Beller, G. Gousios and A. Zaidman, "Oops, My Tests Broke the Build: An Explorative Analysis of Travis CI with GitHub," 2017 IEEE/ACM 14th International Conference on Mining Software Repositories (MSR), 2017, pp. 356-367.
- Georgios Gousios, Eirini Kalliamvakou, and Diomidis Spinellis. 2008. Measuring developer contribution from software repository data. In Proceedings of the 2008 international working conference on Mining software repositories (MSR '08).
- Moritz Beller, Alberto Bacchelli, Andy Zaidman, and Elmar Juergens. 2014. Modern code reviews in open-source projects: which problems do they fix? In Proceedings of the 11th Working Conference on Mining Software Repositories (MSR 2014).
- Davide Spadini, Maurício Aniche, and Alberto Bacchelli. 2018. PyDriller: Python framework for mining software repositories. In Proceedings of the 2018 26th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2018).
- M. Ortu, B. Adams, G. Destefanis, P. Tourani, M. Marchesi and R. Tonelli, "Are Bullies More Productive? Empirical Study of Affectiveness vs. Issue Fixing Time," 2015 IEEE/ACM 12th Working Conference on Mining Software Repositories, 2015, pp. 303-313.

---
<footnote><sup>[1](#footnote1)</sup>Gold, N.E., Krinke, J. Ethics in the mining of software repositories. Empir Software Eng 27, 17 (2022). https://doi.org/10.1007/s10664-021-10057-7</footnote><br>
<footnote><sup>[2](#footnote2)</sup>Sebastian Baltes, Paul Ralph. 2021. Sampling in Software Engineering Research: A Critical Review and Guidelines. arXiv eprint 2002.07764.</footnote><br>
<footnote><sup>[3](#footnote3)</sup>Eirini Kalliamvakou, Georgios Gousios, Kelly Blincoe, Leif Singer, Daniel M. German, and Daniela Damian. 2014. The promises and perils of mining GitHub. In Proceedings of the 11th Working Conference on Mining Software Repositories (MSR 2014).</footnote><br>


</standard>
