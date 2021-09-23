# Benchmarking (de sistemas software)
<standard name="Benchmarking (of Software Systems)">
         
"Un estudio en el que se evalúa un sistema de software utilizando una herramienta estándar (es decir, un benchmark) para evaluar y comparar de manera competitiva métodos, técnicas o sistemas "de acuerdo con características específicas como rendimiento, confiabilidad o seguridad" (Kistowski et al. 2015).

## Aplicación 

Este estándar se aplica a la investigación empírica que cumple las siguientes condiciones.

-   Investiga sistemas software dentro de un contexto definido con un procedimiento automatizado y repetible
-   Estudia la calidad de servicio del sistema software bajo una carga de trabajo o perfil de uso específicos

Si los benchmark estudian principalmente sistemas software, utilice este estándar.
Para experimentos con participantes humanos, consulte el **Estándar de Experimentos (con participantes humanos)**.
Para la simulación de modelos de los sistemas software, consulte el **Estándar de Simulación (cuantitativo)**.
Si el estudio se lleva a cabo en un contexto del mundo real, consulte el **Estándar de Estudio de Caso y Etnografía**.
El benchmarking se utiliza a menudo con la Investigación en Ingeniería (consulte el **Estándar de Investigación en Ingeniería (Alias Ciencia de Diseño)**)

## Atributos Específicos
### Atributos Esenciales
<checklist name="Essential">

<method>        
             
- [ ]   O BIEN: justifica la selección de un benchmark existente, disponible públicamente o estándar (en términos de relevancia, oportunidad, etc.)
        O: define un nuevo benchmark, que incluye:
        (i) La calidad que se va a evaluar (por ejemplo, rendimiento, disponibilidad, escalabilidad, seguridad),
        (ii) La/s métrica/s) para cuantificar la calidad,
        (iii) El/los método/s de medición para la métrica (si no es obvio),
        (iv) La carga de trabajo, el perfil de uso y/o la muestra de tareas a la que está sujeto el sistema bajo prueba (es decir, qué está haciendo el sistema cuando se toman las medidas)
        Y justifica el diseño del benchmark (en términos de relevancia, oportunidad, etc.)
        Y reutiliza componentes de diseño de benchmarks existentes a partir de benchmarks establecidos o justifica nuevos componentes
- [ ]   Describe la configuración experimental para el benchmark con suficiente detalle para respaldar la replicación independiente (o se refiere a dicha descripción en materiales complementarios)
- [ ]   Especifica la carga de trabajo o el perfil de uso con suficiente detalle para respaldar la replicación independiente (o se refiere a dicha descripción en materiales complementarios)
- [ ]   Permite que diferentes configuraciones de un sistema bajo prueba compitan por sus méritos sin limitaciones artificiales
- [ ]   Evalúa la estabilidad o confiabilidad usando suficientes repeticiones de experimentos y duraciones de ejecución
        
<discussion>
            
- [ ]   Discute la validez de constructo del benchmark; eso es, el benchmark mide lo que se supone que mida?  
        
<other>                


</checklist>
    
### Atributos Deseables
<checklist name="Desirable">
    
- [ ]   Proporciona materiales complementarios que incluyen conjuntos de datos, scripts de análisis y (para benchmarks novedosos) documentación ampliada
- [ ]   Proporciona benchmark/s en una forma utilizable que facilita la replicación independiente
- [ ]   Informa sobre la replicación independiente de los resultados del benchmark
- [ ]   Informa sobre una gran comunidad que utiliza el benchmark
- [ ]   Informa sobre una organización independiente que mantiene el benchmark
- [ ]   Utiliza o crea benchmarks de código abierto
- [ ]   Informa de forma transparente sobre problemas con la ejecución del benchmark, si las hubiera

</checklist>
    
### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Proporciona evidencia empírica de la relevancia de un benchmark, por ejemplo, utilizando una revisión sistemática
- [ ] Proporciona evidencia empírica para la usabilidad de un benchmark, por ejemplo, utilizando investigación acción o estudios de caso

</checklist>
     
## Criterios Generales de Calidad

Equidad de las mediciones, reproducibilidad de los resultados a través de las repeticiones de experimentos, evaluación de los aspectos *correctos*, utilizando un benchmark realista con una carga de trabajo representativa

## Ejemplos de Desviaciones Aceptables 

-   La naturaleza del benchmark requiere hardware especializado (por ejemplo, una computadora cuántica) por lo que no es fácil de replicar
-   En un estudio que replica el trabajo existente publicado, la descripción de la configuración experimental podría ser bastante breve
-   El estudio solo emplea una (o algunas) corridas porque el trabajo previo ha demostrado que una sola corrida es suficiente

## Antipatrones

-   Adaptar el benchmark para un método, técnica o herramienta específica, que se evalúa con el benchmark.
-   Utilizar experimentos de benchmarking que son irrelevantes para el problema estudiado para ocultar las debilidades del enfoque propuesto.
-   Repeticiones o duración insuficientes para evaluar la estabilidad de los resultados
-   Recopilar mediciones agregadas en lugar de conservar todos los resultados sin procesar y ejecutar un análisis fuera de línea

## Criticas Inválidas

