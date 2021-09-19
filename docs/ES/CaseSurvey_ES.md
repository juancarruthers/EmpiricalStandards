# Encuesta de Caso (Alias Meta-Análisis de Caso)
<standard name="Case Survey">

*Un estudio que tiene como objetivo generalizar los resultados sobre un fenómeno complejo convirtiendo sistemáticamente las descripciones cualitativas disponibles en los estudios de casos publicados en datos cuantitativos, y analizando los datos convertidos.*

## Aplicación

Esta norma se aplica a los estudios en los que:
-	Se obtiene una muestra de estudios de casos publicados anteriormente;
-	Las descripciones cualitativas de los casos se convierten sistemáticamente en datos cuantitativos; y
-	Los datos cuantitativos convertidos se analizan para alcanzar resultados generalizables.

Esta norma no se aplica a los estudios que recopilan datos primarios de una gran cantidad de casos de un fenómeno; por ejemplo, utilizando entrevistas (considere el **Estándar de Encuesta Cualitativa**) o cuestionarios (considere el **Estándar de Encuesta de Cuestionario**). Para estudios de casos individuales, utilice el **Estándar de Estudios de Casos**. Para revisiones de otros tipos de estudios (por ejemplo, experimentos), considere el **Estándar de Revisión Sistemática**. Este estándar tampoco se aplica a la síntesis cualitativa (por ejemplo, meta-etnografía, síntesis narrativa).

## Atributos Específicos

### Atributos Esenciales
<checklist name="Essential">

<intro>


<method>

