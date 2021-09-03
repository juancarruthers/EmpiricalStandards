# Estudios de Optimización en IS (incluyendo la Ingeniería de Software Basada en Búsquedas)
<standard name="Optimization Studies">

*Estudios de investigación que se centren en la formulación de problemas de la Ingeniería de Software como problemas de búsqueda y apliquen técnicas de optimización para resolver dichos problemas*<sup>[1](#myfootnote1)</sup>.  

## Aplicación

Este estándar se aplica a los estudios empíricos que cumplen los siguientes criterios:

- Formula una tarea de la Ingeniería de Software<sup>[2](#myfootnote2)</sup> como un problema de optimización, con una o más funciones de calidad específicas<sup>[3](#myfootnote3)</sup> utilizadas para juzgar el éxito en esta tarea.
- Aplica uno o más enfoques que generan soluciones al problema en un intento de maximizar o minimizar las funciones de calidad especificadas.

## Atributos Específicos
Hacemos hincapié en que el uso de la optimización en IS sigue siendo un campo en rápida evolución. Por lo tanto, los siguientes criterios son aproximados y pueden existir muchas excepciones. Los revisores deben recompensar el trabajo sólido y novedoso y, cuando sea posible, apoyar una amplia gama de estudios.
### Atributos Esenciales
<checklist name="Essential">  

<intro>

- [ ] Explica por qué el problema no se puede optimizar manualmente o mediante la fuerza bruta dentro de un período de tiempo razonable<sup>[4](#myfootnote4)</sup>
- [ ] O BIEN: describe el estado de la técnica anterior en esta área
      O: motiva y define cuidadosamente el problema abordado y la solución propuesta

<method>

- [ ] Describe el espacio de búsqueda (por ejemplo, restricciones, opciones de variables independientes)
- [ ] Utiliza simplificaciones y restricciones realistas y limitadas para el problema de optimización; Las simplificaciones y restricciones no reducen la búsqueda a una en la que todas las soluciones puedan enumerarse mediante la fuerza bruta.
- [ ] Justifica la elección del algoritmo<sup>[5](#myfootnote5)</sup> subyacente al enfoque<sup>[6](#myfootnote6)</sup>
- [ ] Compara enfoques con una base de referencia justificada y apropiada<sup>[7](#myfootnote7)</sup>
- [ ] Define explícitamente la formulación de la solución, incluyendo una descripción de lo que representa una solución<sup>[8](#myfootnote8)</sup>, cómo se representa<sup>[9](#myfootnote9)</sup>, y como se manipula
- [ ] Define explícitamente todas las funciones de calidad, incluyendo el tipo de objetivos optimizados y las ecuaciones para calcular los valores de calidad
- [ ] Define explícitamente los enfoques evaluados, incluyendo las técnicas, heurísticas específicas y los parámetros y sus valores<sup>[10](#myfootnote10)</sup>
- [ ] O BIEN: describe claramente (y sigue) un proceso sólido para recopilar y preparar los conjuntos de datos utilizados para ejecutar y evaluar el enfoque de optimización
      O: si los sujetos provienen de trabajos anteriores, haga referencia completa a la fuente original y explique si se aplicó alguna transformación o limpieza a los conjuntos de datos
- [ ] O BIEN: pone los datos a disposición del público
      O: explica por qué esto no es posible<sup>[11](#myfootnote11)</sup>
- [ ] Identifica y explica todas las posibles fuentes de estocasticidad<sup>[12](#myfootnote12)</sup>
- [ ] O BIEN: ejecuta enfoques o elementos estocásticos varias veces
      O: explica por qué esto no es posible<sup>[13](#myfootnote13)</sup>


<results>

<discussion>

<other>
      
</checklist>

### Atributos Deseables
<checklist name="Desirable">

- [ ] Proporciona un paquete de replicación que cumple con los estándares SIGSOFT para artefactos<sup>[14](#myfootnote14)</sup>.
- [ ] Motiva la novedad y solidez del enfoque propuesto<sup>[15](#myfootnote15)</sup>
- [ ] Explica si el estudio explora un nuevo tipo de problema (o un área nueva dentro de un espacio de problema existente), o cómo reproduce, replica o mejora el trabajo anterior
- [ ] Explica en detalle cómo se recopilaron/eligieron sujetos o conjuntos de datos para mitigar el sesgo de selección y mejorar la generalización de los hallazgos
- [ ] Describe las características principales de los sujetos utilizados para ejecutar y evaluar el/los enfoque(s) de optimización y discutir qué caracteriza las diferentes instancias en términos de "dureza"
- [ ] Justifica el uso de datos sintéticos (si los hubiera); explica por qué no se pueden utilizar datos del mundo real; discute hasta qué punto el enfoque propuesto y los hallazgos pueden aplicarse al mundo real
- [ ] (Si los datos no se pueden compartir) proporciona un conjunto de datos de muestra que se puede compartir para ilustrar el enfoque
- [ ] Selecciona un espacio de opciones realista para formular una solución; los valores establecidos para los atributos deben reflejar uno que pueda elegirse en una solución del "mundo real" y no generarse a partir de una distribución arbitraria.
- [ ] Justifica los valores de los parámetros utilizados al ejecutar los enfoques evaluados (y tenga en cuenta que los experimentos que prueben una amplia gama de valores de parámetros diferentes serían extraordinarios, ver más abajo)
- [ ] Muestrea datos varias veces de manera controlada (cuando sea apropiado y posible)
- [ ] Realiza múltiples pruebas ya sea como validación cruzada (múltiples ejecuciones independientes) o temporalmente (múltiples aplicaciones como parte de una secuencia cronometrada), dependiendo del problema en cuestión
- [ ] Proporciona divisiones de datos aleatorias (por ejemplo, las que se utilizan en enfoques basados en datos) o garantiza que las divisiones son reproducibles.
- [ ] Compara distribuciones (en lugar de medias) de los resultados utilizando estadísticas adecuadas
- [ ] Compara soluciones utilizando un criterio de meta-evaluación apropiado<sup>[16](#myfootnote16)</sup>; justifica los criterios elegidos
- [ ] Distingue claramente los resultados basados en evidencia de las interpretaciones y especulaciones<sup>[17](#myfootnote17)</sup>
</checklist>

### Atributos Extraordinarios
<checklist name="Extraordinary">

- [ ] Analiza diferentes opciones de parámetros para el algoritmo, indicando cómo se seleccionaron los parámetros finales<sup>[18](#myfootnote18)</sup>
- [ ] Analiza el panorama de calidad para una o más de las funciones de calidad elegidas
</checklist>

## Criterios Generales de Calidad

Los criterios de calidad más valiosos para los estudios de optimización en IS incluyen confiabilidad, replicabilidad, reproducibilidad, rigor y utilidad (ver **Glosario**).

## Ejemplos de Desviaciones Aceptables

 - El número de pruebas puede verse limitado por el tiempo disponible o los recursos experimentales (por ejemplo, cuando los experimentos requieren mucho tiempo para repetirse o tienen elementos humanos). En tales casos, las pruebas múltiples siguen siendo ideales, pero se puede justificar un número limitado de pruebas siempre que se revelen las limitaciones y se discutan los posibles efectos de la estocasticidad.
 - El uso de estudios de casos industriales es importante para demostrar la aplicación en el mundo real de una técnica propuesta, pero los datos industriales generalmente no se pueden compartir. En tales casos, se recomienda que se prepare y distribuya un pequeño ejemplo de código abierto como parte de un paquete de replicación para demostrar cómo se puede aplicar el enfoque.

## Antipatrones

- Informar test de significación (por ejmplo, test de Mann-Whitney Wilcoxon) sin pruebas de effect size (ver **Notas**)
- Realizar múltiples pruebas pero no revelar o discutir la variación entre las pruebas; por ejemplo, informar una medida de central (por ejemplo, mediana) sin ninguna indicación de varianza (por ejemplo, un diagrama de caja).

## Críticas Inválidas

- El artículo no es importante. Tenga cuidado de rechazar trabajos que parezcan "no importantes" (a los ojos de un revisor). La investigación es exploratoria y se trata de asumir riesgos. La investigación claramente motivada y la exploración especulativa son importantes y deben ser recompensadas.
- El artículo solo utiliza algoritmos más antiguos sin referencia a trabajos recientes. El uso de algoritmos más antiguos (y ampliamente entendidos) pueden ser válidos cuando se usan, por ejemplo, (1) como parte de un conjunto más grande que compara muchos enfoques; por ejemplo, (2) ofrecer un método de "hombre de paja" que defina el "piso" del rendimiento (que todo lo demás debe superar); o (3), como un marco de trabajo dentro del cual se cambia una cosa (por ejemplo, la función de calidad) pero todo lo demás permanece constante.
- Que un enfoque no se compare con una línea base inapropiada o no disponible. Si un enfoque de vanguardia carece de una implementación disponible y funcional, no es razonable esperar que el autor vuelva a crear ese enfoque con fines de evaluación comparativa.
- Que un enfoque multi-objetivo no se compare con un enfoque de objetivo único evaluando cada objetivo por separado. Esta no es una comparación significativa porque, en un problema multi-objetivo, la compensación entre los objetivos es un factor importante en la calidad de los resultados. Es más importante considerar las fronteras de Pareto y los indicadores de calidad.
- Que se utilicen uno o muy pocos sujetos, siempre que el trabajo ofrezca una justificación razonable de por qué fue así.

## Lecturas Sugeridas

- Shaukat Ali, Lionel C. Briand, Hadi Hemmati, Rajwinder Kaur Panesar-Walawege. 2010. A Systematic Review of the Application and Empirical Investigation of Search-Based Test Case Generation," in IEEE Transactions on Software Engineering, vol. 36, no. 6, pp. 742-762, DOI: https://doi.org/10.1109/TSE.2009.52
- Andrea Arcuri and Lionel Briand. 2014. A Hitchhiker's guide to statistical tests for assessing randomized algorithms in software engineering. Softw. Test. Verif. Reliab. 24, 3, pp. 219–250. DOI: https://doi.org/10.1002/stvr.1486 
- Amritanshu Agrawal, Tim Menzies, Leandro L. Minku, Markus Wagner, and Zhe Yu. 2020. Better software analytics via DUO: Data mining algorithms using/used-by optimizers." Empirical Software Engineering 25, no. 3. pp.2099-2136. DOI: https://doi.org/10.1007/s10664-020-09808-9
- Efron, Bradley, and Robert J. Tibshirani. An introduction to the bootstrap. CRC press, 1994
- Mark Harman, Phil McMinn, Jerffeson Teixeira Souza, and Shin Yoo. 2011. Search-Based Software Engineering: Techniques, Taxonomy, Tutorial. Empirical Software Engineering and Verification. Lecture Notes in Computer Science, vol. 7007, pp. 1–59. DOI: https://doi.org/10.1007/978-3-642-25231-0_1
- Vigdis By Kampenes, Tore Dybå, Jo E. Hannay, and Dag I. K. Sjøberg. 2007. Systematic review: A systematic review of effect size in software engineering experiments. Inf. Softw. Technol. 49, 11–12 (November, 2007), 1073–1086. DOI:https://doi.org/10.1016/j.infsof.2007.02.015
- M. Li, T. Chen and X. Yao. 2020. How to Evaluate Solutions in Pareto-based Search-Based Software Engineering? A Critical Review and Methodological Guidance. In IEEE Transactions on Software Engineering. DOI: https://doi.org/10.1109/TSE.2020.3036108.
- Nikolaos Mittas and Lefteris Angelis. Ranking and clustering software cost estimation models through a multiple comparisons algorithm. IEEE Trans. Software Eng.,
39(4):537–551, 2013.
- Guenther Ruhe. 2020. Optimization in Software Engineering - A Pragmatic Approach. In  Felderer, M. and Travassos, G.H. eds., Contemporary Empirical Methods in Software Engineering, Springer. DOI: https://doi.org/10.1007/978-3-030-32489-6_9

## Ejemplares

- Hussein Almulla, Gregory Gay. 2020. Learning How to Search: Generating Exception-Triggering Tests Through Adaptive Fitness Function Selection. In Proceedings of 13th IEEE International Conference on Software Testing (ICST’20). IEEE, 63-73. DOI: https://doi.org/10.1109/ICST46399.2020.00017 
- Jianfeng Chen, Vivek Nair, Rahul Krishna, Tim Menzies. “Sampling” as a Baseline Optimizer for Search-Based Software Engineering. IEEE Transactions on Software Engineering 2019 45(6), 2019. DOI: https://doi.org/10.1109/TSE.2018.279092
- José Campos, Yan Ge, Nasser Albunian, Gordon Fraser, Marcelo Eler and Andrea Arcuri. 2018. An empirical evaluation of evolutionary algorithms for unit test suite generation. Information and Software Technology. vol. 104, pp. 207–235. DOI: https://doi.org/10.1016/j.infsof.2018.08.010
- Feather, Martin S., and Tim Menzies. "Converging on the optimal attainment of requirements." Proceedings IEEE Joint International Conference on Requirements Engineering. IEEE, 2002.
- G. Mathew, T. Menzies, N. Ernst and J. Klein. 2017.  "SHORT"er Reasoning About Larger Requirements Models. In 2017 IEEE 25th International Requirements Engineering Conference (RE), Lisbon, Portugal, pp. 154-163. doi: 10.1109/RE.2017.3
- Annibale Panichella, Fitsum Meshesha Kifetew and Paolo Tonella. 2018. Automated Test Case Generation as a Many-Objective Optimisation Problem with Dynamic Selection of the Targets. IEEE Transactions on Software Engineering. vol. 44, no. 2, pp. 122–158. DOI: https://doi.org/10.1109/TSE.2017.2663435
- Federica Sarro, Filomena Ferrucci, Mark Harman, Alessandra Manna and Jen Ren.  2017. Adaptive Multi-Objective Evolutionary Algorithms for Overtime Planning in Software Projects. IEEE Transactions on Software Engineering, vol. 43, no. 10, pp. 898-917. DOI: https://doi.org/10.1109/TSE.2017.2650914
- Federica Sarro, Alessio Petrozziello, and Mark Harman. 2016. Multi-objective software effort estimation. In Proceedings of the 38th International Conference on Software Engineering (ICSE'16). Association for Computing Machinery, New York, NY, USA, 619–630. DOI: https://doi.org/10.1145/2884781.2884830
- Norbert Siegmund, Stefan Sobernig, and Sven Apel. 2017. Attributed variability models: outside the comfort zone. In Proceedings of the 2017 11th Joint Meeting on Foundations of Software Engineering (ESEC/FSE. Association for Computing Machinery, New York, NY, USA, 268–278. DOI: https://doi.org/10.1145/3106237.3106251

## Notas

Con respecto a la diferencia entre los tests de "significancia" y "tamaño del efecto": "Significancia" verifica si las distribuciones se pueden distinguir entre sí, mientras que las pruebas de "effect size" son necesarias para verificar si la diferencia entre distribuciones es "interesante" (y no solo una trivialmente "pequeño efecto"). Estas pruebas pueden ser paramétricas o no paramétricas. Por ejemplo, el código para el t-test/Hedges paramétrico de significancia/efecto respaldado por Kampenese et al. se puede encontrar en https://tinyurl.com/y4o7ucnx.  El código para el test paramétrico Scott-Knot/Cohen del tipo respaldado por Mittas et al. está disponible en https://tinyurl.com/y5tg37fp. El código para el test no paramétrico bootstrap/Cliffs Delta de significancia/efecto del tipo respaldado por Efron et al. y Arcuri et al.
se puede encontrar en https://tinyurl.com/y2ufofgu.

---

<footnote><sup>[1](#myfootnote1)</sup> Tenga en cuenta que existen muchas técnicas de optimización de este tipo (metaheurísticas; optimizadores numéricos; probadores de teoremas de resolución de restricciones SAT, SMT, CSP; y otras), algunas de las cuales son estocásticas.</footnote><br> 
<footnote><sup>[2](#myfootnote2)</sup> Por ejemplo, creación de entradas de pruebas, refactorización de diseño, predicción de esfuerzo.</footnote><br> 
<footnote><sup>[3](#myfootnote3)</sup> Una "función de calidad", o "función objetivo", es una función de puntuación numérica que se utiliza para indicar la calidad de una solución a un problema definido. Los enfoques de optimización intentan maximizar o minimizar tales funciones, dependiendo de si las puntuaciones más bajas o más altas indican éxito.</footnote><br>
<footnote><sup>[4](#myfootnote4)</sup> Por ejemplo, si el producto cruzado del espacio de opciones es muy grande o si el tiempo necesario para realizar una tarea manualmente es muy lento.</footnote><br>
<footnote><sup>[5](#myfootnote5)</sup> Por ejemplo, el optimizador numérico, la metaheurística específica, el método de resolución de restricciones, etc.</footnote><br>
<footnote><sup>[6](#myfootnote6)</sup> Por ejemplo, no utilice un algoritmo como el enfriamiento simulado, o incluso un enfoque específico como NSGA-II, para resolver un problema de optimización a menos que sea realmente apropiado para ese problema. Si bien rara vez se conoce el *mejor* enfoque para un problema nuevo, al menos se deben considerar los algoritmos aplicados para abordar problemas similares y hacer un juicio informado.</footnote><br>
<footnote><sup>[7](#myfootnote7)</sup> Si el enfoque aborda un problema nunca antes abordado, entonces debería compararse, al menos, con una búsqueda aleatoria. De lo contrario, compare el enfoque propuesto con el estado de arte de la técnica existente.</footnote><br>
<footnote><sup>[8](#myfootnote8)</sup> Por ejemplo , un suite de pruebas o caso de prueba en generación de tests.</footnote><br>
<footnote><sup>[9](#myfootnote9)</sup> Por ejemplos, un árbol o una estructura de vector.</footnote><br>
<footnote><sup>[10](#myfootnote10)</sup> Técnicas de ejemplo - Enfriamiento Simulado, Algoritmo Genético. Ejemplo de heurística - Cruce de un punto. Parámetros de ejemplo: tasas de cambio y mutación.</footnote><br>
<footnote><sup>[11](#myfootnote11)</sup> Por ejemplo, datos de propiedad, problemas éticos o un acuerdo de confidencialidad.</footnote><br>
<footnote><sup>[12](#myfootnote12)</sup> Por ejemplo, la estocasticidad puede surgir del uso de algoritmos aleatorios, del uso de una función de calidad que mida una variable aleatoria del entorno (por ejemplo, una función de calidad basada en el tiempo de ejecución puede devolver diferentes resultados en diferentes ejecuciones), del uso de muestreo de datos o enfoques de validación cruzada.</footnote><br>
<footnote><sup>[13](#myfootnote13)</sup> Por ejemplo, el enfoque es demasiado lento, humano en el circuito.</footnote><br>
<footnote><sup>[14](#myfootnote14)</sup> Incluyendo, por ejemplo, el código fuente (del enfoque, la representación de la solución y los cálculos de calidad), los conjuntos de datos utilizados como entrada del experimento y los datos del experimento recopilado (por ejemplo, salidas registros logs, soluciones generadas).</footnote><br>
<footnote><sup>[15](#myfootnote15)</sup> Por ejemplo, si aplica un enfoque de optimización multi-objetivo, entonces utilice un criterio que pueda analizar la frontera de soluciones de Pareto (por ejemplo, distancia generacional y distancia generacional inversa)</footnote><br>
<footnote><sup>[16](#myfootnote16)</sup> Por ejemplo, aplicando optimización de hiperparámetros.</footnote><br>
<footnote><sup>[17](#myfootnote17)</sup> Por lo general, basta con separar los resultados y la discusión en diferentes secciones. Sin especulaciones en la sección de resultados.</footnote><br>
<footnote><sup>[18](#myfootnote18)</sup> Por ejemplo, aplicando optimización de hiperparámetros.</footnote><br>

</standard>