-   El benchmark no se utiliza mucho. Basta con empezar a desarrollar un nuevo benchmark con un pequeño grupo de investigadores como oferta a una comunidad científica más amplia. Dicho prototipo de benchmark (Sim et al. 2003) puede actuar como una plantilla para promover la discusión del tema e iniciar el proceso de consenso.
-   No se informa una replicación independiente de los resultados del benchmark.
-   No existe una organización independiente que mantenga el benchmark.

## Lecturas Sugeridas

David Bermbach, Erik Wittern, and Stefan Tai. 2017. Cloud service benchmarking: Measuring Quality of Cloud Services from a Client Perspective. Springer. DOI: [10.1007/978-3-319-55483-9](https://doi.org/10.1007/978-3-319-55483-9)

Susan Elliott Sim, Steve Easterbrook, and Richard C. Holt. 2003. Using benchmarking to advance research: a challenge to software engineering. In 25th International Conference on Software Engineering. IEEE. DOI: [10.1109/icse.2003.1201189](https://doi.org/10.1109/icse.2003.1201189)

Jim Gray (Ed.). 1993. The Benchmark Handbook for Database and Transaction Systems (2nd ed.). Morgan Kaufmann.

Wilhelm Hasselbring. 2021. Benchmarking as Empirical Standard in Software Engineering Research. In Proceedings of the 25th International Conference on Evaluation and Assessment in Software Engineering (EASE 2021). 365-372. DOI: [10.1145/3463274.3463361](https://doi.org/10.1145/3463274.3463361)

Jóakim v. Kistowski, Jeremy A. Arnold, Karl Huppler, Klaus-Dieter Lange, John L. Henning, and Paul Cao. 2015. How to Build a Benchmark. In Proceedings of the 6th ACM/SPEC International Conference on Performance Engineering. DOI: [10.1145/2668930.2688819](https://doi.org/10.1145/2668930.2688819)

Samuel Kounev, Klaus-Dieter Lange, and Jóakim von Kistowski. 2020. Systems Benchmarking for Scientists and Engineers. Springer. DOI: [10.1007/978-3-030-41705-5](https://doi.org/10.1007/978-3-030-41705-5)

Alessandro Vittorio Papadopoulos,  Laurens Versluis, André Bauer, Nikolas Herbst,  Jóakim von Kistowski, Ahmed Ali-Eldin, Cristina L. Abad,  José Nelson Amaral, Petr Tůma, Alexandru Iosup. 2021. Methodological Principles for Reproducible Performance Evaluation in Cloud Computing. In IEEE Transactions on Software Engineering, vol. 47, no. 8, pp. 1528-1543. DOI: [10.1109/TSE.2019.2927908](https://doi.org/10.1109/TSE.2019.2927908)

Walter F. Tichy. 1998. Should computer scientists experiment more? Computer 31, 5 (May 1998), 32–40. DOI: [10.1109/2.675631](https://doi.org/10.1109/2.675631)

Walter F. Tichy. 2014. Where’s the Science in Software Engineering? Ubiquity Symposium: The Science in Computer Science. Ubiquity 2014 (March 2014), 1–6.  DOI: [10.1145/2590528.2590529](https://doi.org/10.1145/2590528.2590529)


## Ejemplares

Sören Henning and Wilhelm Hasselbring. 2021. Theodolite: Scalability Benchmarking
of Distributed Stream Processing Engines in Microservice Architectures.
Big Data Research 25 (July 2021), 1–17. DOI: [10.1016/j.bdr.2021.100209](https://doi.org/10.1016/j.bdr.2021.100209)

Guenter Hesse, Christoph Matthies, Michael Perscheid, Matthias Uflacker, and Hasso Plattner. 2021. ESPBench: The Enterprise Stream Processing Benchmark. In ACM/SPEC International Conference on Performance Engineering (ICPE '21). ACM, 201–212. DOI: [10.1145/3427921.3450242](https://doi.org/10.1145/3427921.3450242)

Martin Grambow, Erik Wittern, and David Bermbach. 2020. Benchmarking the Performance of Microservice Applications. ACM SIGAPP Applied Computing Review, vol 20, issue 3, 20-34. DOI: [10.1145/3429204.3429206](https://doi.org/10.1145/3429204.3429206)
    
Joakim von Kistowski, Simon Eismann, Norbert Schmitt, Andre Bauer, Johannes Grohmann, and Samuel Kounev. 2018. TeaStore: A Micro-Service Reference Application for Benchmarking, Modeling and Resource Management Research. In 2018 IEEE 26th International Symposium on Modeling, Analysis, and Simulation of Computer and Telecommunication Systems (MASCOTS). IEEE, 223–236. DOI: [10.1109/mascots.2018.00030](https://doi.org/10.1109/mascots.2018.00030)

Christoph Laaber, Joel Scheuner, and Philipp Leitner. 2019. Software microbenchmarking in the cloud. How bad is it really?. Empirical Software Engineering 24, 2469–2508. DOI: [10.1007/s10664-019-09681-1](https://doi.org/10.1007/s10664-019-09681-1)

Jan Waller, Nils C. Ehmke, and Wilhelm Hasselbring. 2015. Including Performance Benchmarks into Continuous Integration to Enable DevOps. SIGSOFT Softw. Eng. Notes 40, 2 (March 2015), 1–4. DOI: [10.1145/2735399.2735416](https://doi.org/10.1145/2735399.2735416)

</standard>
