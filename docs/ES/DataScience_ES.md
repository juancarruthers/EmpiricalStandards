# Ciencia de Datos
<standard name="Data Science">

<desc>Estudios que analizan fenómenos o artefactos de la Ingeniería de Software utilizando métodos de análisis centrados en datos como el aprendizaje automático u otras aplicaciones de inteligencia computacional, así como enfoques basados en búsquedas.<footnote></desc><sup>[1](#myfootnote1)</sup>

## Aplicación

Se aplica a estudios que analizan principalmente los fenómenos de software existentes utilizando modelos predictivos, preventivos o correctivos.

- Si el análisis se enfoca en el kit de herramientas, en lugar de conclusiones nuevas generadas por el kit de herramientas, considere el **Estándar de Artefactos**
- Si el análisis se centra en un único entorno rico en contexto (por ejemplo, un análisis detallado de un único repositorio), considere el **Estándar de Estudio de Caso**.
- Si se analiza la dimensión temporal considere el **Estándar de Estudios Longitudinales**.
- Si los objetos de datos son discusiones o mensajes entre humanos, considere el **Estándar de Análisis del Discurso**.
- Si se utilizan visualizaciones de datos, considere el **Suplemento de Visualización de Información**. (Especialmente con grandes conjuntos de datos, se debe tener cuidado para mantener legibles las visualizaciones).
- Si el análisis selecciona un subconjunto de datos disponibles, consulte el **Suplemento de Muestreo**.


## Atributos Específicos

### Atributos Esenciales
<checklist name="Essential">
	
<intro>

- [ ] Explica por qué es oportuno investigar el problema propuesto utilizando el método propuesto.

<method>

- [ ] Explica cómo y por qué se seleccionaron los datos.
- [ ] Presenta la configuración experimental (por ejemplo, usando un diagrama de flujo de datos)<sup>[2](#myfootnote2)</sup>
- [ ] Describe los enfoques de ingeniería de características<sup>[3](#myfootnote3)</sup> y transformaciones que se aplicaron.
- [ ] Explica cómo se preprocesaron, filtraron y categorizaron los datos.
- [ ] O BIEN: discute las bases del estado del arte (y sus fortalezas, debilidades y limitaciones)
	O: explica por qué no existen líneas de base de última generación
	O: proporciona un argumento convincente de que las comparaciones directas no son prácticas.
- [ ] Define los enfoques de modelado utilizados (por ejemplo, agrupación y luego aprendizaje de árbol de decisiones), por lo general utilizando pseudocódigo.
- [ ] Analiza la infraestructura de hardware y software utilizada.<sup>[4](#myfootnote4)</sup>
- [ ] Justifica todas las estadísticas y heurísticas (automáticas o manuales) utilizadas. 
- [ ] Describe y justifica las métricas de evaluación utilizadas.	

<results>

- [ ] Va más allá de los resúmenes unidimensionales de desempeño (por ejemplo, promedio, mediana) para incluir medidas de variación, confianza u otra información de distribución

<discussion>

- [ ] Analiza los supuestos técnicos y las amenazas a la validez que son específicas de la ciencia de datos<sup>[5](#myfootnote5)</sup>
	
<other>

</checklist>

### Atributos Deseables
<checklist name="Desirable">

- [ ] Proporciona un paquete de replicación que incluye código fuente y conjuntos de datos, o si los datos no se pueden compartir, datos sintéticos para ilustrar el uso de los algoritmos<sup>[6](#myfootnote6)</sup>
- [ ] Los datos son procesados por múltiples aprendices, de diferentes tipos<sup>[7](#myfootnote7)</sup>
- [ ] Los datos se procesan varias veces con diferentes ejemplos de entrenamiento/prueba seleccionados al azar; cuyos resultados se comparan mediante pruebas de significación y pruebas de tamaño del efecto (por ejemplo, validación cruzada)
- [ ] Selecciona cuidadosamente los hiperparámetros que controlan los mineros de datos (por ejemplo, a través del análisis de la configuración en el trabajo relacionado o algún optimizador automático de hiperparámetros como la búsqueda de cuadrícula)
- [ ] Inspecciona manualmente una parte no trivial de los datos (es decir, verificaciones de la integridad de los datos)
- [ ] Distingue claramente los resultados basados en la evidencia de las interpretaciones y la especulación<sup>[8](#myfootnote8)</sup>
</checklist>

### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Aprovecha los datos temporales a través de análisis longitudinales (consulte el [Estándar de Estudios Longitudinales](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/Longitudinal.md))
- [ ] Triangula con análisis de datos cualitativos de muestras seleccionadas de los datos.
- [ ] Triangula con otras fuentes de datos, como encuestas o entrevistas.
- [ ] Comparte hallazgos y solicita comentarios de los creadores de los artefactos (de software) que se están estudiando.
</checklist>

## Ejemplos de Desviaciones Aceptables

- Usar un procesamiento de datos más ligero y menos preciso (por ejemplo, concordancia de palabras clave o submuestreo aleatorio) si la escala de datos es demasiado grande para que un análisis preciso sea práctico.
- Los datos no se comparten porque no son prácticos (por ejemplo, demasiado grandes) o poco éticos (por ejemplo, demasiado sensibles). Debe ofrecerse suficiente información para asegurar al lector que los datos son reales.
- No utilizar técnicas de análisis temporal, como series de tiempo, cuando los datos no se convierten fácilmente en series de tiempo (por ejemplo, algunos aspectos de la evolución del código fuente pueden no modelarse fácilmente como series de tiempo).
- No todos los estudios necesitan estadísticas e hipótesis. Algunos estudios pueden ser pura o principalmente descriptivos.
- Diferentes explicaciones tienen diferentes requisitos (por ejemplo, conjuntos de espera, validación cruzada)<sup>[9](#myfootnote9)</sup>.

## Antipatrones

- Utilizar pruebas estadísticas sin comprobar sus supuestos.
- Usar estadísticas bayesianas sin motivar a priori.
- Afirmar causalidad no solo sin establecer la covariación y la precedencia, sino también eliminar las explicaciones de la tercera variable y al menos plantear la hipótesis de un mecanismo generativo.
- El procesamiento previo modifica datos de entrenamiento y datos de prueba; p.ej. Si bien puede ser útil ajustar las distribuciones de clases de datos de entrenamiento a través de (por ejemplo) submuestreo de clases mayoritarias, ese ajuste no debe aplicarse a los datos de prueba (ya que es importante evaluar al aprendiz sobre los tipos de datos que pueden encontrarse "en la naturaleza").
- Recopilación o análisis poco éticos de datos (consulte el [Suplemento de Ética (Datos Secundarios)](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/EthicsSecondaryData.md)
- Pruebas de significación sin pruebas de tamaño del efecto; tamaños del efecto sin intervalos de confianza.
- Informar una mediana, sin ninguna indicación de varianza (por ejemplo, un diagrama de caja).
- Realización de múltiples ensayos sin informar variaciones entre ensayos.

## Críticas Inválidas

- Se deberían haber analizado los datos ABC. La pregunta que los revisores deben hacerse es si las afirmaciones principales del artículo están respaldadas por los datos que se analizaron, no si algunos otros datos hubieran sido mejores.
- No tiene paquete de reproducción. Estos son deseables, no esenciales (todavía).
- Los resultados no son procesables: no todos los estudios pueden tener resultados directamente procesables a corto plazo.
- "Necesita más datos" como crítica genérica sin una razón clara y justificada.
- El estudio no utiliza datos cualitativos.
- El estudio no hace afirmaciones causales cuando no puede.
- El estudio no utiliza la fuente de datos más precisa, a menos que la fuente de datos sea claramente problemática para el estudio en cuestión. No es práctico recopilar algunos datos a escala. 

## Lecturas Sugeridas

1. Hemmati, Hadi, et al. "The msr cookbook: Mining a decade of research." 2013 10th Working Conference on Mining Software Repositories (MSR). IEEE, 2013.
2. Robles, Gregorio, and Jesus M. Gonzalez-Barahona. "Developer identification methods for integrated data from various sources." (2005).
3. Dey, Tapajit, et al. "Detecting and Characterizing Bots that Commit Code." arXiv preprint arXiv:2003.03172 (2020).
4. Hora, Andre, et al. "Assessing the threat of untracked changes in software evolution." Proceedings of the 40th International Conference on Software Engineering. 2018.
5. Herzig, Kim, and Andreas Zeller. "The impact of tangled code changes." 2013 10th Working Conference on Mining Software Repositories (MSR). IEEE, 2013.
6. Berti-Équille, L. (2007). Measuring and Modelling Data Quality for Quality-Awareness in Data Mining.. In F. Guillet & H. J. Hamilton (ed.), Quality Measures in Data Mining , Vol. 43 (pp. 101-126) . Springer . ISBN: 978-3-540-44911-9.
7. Wohlin, C., Runeson, P., Höst, M., Ohlsson, M. C.,, Regnell, B. (2012). Experimentation in Software Engineering.. Springer. ISBN: 978-3-642-29043-5Wohlin’ standard thrrs
8.  Raymond P. L. Buse and Thomas Zimmermann. 2012. Information needs for software development analytics. In Proceedings of the 34th International Conference on Software Engineering (ICSE '12). IEEE Press, 987–996.
9.  https://aaai.org/Conferences/AAAI-21/reproducibility-checklist/
10.  Baljinder Ghotra, Shane McIntosh, and Ahmed E. Hassan. 2015. Revisiting the impact of classification techniques on the performance of defect prediction models. In Proceedings of the 37th International Conference on Software Engineering - Volume 1 (ICSE '15). IEEE Press, 789–800.
11.  Daniel Russo and Klaas-Jan Stol. In press. PLS-SEM for Software Engineering Research: An Introduction and Survey. *ACM Computing Surveys*.  

## Ejemplares

1. A. Barua, S. W. Thomas, A. E. Hassan, What are developers talkingabout? an analysis of topics and trends in stack overflow, Empirical Software Engineering 19 (3) (2014) 619–654.
2. Bird, C., Rigby, P. C., Barr, E. T., Hamilton, D. J., German, D. M., & Devanbu, P. (2009, May). The promises and perils of mining git. In 2009 6th IEEE International Working Conference on Mining Software Repositories (pp. 1-10). IEEE.
3. Kalliamvakou, E., Gousios, G., Blincoe, K., Singer, L., Germán, D. M. & Damian, D. E. (2014). The promises and perils of mining GitHub.. In P. T. Devanbu, S. Kim & M. Pinzger (eds.), MSR (p./pp. 92-101), : ACM. ISBN: 978-1-4503-2863-0
4. Herbsleb, J. & Mockus, A. (2003). An Empirical Study of Speed and Communication in Globally Distributed Software Development. IEEE Transactions on Software Engineering, 29, 481-94.2
4. Menzies, T., Greenwald, J., & Frank, A. (2006). Data mining static code attributes to learn defect predictors. IEEE transactions on software engineering, 33(1), 2-13.
5. Menzies, T., & Marcus, A. (2008, September). Automated severity assessment of software defect reports. In 2008 IEEE International Conference on Software Maintenance (pp. 346-355). IEEE.
6. Nair, V., Agrawal, A., Chen, J., Fu, W., Mathew, G., Menzies, T., Minku, L. L., Wagner, M. & Yu, Z. (2018). Data-driven search-based software engineering.. In A. Zaidman, Y. Kamei & E. Hill (eds.), MSR (p./pp. 341-352), : ACM.
7. Rahman, F., & Devanbu, P. (2013, May). How, and why, process metrics are better. In 2013 35th International Conference on Software Engineering (ICSE) (pp. 432-441). IEEE.
8. Tufano, M., Palomba, F., Bavota, G., Oliveto, R., Penta, M. D., Lucia, A. D. & Poshyvanyk, D. (2017). When and Why Your Code Starts to Smell Bad (and Whether the Smells Go Away).. IEEE Trans. Software Eng., 43, 1063-1088.

---
<footnote><sup>[1](#myfootnote1)</sup>Dhar, V. (2013). Data Science and Prediciton, Communications of the ACM, December 2013, Vol. 56 No. 12, Pages 64-73. https://cacm.acm.org/magazines/2013/12/169933-data-science-and-prediction/fulltext</footnote> 
<br>
<footnote><sup>[2](#myfootnote2)</sup>Akidau, Tyler, Robert Bradshaw, Craig Chambers, Slava Chernyak, Rafael J. Fernández-Moctezuma, Reuven Lax, Sam McVeety et al. "The dataflow model: a practical approach to balancing correctness, latency, and cost in massive-scale, unbounded, out-of-order data processing." (2015). Proceedings of the VLDB Endowment 8.12</footnote>
<br>
<footnote><sup>[3](#myfootnote3)</sup>Acf. Nargesian, Fatemeh, Horst Samulowitz, Udayan Khurana, Elias B. Khalil, and Deepak S. Turaga. "Learning Feature Engineering for Classification." In Ijcai, pp. 2529-2535. 2017.</footnote>
<br>
<footnote><sup>[4](#myfootnote4)</sup>incluidos los modelos de GPU/CPU; cantidad de memoria; sistema operativo; nombres y versiones de bibliotecas de software y frameworks relevantes</footnote>
<br>
<footnote><sup>[5](#myfootnote5)</sup>Por ejemplo, no abordar las variaciones del tamaño o la complejidad de los conjuntos de datos de capacitación, prueba y validación. Para más información, vea: Wohlin, C., Runeson, P., Höst, M., Ohlsson, M. C.,,Regnell, B. (2012). Experimentation in Software Engineering. Springer. ISBN: 978-3-642-29043-5</footnote>
<br>	
<footnote><sup>[6](#myfootnote6)</sup>Sarkar, T. (2019). Synthetic data generation - a must-have skill for new data scientists. (July 2019).https://towardsdatascience.com/synthetic-data-generation-a-must-have-skill-for-new-data-scientists-915896c0c1ae</footnote>
<br> 
<footnote><sup>[7](#myfootnote7)</sup>p.ej. regresión, clasificador de Bayes, árbol de decisión, bosques aleatorios, SVM (tal vez con diferentes núcleos); para obtener orientación, consulte Baljinder Ghotra, Shane McIntosh, and Ahmed E. Hassan. 2015. Revisiting the impact of classification techniques on the performance of defect prediction models. In Proceedings of the 37th International Conference on Software Engineering - Volume 1 (ICSE '15). IEEE Press, 789–800.</footnote>
<br>
<footnote><sup>[8](#myfootnote8)</sup>Por lo general, basta con separar los resultados y la discusión en diferentes secciones. Sin especulaciones en la sección de resultados.</footnote>
<br>
<footnote><sup>[9](#myfootnote9)</sup>c.f. Raymond P. L. Buse and Thomas Zimmermann. 2012. Information needs for software development analytics. In Proceedings of the 34th International Conference on Software Engineering (ICSE '12). IEEE Press, 987–996.</footnote>
<br>
</standard>
