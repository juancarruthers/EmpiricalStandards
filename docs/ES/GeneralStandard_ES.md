# El Estándar General

<standard name="General Standard">

## Aplicación

Este estándar general aplica a todos los estudios de Ingeniería del Software
que recolectan y analizan datos. Debe ser complementado con guías específicas
cuando sea posible.

## Comprobaciones Iniciales (Editor) 

Reviewers should only be invited for papers with the following
attributes. By assigning reviewers, the editor/chair/administrator is
confirming that the manuscript meets these criteria:
-   Satisface los requerimientos del llamado a presentación del trabajo: cantidad de páginas, palabras claves adecuadas,
    anonimización, etc.
-   El tema del trabajo se enmarca en el alcance del llamado a presentación.
-   Satisface un nivel mínimo aceptable en la calidad del idioma en el que se encuentra
    escrito el trabajo.
-   Cita fuentes académicas
-   Presenta resultados no previamente publicados y aceptados en revistas o eventos
    académicos con revisión por pares.
-   No incluye texto literal publicado y no atribuido a la fuente
    (como plagio)

### Comprobaciones Iniciales (Revisor)

Los trabajos deberían ser revisados por pares evaluadores siempre que tengan los
siguientes criterios:
-   El revisor no tiene conflicto de interés con
    el trabajo a revisar.
-   El revisor tiene suficiente experiencia; if unsure, check with the chair
    or editor and clarify what you can(not) evaluate
-   El trabajo es claro tanto en lenguaje como en su formato de presentación.

## Atributos Específicos

### Atributos Esenciales

<checklist name="Essential"> 

<intro>    
    
- [ ]	Establece un propósito, problema, objetivo o pregunta de investigación
- [ ]	Explica por qué el propósito, problema, etc. es importante (motivación)
- [ ]	Define la jerga, los acrónimos y los conceptos clave

<method>
    
- [ ]	La metodología es apropiada (no necesariamente óptima) para el propósito, problema, etc.
- [ ]	Describe en detalle qué, dónde, cuándo y cómo se recopilaron los datos (consultar el [Suplemento de Muestreo](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/Sampling.md))
- [ ]	Describe en detalle cómo se analizaron los datos


<results>
    
