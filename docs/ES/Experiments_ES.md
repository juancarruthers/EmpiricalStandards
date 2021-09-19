# Experimentos (con Participantes Humanos) 
<standard name="Experiments (with Human Participants)">

*Un estudio en el que se introduce deliberadamente una intervención para observar
sus efectos sobre algunos aspectos de la realidad en condiciones controladas*

## Aplicación

Esta norma se aplica a experimentos controlados y cuasiexperimentos
que cumplen las siguientes condiciones (todas):

-   Manipula una o más variables independientes
-   Identifica y controla muchas de las variables extrañas
-   Aplica cada tratamiento de forma independiente a varias unidades experimentales
-   Involucra a participantes humanos

En los experimentos verdaderos, las unidades experimentales se asignan al azar entre
tratamientos; los cuasiexperimentos carecen de asignación aleatoria. Los experimentos
incluyen diseños inter-sujetos, intra-sujetos y medidas repetidas.
Para experimentos sin participantes humanos, consulte el **Estándar de Ciencia de Datos
Exploratorios** o el **Estándar de Investigación de Ingeniería**.

## Atributos Específicos

### Atributos Esenciales
<checklist name="Essential">

<intro>


<method>
    
- [ ]	Establece hipótesis formales
- [ ]	Justifica el uso de hipótesis unilaterales (si las hay) basadas en la validez aparente o en trabajos previos
- [ ]	Describe las variables dependientes y justifica cómo se miden (incluidas las unidades, los instrumentos)
- [ ]	Describe las variables independientes y cómo se manipulan o miden
- [ ]	Describe variables extrañas y cómo se controlan o no
- [ ]	Describe cómo las características del fenómeno bajo investigación se relacionan con los constructos experimentales
- [ ]	Describe el diseño y el protocolo de la investigación, incluidos los tratamientos, materiales, tareas, diseño (por ejemplo, factorial 2x2), asignación de participantes, período y secuencias (para diseños cruzados) y logística
- [ ]	O BIEN: utiliza la asignación aleatoria y explica la logística (por ejemplo, cómo se generaron los números aleatorios)
    O: proporciona una justificación convincente para no utilizar la asignación aleatoria y explica cómo se mitiga la amenaza a la validez de grupos desiguales (por ejemplo, utilizando el diseño pre-test/post-test y sujetos emparejados)
