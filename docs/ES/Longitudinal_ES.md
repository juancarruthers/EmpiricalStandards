# Estudios Longitudinales
<standard name="Longitudinal">

*Un estudio centrado en los cambios y la evolución de un fenómeno a lo largo del tiempo*

## Aplicación

Este estándar se aplica a estudios que involucran observaciones repetidas de las mismas variables (por ejemplo, productividad o deuda técnica) durante un período de tiempo. Los estudios longitudinales incluyen el análisis de conjuntos de datos a lo largo del tiempo, como el análisis de la evolución del código. Los estudios longitudinales requieren mantener la identificabilidad de los sujetos (humanos o artefactos) entre los momentos de recopilación de datos y utilizar al menos dos momentos de recopilación.

Para el análisis transversal, considere el **Estándar de Ciencia de Datos Exploratorios** o el **Estándar de Experimentos** (si se manipulan las variables).

## Atributos Específicos

### Atributos Esenciales 
<checklist name="Essential">
    
<intro>

<method>
    
- [ ] Determina el número apropiado de momentos de recolección según la oscilación natural del fenómeno de investigación<sup>[1](#myfootnote1)</sup>
- [ ] Utiliza al menos dos momentos de recolección de datos
- [ ] Sujetos (humanos o artefactos) son identificables entre momentos de recolección
- [ ] Justifica la estrategia de análisis de datos<sup>[3](#myfootnote3)</sup>
- [ ] La estrategia de análisis de datos es adecuada para la naturaleza interdependiente de los datos<sup>[2](#myfootnote2)</sup>
- [ ] Discute los niveles alfa críticos o justifica los antecedentes bayesianos<sup>[4](#myfootnote4)</sup>
- [ ] Justifica el tamaño de la muestra (por ejemplo, mediante el análisis de potencia)<sup>[5](#myfootnote5)</sup>
- [ ] Describe la pérdida de datos en los diferentes momentos de recolección
- [ ] Explica cómo se manejan los datos faltantes

<results>

- [ ] Describe los sujetos (por ejemplo, información demográfica en el caso de los seres humanos)<sup>[6](#myfootnote6)</sup>

<discussion>

- [ ] Discute la operacionalización del modelo de investigación (es decir, validez de constructo)<sup>[7](#myfootnote7)</sup>

<other>
    
</checklist>
    
### Atributos Deseables
<checklist name="Desirable">

- [ ] Proporciona materiales complementarios que incluyen conjuntos de datos, scripts o instrumentos de recopilación de datos, scripts analíticos, una descripción de cómo reproducir el trabajo y cualquier otro material utilizado
- [ ] Construye una nueva teoría o prueba la teoría existente
- [ ] Investiga la causalidad utilizando la naturaleza longitudinal de los datos para establecer la precedencia y controlando estadísticamente las explicaciones de terceras variables
- [ ] Discute posibles factores de confusión (para análisis inferenciales) que no se pueden controlar estadísticamente
- [ ] Discute las (in)consistencias de los datos en las distintos momentos de recolección (p. ej., fiabilidad testeo-retesteo)
- [ ] Examina las diferencias en las distribuciones entre momentos de recolección (y utiliza una estrategia de análisis de datos adecuada)
- [ ] Describe el costo de recopilar datos y los incentivos utilizados
- [ ] Aborda el sesgo de supervivencia <sup>[8](#myfootnote8)</sup>

</checklist>
    
### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Utiliza un proceso de selección multi-etapa para identificar los sujetos del estudio<sup>[9](#myfootnote9)</sup>
</checklist>
- [ ] Sigue sujetos durante un período excepcionalmente largo (por ejemplo, más de cinco años)

## Criterios Generales de Calidad 

Fiabilidad, validez interna, validez de conclusión, validez de constructo y validez externa.

Los estudios longitudinales explotan la naturaleza temporal de los datos para maximizar la validez interna. A veces se sacrifican otros criterios para mejorar la validez interna.

## Antipatrones

- La pérdida de sujetos entre dos momentos de recolección es demasiado alta, lo que lleva a un estudio con muy poca potencia
- El período entre dos momentos de recolección no coincide con los ciclos naturales del fenómeno
- Tratar los datos longitudinales como transversales

## Variaciones

- _Muestreo de experiencia_ proporciona una comprensión muy específica de un fenómeno a través de múltiples mediciones repetidas por día durante un período corto (generalmente de una a tres semanas). Enfatiza la evaluación en el momento en lugar de la evaluación reflexiva (van Berkel et al.2017). Este estándar se aplica a los estudios de muestreo por experiencia.
- _Estudios de cohorte_ son un tipo de estudio observacional analítico en el que los investigadores investigan la relación entre una variable independiente y dependiente observando a los sujetos a lo largo del tiempo y comparando grupos con diferentes niveles de exposición. Los estudios de cohortes siguen reglas más estrictas que las que se presentan aquí.<sup>[10](#myfootnote10)</sup>

## Críticas Inválidas

- Afirmar que el intervalo de tiempo entre mediciones es demasiado corto o demasiado largo.
- Afirmar que el número de momentos de recolección es inadecuado sin una explicación razonada.
- Afirmar que el tamaño de la muestra es demasiado pequeño sin realizar un cálculo de potencia _post hoc_.
- Afirmar que el artículo con un número modesto de comparaciones debería haber utilizado alfas más conservadoras o adoptado un enfoque bayesiano.
- Quejarse de la generalización cuando el artículo reconoce claramente las limitaciones de la generalización.

## Lecturas Sugeridas

- Franz Faul, et al. Statistical power analyses using G\* Power 3.1: Tests for correlation and regression analyses. In _Behavior Research Methods_. 41,4 (2009), 1149–1160.  
- Flavius Kehr and Tobias Kowatsch. 2015. Quantitative Longitudinal Research: A Review of IS Literature, and a Set of Methodological Guidelines. In _Proceedings of the 23rd European Conference on Information Systems_ (ECIS). Münster, Germany.  
- Hall, Sharon M., et al. &quot;Statistical analysis of randomized trials in tobacco treatment: longitudinal designs with dichotomous outcome.&quot; Nicotine &amp; Tobacco Research 3.3 (2001): 193–202.  
- Duncan, Susan C., Terry E. Duncan, and Hyman Hops. &quot;Analysis of longitudinal data within accelerated longitudinal designs.&quot; Psychological Methods 1.3 (1996): 236.  
- Langfred, Claus W. &quot;The downside of self-management: A longitudinal study of the effects tf conflict on trust, autonomy, and task interdependence in self-managing teams.&quot; Academy of Management Journal 50.4 (2007): 885–900.  
- Benner, Mary J., and Michael Tushman. &quot;Process management and technological innovation: A longitudinal study of the photography and paint industries.&quot; Administrative Science Quarterly 47.4 (2002): 676–707.  
- Joseph P. Simmons, Leif D. Nelson, and Uri Simonsohn. False-positive psychology: Undisclosed flexibility in data collection and analysis allows presenting anything as significant. In _Psychological Science._ 22,11 (2011), 1359—1366.  
- Niels van Berkel, Denzil Ferreira, and Vassilis Kostakos. The experience sampling method on mobile devices. In _ACM Computing Surveys_. 50,6 (2017), 1—40.

## Ejemplares

- Daniel Russo, Paul H.P. Hanel, Seraphina Altnickel, and Niels van Berkel. Predictors of Well-being and Productivity among Software Professionals during the COVID-19 Pandemic — A Longitudinal Study. _Empirical Software Engineering_ (2021). 
- Chandrasekar Subramaniam, Sen Ravi, and Matthew L. Nelson. Determinants of open source software project success: A longitudinal study. In _Decision Support Systems._ 46, 2 (2009), 576—585.  
- Davide Fucci, Simone Romano, Maria Teresa Baldassarre, Danilo Caivano, Giuseppe Scanniello, Burak Turhan, Natalia Juristo. A longitudinal cohort study on the retainment of test-driven development. _International Symposium on Empirical Software Engineering and Measurement._ (2018), 1-10  
- Jingyue Li, Nils B Moe, and Tore Dybå. 2010. Transition from a plan-driven process to Scrum: a longitudinal case study on software quality. _International symposium on empirical software engineering and measurement_. (2010), 1-10  
- Laurie McLeod, Stephen MacDonell, and Bill Doolin.Qualitative Research on software development: a longitudinal case study methodology. _Empirical software engineering_ 16, 4 (2011), 430–459.  
- Jari Vanhanen, Casper Lassenius, and Mika V Mantyla. Issues and tactics when adopting pair programming: A longitudinal case study. _International Conference on Software Engineering Advances_. (2007)  
- Donald E Harter, Chris F Kemerer, and Sandra A Slaughter. 2012. Does software process improvement reduce the severity of defects? A longitudinal field study. _IEEE Transactions on Software Engineering_ 38, 4 (2012), 810–827.

---
<footnote><sup>[1](#myfootnote1)</sup> Sobre el concepto de oscilación natural cf. Kehr &amp; Kowatsch, 2015.</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup> Se utilizan varios enfoques estadísticos diferentes para analizar datos longitudinales (Kehr &amp; Kowatsch provide a partial overview).</footnote><br>
<footnote><sup>[3](#myfootnote3)</sup> Aunque puede que no exista un mejor método para un problema específico, aún debe discutirse a un nivel subjetivo (por ejemplo, por qué se ajusta mejor a la pregunta de investigación) y a un nivel objetivo (por ejemplo, normalidad de los datos).</footnote><br>
<footnote><sup>[4](#myfootnote4)</sup> La elección de los umbrales (por ejemplo, _p_-valores \&lt; 0.05) debe discutirse, para evitar errores de Tipo I. Por lo general, los análisis longitudinales se ocupan de muchas variables y múltiples comparaciones, lo que aumenta la probabilidad de obtener resultados dentro de los umbrales tradicionalmente aceptables. Por esta razón, se recomienda a los autores que ajusten el nivel alfa crítico (p. Ej., Utilizando como umbral _p_-valores \&lt; 0.001) o que utilicen estadísticas bayesianas (Simmons et al., 2011).</footnote><br>
<footnote><sup>[5](#myfootnote5)</sup> Determinar el tamaño de la muestra es de suma importancia para evitar errores de Tipo II. Por lo tanto, los autores pueden definir el tamaño de su muestra utilizando cálculos de potencia a priori. Al mismo tiempo, los revisores pueden controlar el tamaño adecuado mediante un análisis post hoc (Faul, 2019).</footnote><br>
<footnote><sup>[6](#myfootnote6)</sup> El diseño de la investigación debe indicar explícitamente cómo se ha seleccionado y filtrado la muestra a través de un proceso de selección. Por ejemplo, ¿cómo estamos seguros de haber incluido solo ingenieros de software al tratar con sujetos humanos? O, ¿qué tipo de controles de calidad se han realizado en los repositorios de software para garantizar la consistencia y homogeneidad de los artefactos?</footnote><br>
<footnote><sup>[7](#myfootnote7)</sup> Debe quedar claro cuáles son los factores que se están investigando y cómo se han seleccionado. De manera similar, las mediciones deben mostrar una confiabilidad adecuada según los benchmarks de la literatura (por ejemplo, alfa de Cronbach, confiabilidad de testeo-retesteo entre momentos de recolección).</footnote><br>
<footnote><sup>[8](#myfootnote8)</sup> Por ejemplo, si analiza los últimos 100 años de desempeño del mercado de valores en función de los mercados que existen hoy, obtiene retornos promedio mucho más altos que si analiza todos los mercados que existían hace 100 años.</footnote><br>
<footnote><sup>[9](#myfootnote9)</sup> Un ejemplo de dicho proceso de selección se puede encontrar en Russo, Daniel y Klaas-Jan Stol. &quot;Gender differences in personality traits of software engineers.&quot; _IEEE Transactions on Software Engineering_ (2020).</footnote><br>
<footnote><sup>[10](#myfootnote10)</sup> Consultar: David A. Grimes and Kenneth F. Schulz. Cohort studies: marching towards outcomes. _The Lancet_ 359, no. 9303 (2002): 341-345. </footnote><br>
</standard>