- [ ]   Presenta una descripción paso a paso, sistemática y replicable del proceso de búsqueda de estudios de casos publicados (no necesariamente en lugares de publicación revisados por pares)
- [ ]   Define criterios claros de inclusión y exclusión para los casos<sup>[1](#myfootnote1)</sup>
- [ ]   Describe la estrategia de muestreo (consulte el [Suplemento de muestreo](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/Sampling.md))
- [ ]   Mitiga el sesgo de muestreo y el sesgo de publicación, utilizando algunas (no todas):
(i) Búsquedas manuales y búsquedas automáticas por palabras clave;
(ii) Búsquedas con bola de nieve hacia atrás y hacia adelante;
(iii) Revisión de perfiles de autores prolíficos en el tema;
(iv) Búsqueda en bases de datos formales (por ejemplo, ACM Digital Library) y buscadores (por ejemplo, Google Scholar);
(v) Búsqueda de disertaciones relevantes;
(vi) Buscar servidores de pre-impresión (por ejemplo, arXiv);
(vii) Solicitar manuscritos no publicados a través de listas de correo electrónico o redes sociales apropiadas;
(viii) Contactar a autores conocidos en el tema.
- [ ]   define un esquema de codificación para convertir descripciones de casos cualitativos en variables cuantitativas<sup>[2](#myfootnote2)</sup>
- [ ]   O BIEN: describe el esquema de codificación en detalle;
O: proporciona el esquema de codificación en materiales complementarios
- [ ]   explica claramente cómo se gestionó las ausencias de datos en el conjunto de datos

<results>

- [ ]   Saca conclusiones basadas en las variables cuantitativas derivadas

<discussion>

- [ ]   Reconoce las amenazas de generalización; discute cómo los estudios de caso revisados pueden diferir de la población objetiva

<other>  
  
</checklist>

### Atributos Deseables
<checklist name="Desirable">

- [ ]   Proporciona materiales complementarios como protocolos, términos de búsqueda, resultados de búsqueda, resultados del proceso de selección, esquemas de codificación, ejemplos de codificación, reglas de decisión, conjuntos de datos completos, scripts de análisis, descripciones de casos extremos<sup>[3](#myfootnote3)</sup>
- [ ]   Explica y justifica el diseño del esquema de codificación
- [ ]   Utiliza más de 2 analistas independientes; analiza la confiabilidad entre evaluadores (consulte el [Suplemento de IRR/IRA](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/InterRaterReliabilityAndAgreement.md)); explica cómo se resolvieron las discrepancias entre los codificadores<sup>[4](#myfootnote4)</sup>
- [ ]   Describe cómo ponerse en contacto con los autores de los estudios primarios para obtener más información, verificar la precisión de la codificación o resolver desacuerdos de codificación
- [ ]   Evalúa la calidad de los estudios primarios utilizando un esquema a priori (por ejemplo, el **Estándar de Encuestas de Casos**); explica cómo se evaluó la calidad; los modelos estudian la calidad como variable moderadora
- [ ]   Consolida los resultados mediante tablas, diagramas o gráficos; incluye el diagrama de flujo PRISMA (cf. Moher et al. 2009)
- [ ]   Integra resultados en teorías o investigaciones anteriores; identifica brechas, sesgos o direcciones futuras
- [ ]   Presenta los resultados como pautas prácticas basadas en evidencia para profesionales, investigadores o educadores
- [ ]   Distingue claramente los resultados basados en evidencia de las interpretaciones y especulaciones<sup>[5](#myfootnote5)</sup>

</checklist>

### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ]   Utiliza la teoría para seleccionar y muestrear casos
- [ ]   Dos o más investigadores realizan de forma independiente el proceso de búsqueda preliminar antes de finalizar el alcance de la búsqueda y las palabras clave de búsqueda
- [ ]   Agrega datos de otras fuentes a los casos seleccionados
- [ ]   Emplea autores de estudios primarios para realizar la codificación o garantizar que las interpretaciones sean correctas
- [ ]   Analiza si y cómo las características de los estudios (por ejemplo, el diseño de la investigación, el lugar de publicación o la fecha) influyen en la codificación
</checklist>

## Criterios Generales de Calidad

Fiabilidad, validez interna, validez externa, validez de constructo, validez de la conclusión

## Antipatrones

-	Incluir estudios primarios que no son estudios de caso (por ejemplo, cuestionarios o una pequeña cantidad de datos)
-	Incluir todos los casos sin una evaluación crítica de los datos disponibles
-	Analizar datos de casos utilizando técnicas cualitativas
-	Describir cada caso de forma aislada en lugar de sintetizar los resultados.
-	Confiar en el lugar de publicación como proxy de la calidad
-	Combinar la correlación con la causalidad en los hallazgos

## Criticas Inválidas

-	Los estudios no se publicaron en lugares de publicación revisados por pares
-	Los estudios originales no emplean un diseño de investigación común
-	Los casos no son una muestra aleatoria del fenómeno

## Lecturas Sugeridas

R.J. Bullock and Mark Tubbs. 1987. “The case meta-analysis method for OD,” *Research in organizational change and development*.  1, 171–228.

Marlen Jurisch, Petra Wolf, and Helmut Krcmar. 2013. Using the case survey method for synthesizing case study evidence in information systems research. *19th Americas Conference on Information Systems, AMCIS 2013 - Hyperconnected World: Anything, Anywhere, Anytime (2013)*, 3904–3911.

Rikard Larsson. 1993. Case survey methodology: quantitative analysis of patterns across case studies. *Academy of Management Journal*. 36, 6 (Dec. 1993), 1515–1546. DOI: 10.2307/256820.

William Lucas. 1974. The Case Survey Method: Aggregating Case Experience. Rand Corporation, Santa Monica, CA.

Jorge Melegati and Xiaofeng Wang. 2020. Case Survey Studies in Software Engineering Research. *Proceedings of the 14th ACM / IEEE International Symposium on Empirical Software Engineering and Measurement (ESEM)* (Oct. 2020), 1–12.

Moher D, Liberati A, Tetzlaff J, Altman DG, The PRISMA Group (2009). *P*referred *R*eporting *I*tems for *S*ystematic Reviews and *M*eta-*A*nalyses: The PRISMA Statement. PLoS Med 6, 7: e1000097. doi:10.1371/journal.pmed1000097  
  
Robert Yin and Karen Heald. 1975. Using the Case Survey Method to Analyze Policy Studies. *Administrative Science Quarterly*. 20, 3 (1975), 371. DOI:10.2307/2391997.


## Ejemplares

R.J. Bullock and Mark Tubbs. 1990. A case meta-analysis of gainsharing plans as organization development interventions. *The Journal of Applied Behavioral Science* 26.3 (1990): 383-404.

Åke Grönlund and Joachim Åström. 2009. DoIT right: Measuring effectiveness of different eConsultation designs. *Lecture Notes in Computer Science (including subseries Lecture Notes in Artificial Intelligence and Lecture Notes in Bioinformatics)*. 5694 LNCS, (2009), 90–100. DOI: 10.1007/978-3-642-03781-8_9.

Marlen Jurisch, Christin Ikas, Petra Wolf and Helmut Krcmar. 2013. Key Differences of Private and Public Sector Business Process Change. *e-Service Journal*. 9, 1 (2013), 3. DOI:10.2979/eservicej.9.1.3.

Marlen Jurisch, Wolfgang Palka, Petra Wolf, and Helmut Krcmar. 2014. Which capabilities matter for successful business process change? *Business Process Management Journal*. 20, 1 (2014), 47–67. DOI:10.1108/BPMJ-11-2012-0125.

Rikard Larsson and Michael Lubatkin. 2001. Achieving acculturation in mergers and acquisitions: An international case survey. _Human Relations_. 54, 12 (2001), 1573–1601. DOI: 10.1177/00187267015412002.

Mark de Reuver, Harry Bouwman, and Ian MacInnes. 2007. What drives business model dynamics? A case survey. *8th World Congress on the Management of e-Business, WCMeB 2007 - Conference Proceedings*. WCMeB (2007). DOI: 10.1109/WCMEB.2007.95.

Mark de Reuver, Harry Bouwman, and Ian MacInnes. 2009. Business model dynamics: A case survey. *Journal of Theoretical and Applied Electronic Commerce Research*. 4, 1 (2009), 1–11. DOI:10.4067/S0718-18762009000100002.

---
<footnote><sup>[1](#myfootnote1)</sup>Por ejemplo, informa al menos dos de las variables en el esquema de codificación.</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup>El esquema de codificación debe equilibrar la simplicidad y la riqueza de la información.</footnote><br>
<footnote><sup>[3](#myfootnote3)</sup>Proporciona datos de varios evaluadores y scripts para calcular el acuerdo entre evaluadores, si es posible, pero no proporciona las respuestas del autor principal del estudio a ningún cuestionario a menos que los autores hayan dado permiso explícito.</footnote><br> 
<footnote><sup>[4](#myfootnote4)</sup>Mediante la discusión y acuerdo, votando, agregando un desempate, consultando con los autores del estudio, etc.</footnote><br>
<footnote><sup>[5](#myfootnote5)</sup>Por lo general, basta con separar los resultados y la discusión en diferentes secciones. Sin especulaciones en la sección de resultados.</footnote><br>
                                    
</standard>