- [ ]	Describe objetos experimentales (por ejemplo, un sistema de laboratorio o real) y sus características (por ejemplo, tamaño, tipo)
- [ ]	Justifica la selección de objetos experimentales; reconoce las confusiones entre el objeto y el tratamiento, si las hubiera<sup>[1](#myfootnote1)</sup>
- [ ]	Diseño y protocolo apropiados (no óptimos) para las preguntas e hipótesis de investigación establecidas

<results>

- [ ]	Describe a los participantes (por ejemplo, edad, género, educación, experiencia o preferencias relevantes)
- [ ]	Reporta estadísticas descriptivas e inferenciales apropiadas para la distribución; justifica las pruebas utilizadas
- [ ]	Informa el Tamaño del Efecto con intervalos de confianza (si se utiliza un enfoque de probabilidad frecuentista)

<discussion>

- [ ]	Discute la validez del constructo, de la conclusión, interna y externa
- [ ]	Analiza interpretaciones alternativas de los resultados

<other>    

</checklist>
     
### Atributos Deseables
<checklist name="Desirable">

- [ ]	Proporciona material complementario, como un protocolo completo de los pasos; material de las tareas; conjunto de datos sin procesar y sin identificar,guiones de análisis
- [ ]	Justifica hipótesis y antecedentes bayesianos (si corresponde) basándose en estudios y teorías previas
- [ ]	Discute diseños experimentales alternativos y por qué no se utilizaron (por ejemplo, compensaciones de validez)
- [ ]	Incluye visualizaciones de distribuciones de datos
- [ ]	Cita la investigación estadística para respaldar cualquier problema matizado o enfoque inusual
- [ ]	Explica las desviaciones entre el diseño y la ejecución, y sus implicaciones<sup>[2](#myfootnote2)</sup>
- [ ]	Diseño de experimento con nombre (por ejemplo, 2 grupos simples, factorial 2x2, bloque aleatorio)
- [ ]	Justifica el tamaño de la muestra (por ejemplo, usando análisis de potencia)
- [ ]	Analiza la validez de constructo de la variable dependiente
- [ ]	Informa los controles de manipulación
- [ ]	prerregistro de hipótesis y diseño (donde el lugar lo permita)
- [ ]	distingue claramente los resultados basados en la evidencia de las interpretaciones y la especulación<sup>[3](#myfootnote3)</sup>
</checklist>
     
### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ]	Reporta múltiples experimentos o réplicas en diferentes culturas o regiones
- [ ]	Utiliza múltiples métodos de recopilación de datos; triangulación de datos
- [ ]	Recopilación de datos longitudinales con análisis de series de tiempo adecuados (consulte el [Estándar de estudios Longitudinales](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/Longitudinal.md))
</checklist>

## Criterios Generales de Calidad

Validez de conclusión, validez de constructo, validez interna, confiabilidad,
objetividad, reproducibilidad

## Antipatrones

-   Uso de proxy incorrectos para variables dependientes (por ejemplo, la duración 
    de la tarea como un proxy para la complejidad de la tarea)
-   Cuasi-experimentos sin una buena razón<sup>[4](#myfootnote4)</sup>
-   Los tratamientos o las variables de respuesta están mal descritos
-   Diseño inadecuado para las condiciones en las que se llevó a cabo
    el experimento.
-   La técnica de análisis de datos utilizada no se corresponde con el diseño
    elegido o las características de los datos (p. ej., utilizando una prueba
    t de muestras independientes en datos emparejados).
-   Las amenazas de validez se enumeran simplemente sin vincularlas a los resultados.
-   Faltan hipótesis

## Críticas Inválidas

-   Los participantes son estudiantes: la idoneidad de las características de los participantes
    debe juzgarse en función del contexto, el nivel de control deseado,
    las opciones de compensación entre la validez interna y externa
    y las características específicas de la tecnología (es decir, método,
    técnica, herramienta, proceso, etc.) bajo evaluación; la elección debe explicarse
    en el documento
-   Baja validez externa
-   El experimento es una replica
-   El revisor habría investigado el tema de cualquier otra forma que no fuera
    un experimento
-   No hay suficientes participantes (a menos que esté respaldado por un análisis de potencia)

## Ejemplares

Dag IK Sjøberg, Aiko Yamashita, Bente CD Anda, Audris Mockus, and Tore
Dybå. 2012. Quantifying the Effect of Code Smells on Maintenance Effort.
*IEEE Transactions on Software Engineering*. 39, 8 (Dec. 2012),
1144–1156. DOI: 10.1109/TSE.2012.89.

Ayse Tosun, Oscar Dieste, Davide Fucci, Sira Vegas, Burak Turhan, Hakan
Erdogmus, Adrian Santos et al. 2017. An industry experiment on the
effects of test-driven development on external quality and productivity.
*Empirical Software Engineering*. *22*, 6 (Dec. 2016), 2763–2805.

Kai Petersen, Kari Rönkkö, and Claes Wohlin. 2008. The impact of time
controlled reading on software inspection effectiveness and efficiency:
a controlled experiment. In *Proceedings of the Second ACM-IEEE
International Symposium on Empirical Software Engineering and
Measurement (ESEM '08)*, 139–148. DOI:10.1145/1414004.1414029

Eduard P. Enoiu, Adnan Cauevic, Daniel Sundmark, and Paul Pettersson.
2016. A controlled experiment in testing of safety-critical embedded
software. In *2016 IEEE International Conference on Software Testing,
Verification and Validation (ICST),* 11-15 April, Chicago, IL, USA.
IEEE. 1-11.

Yang Wang and Stefan Wagner. 2018. Combining STPA and BDD for safety
analysis and verification in agile development. In *Proceedings of the
40th International Conference on Software Engineering: Companion
Proceeedings (ICSE '18)*, 286–287. DOI:10.1145/3183440.3194973

Evrim Itir Karac, Burak Turhan, and Natalia Juristo. 2019. A Controlled
Experiment with Novice Developers on the Impact of Task Description
Granularity on Software Quality in Test-Driven Development. *IEEE
Transactions on Software Engineering.* DOI: 10.1109/TSE.2019.2920377

## Lecturas Sugeridas

Nathaniel L. Gage and Julian C. Stanley. 1963. Experimental and Quasi-experimental Designs For Research. Chicago: R. McNally.

Andreas Jedlitschka, Marcus Ciolkowski, and Dietmar Pfahl. 2008. Reporting Experiments in Software Engineering. _Guide to Advanced Empirical Software Engineering_. 201-228.

Natalia Juristo and Ana M. Moreno. 2001. Basics of Software Engineering Experimentation. Springer Science & Business Media.

Claes Wohlin, Per Runeson, Martin Höst, Magnus C. Ohlsson, Björn Regnell, and Anders Wesslén. 2012. Experimentation in Software Engineering. Springer Science & Business Media.

Martín Solari, Sira Vegas, and Natalia Juristo. 2018. Content and structure of laboratory packages for software engineering experiments. _Information and Software Technology_. 97, 64-79.

Sira Vegas, Cecilia Apa, and Natalia Juristo. 2015. Crossover designs in software engineering experiments: Benefits and perils. _IEEE Transactions on Software Engineering_. IEEE 42, 2 (2015), 120-135.

Vigdis By Kampenes, Tore Dybå, Jo E. Hannay, and Dag IK Sjøberg. 2009. A systematic review of quasi-experiments in software engineering. _Information and Software Technology_. 51, 1 (2009), 71-82.

Davide Falessi, Natalia Juristo, Claes Wohlin, Burak Turhan, Jürgen Münch, Andreas Jedlitschka, and Markku Oivo, Empirical Software Engineering Experts on the Use of Students and Professionals in Experiments, _Empirical Software Engineering_. 23, 1 (2018), 452-489.

Robert Feldt, Thomas Zimmermann, Gunnar R. Bergersen, Davide Falessi, Andreas Jedlitschka, Natalia Juristo, Jürgen Münch et al. 2018. Four commentaries on the use of students and professionals in empirical software engineering experiments. _Empirical Software Engineering_. 23, 6 (Nov. 2018), 3801-3820.

Kitchenham, Barbara, Lech Madeyski, David Budgen, Jacky Keung, Pearl Brereton, Stuart Charters, Shirley Gibbs, and Amnart Pohthong. 2017. Robust statistical methods for empirical software engineering. _Empirical Software Engineering_. 22, 2 (2018), 579-630.

Andreas Zeller, Thomas Zimmermann, and Christian Bird. 2011. Failure is a four-letter word: a parody in empirical research. In Proceedings of the _7th International Conference on Predictive Models in Software Engineering (Promise ’11)_. Association for Computing Machinery, New York, NY, USA, Article 5, 1–7. DOI: 10.1145/2020390.2020395


---
<footnote><sup>[1](#myfootnote1)</sup> Por ejemplo, en un experimento donde el grupo de control aplica el desarrollo basado en pruebas (TDD) con el objeto 1, mientras que el grupo de tratamiento aplica la prueba-último-desarrollo (TLD) con el objeto 2, el objeto experimental se confunde con el tratamiento.</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup> p. Ej. abandonos que afectan el equilibrio entre el tratamiento y el grupo de control.</footnote><br>
<footnote><sup>[3](#myfootnote3)</sup> Por lo general, basta con separar los resultados y la discusión en diferentes secciones. Sin especulaciones en la sección de resultados.</footnote><br>
<footnote><sup>[4](#myfootnote4)</sup> Los cuasi experimentos son apropiados para estudios piloto o cuando la asignación está más allá del control del investigador (por ejemplo, asignar a los estudiantes a dos cohortes diferentes de un curso). Afirmar simplemente que un estudio es "exploratorio" no es una justificación suficiente.</footnote><br>
</standard>