- [ ]	Presenta los resultados
- [ ]	Los resultados abordan directamente las preguntas de la investigación
- [ ]	Enumera y valida los supuestos de las pruebas estadísticas utilizadas (si las hubiera)<sup>[1](#myfootnote1)</sup>

<discussion>
 
- [ ]	Analiza las implicaciones de los resultados
- [ ]	Analiza las limitaciones del estudio y las amenazas a la validez (threats to validity)
- [ ]	Apoya las principales afirmaciones o conclusiones con evidencia explícita (datos / observaciones) o argumentos

<other> 
  
- [ ]	Contribuye de alguna manera al cuerpo de conocimientos
- [ ]	El lenguaje no es engañoso; cualquier problema gramatical no obstaculiza sustancialmente la comprensión
- [ ]	Reconoce y mitiga los posibles riesgos, daños o consecuencias no deseadas de la investigación (consultar la entrada suplementaria de Ética para [Investigacion de Ingenieria](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/EthicsEngineering.md), [Participantes Humanos](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/EthicsHumanParticipants.md), o [Datos Secundarios](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/EthicsSecondaryData.md))
- [ ]	Las visualizaciones / los gráficos no son engañosos (consultar el [Suplemento de Visualizacion de Informacion](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/InformationVisualization.md))
- [ ]	Cumple con todos los estándares empíricos aplicables

</checklist>
     
### Atributos Deseables

<checklist name="Desirable">

- [ ]	Establece la postura epistemológica<sup>[2](#myfootnote2)</sup>
- [ ]	Resume y sintetiza una selección razonable de trabajos relacionados (no necesariamente todos los estudios relevantes)
- [ ]	Describe claramente la relación entre las contribuciones y los trabajos relacionados
- [ ]	Demuestra potencia estadística apropiada (para trabajo cuantitativo) o saturación (para trabajo cualitativo)
- [ ]	Describe intentos razonables de estudiar o mitigar las limitaciones
- [ ]	Discute el realismo del estudio, los supuestos y la sensibilidad de los resultados
- [ ]	Proporciona interpretaciones o recomendaciones potencialmente útiles para la industria, la educación o la investigación.
- [ ]	Presentación concisa, precisa, bien organizada y fácil de leer.
- [ ]	Las visualizaciones (por ejemplo, gráficos, diagramas, tablas) promueve los argumentos o la contribución del artículo.
- [ ]	Aclara los roles y responsabilidades de los investigadores (es decir, quién hizo qué?)
- [ ]	Proporciona una autorreflexión o evaluación del propio trabajo de los autores (por ejemplo, lecciones aprendidas)
- [ ]	Publica el estudio en dos fases: un plan y los resultados de la ejecución del plan (consultar el [Suplemento de Registro de Informes](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/RegisteredReports.md))
- [ ]	Utiliza varios evaluadores, cuando sea filosóficamente apropiado, para realizar juicios subjetivos (consultar el [Suplemento de IRR/IRA](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/InterRaterReliabilityAndAgreement.md))

</checklist>
     
### Atributos Extraordinarios	
<checklist name="Extraordinary">

- [ ]	Aplica dos o más estrategias de recopilación o análisis de datos a la misma pregunta de investigación (consultar la entrada de [Estandar Multimetodologico](https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/MixedMethods.md))
- [ ]	Aborda la (s) misma (s) pregunta (s) de investigación desde múltiples perspectivas epistemológicas
- [ ]	Innova en la metodología de investigación mientras completa un estudio empírico

</checklist>

## Criterios Generales de Calidad

No existen criterios de calidad universales. Cada estudio debe evaluarse
en función de los criterios de calidad adecuados para su metodología, tal como se establece
en los estándares **empíricos específicos**. Evite aplicar criterios de calidad inapropiados
(por ejemplo, validez de constructo a un estudio sin constructos;
validez interna a un estudio sin relaciones causales).

### Ejemplos de Desviaciones Aceptables

Un estudio solo puede aplicar un **estándar empírico** si existe un estándar
apropiado. Si no existen estándares relacionados, los estudios deben aplicar
las guías publicadas. Si no existe una guía adecuada, los revisores deben
aplicar el estándar general y construir un esquema de evaluación ad hoc
para el nuevo método.

## Prácticas de Buenas Revisiones

Los revisores evalúan la confiabilidad, la importancia y la claridad de un
manuscrito. Los resultados deben ser, principalmente, verdaderos (confiables)
y, en segundo lugar, importantes. Se puede aceptar un artículo confiable incluso
si no es importante. No se puede aceptar un artículo que no sea confiable, aunque
parezca importante. Los artículos que son importantes y dignos de confianza
pueden tener prioridad. Los artículos deben ser lo suficientemente claros para
juzgar su confiabilidad e importancia. Los revisores deben esforzarse por:
-   Reflexionar y exponer claramente sus propias limitaciones y prejuicios.
-   Aclarar cuáles son los cambios necesarios y cuáles son los cambios sugeridos.
    Idealmente, sepárelos.
-   Identificar las partes del documento que no pueda juzgar de manera efectiva o que
    no revisó.

## Revisando Antipatrones
-   Aplicar estándares empíricos de manera mecánica, inflexible, marcando casillas o siguiendo una receta.
-   Rechazar un estudio porque utiliza una metodología para la que no se dispone de un estándar específico.
-   Hojear un manuscrito en lugar de leer cuidadosamente cada palabra e inspeccionar cada figura y tabla.
-   Emplear un tono poco profesional o mordaz, ataques ad hominem, comentarios despectivos o denigrantes.
-   Permitir que las identidades o afiliaciones de los autores afecten la revisión.
-   Centrarse en los detalles superficiales del trabajo sin comprometerse con sus principales afirmaciones o resultados.
-   Solicitar un análisis adicional que no esté directamente relacionado con el propósito de un estudio o la pregunta 
    de investigación, lo que lleva a resultados mal vinculados a la narrativa del artículo.
-   Tercializar la revisión con otras personas cuando el lugar no lo permita explícitamente.
-   Usar la revisión para promover las propias opiniones, teorías, métodos o publicaciones del revisor.

## Críticas Inválidas
-   Establecer tamaños de muestra mínimos arbitrarios u otros requisitos de datos, sin basarse ni en el análisis de potencia estadística ni en la saturación teórica.
-   Declarar que un estudio:
    - Carece de detalles sin enumerar los detalles que faltan; o
    - es de baja calidad sin explicar problemas específicos;
    - no es nuevo sin citar estudios publicados que hacen contribuciones **prácticamente idénticas**.
-   Rechazar un estudio porque replica o reproduce un trabajo existente
-   Crítica transparadigmática (por ejemplo, atacar un estudio interpretativo por no ajustarse a las normas positivistas).
-   Criticar un estudio por limitaciones intrínsecas a ese tipo de estudio o la metodología utilizada (por ejemplo, atacar un estudio de caso por baja generalización)
-   Rechazar un estudio porque el revisor habría utilizado una metodología o diseño diferente
-   Rechazar un estudio porque reporta resultados negativos
    
## Antipatrones Investigados e Informados 
-   Intentar un estudio sin leer, comprender y aplicar las pautas publicadas para ese tipo de estudio.
-   Estudios irracionalmente pequeños, con poca potencia estadística o limitados.
-   Hipotetizar después de que se conozcan los resultados (del inglés "Hypothesizing After Results are Known" o HARKing) en una investigación (pos) positivista, aparentemente confirmatoria.
-   Informar solo el subconjunto de pruebas estadísticas que producen resultados significativos (p-hacking).
-   Informar, juntos en un artículo, varios estudios inmaduros o inconexos en lugar de un estudio completamente desarrollado.
-   Dividir innecesariamente la presentación de un solo estudio en muchos trabajos.
-   Extraer conclusiones o generalizaciones; ofuscar, restar importancia o descartar las limitaciones de un estudio.
-   Mencionar trabajos relacionados solo para descartarlos como irrelevantes; enumerar en lugar de sintetizar los trabajos relacionados.
-   Reconocer las limitaciones, pero luego escribir implicaciones y conclusiones como si las limitaciones no existieran.

---  
<footnote><sup>[1](#myfootnote1)</sup> los métodos visuales para verificar los supuestos son a menudo tan buenos o mejores que las pruebas estadísticas</footnote><br>
<footnote><sup>[2](#myfootnote2)</sup> p. Ej. positivismo, falisificacionismo, interpretivismo, realismo crítico, posmodernismo)</footnote><br>
</standard>

