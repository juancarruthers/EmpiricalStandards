---
layout: default
title: Estándares
permalink: /docs/
---   

<html>
<head>
<style>
.tablinks {
  background-color: #inherit;
  color: black;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 4px 10px;
  font-size: 17px;
  height: 50px;
  width: 20%;
}

.tablinks:hover {
  background-color: #ddd;
}

.tab {
  padding-bottom: 130px;
}

.tab button.active {
  background-color: #ccc;
}

.tabcontent {
  color: black;
  display: none;
  padding: 10px 20px;
  height: 100%;
}
</style>
<script src="../form_generator/js/read_standards.js"></script>
<script>
function openStandardFromURL(evt) {
  standardName = getParameterByName('standard')[0].replaceAll('"', '');

  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(standardName).style.display = "block";
  document.getElementById(standardName+'_b').className += " active";
}
</script>
</head>
<body onload="openStandardFromURL(event)">

<div class="tab">
  <button id="GeneralStandard_b"        class="tablinks" onclick="openStandard(event, 'GeneralStandard')">Estándar general</button>
  <button id="ActionResearch_b"         class="tablinks" onclick="openStandard(event, 'ActionResearch')">Investigación Acción</button>
  <button id="Benchmarking_b"           class="tablinks" onclick="openStandard(event, 'Benchmarking')">Benchmarking</button>
  <button id="CaseStudy_b"              class="tablinks" onclick="openStandard(event, 'CaseStudy')">Estudio de caso</button>
  <button id="CaseSurvey_b"             class="tablinks" onclick="openStandard(event, 'CaseSurvey')">Encuesta de Caso</button>
  <button id="DataScience_b"            class="tablinks" onclick="openStandard(event, 'DataScience')">Ciencia de Datos</button>
  <button id="EngineeringResearch_b"    class="tablinks" onclick="openStandard(event, 'EngineeringResearch')">Investigación en Ingeniería</button>
  <button id="Experiments_b"            class="tablinks" onclick="openStandard(event, 'Experiments')">Experimentos</button>
  <button id="GroundedTheory_b"         class="tablinks" onclick="openStandard(event, 'GroundedTheory')">Teoría Fundamentada</button>
  <button id="Longitudinal_b"           class="tablinks" onclick="openStandard(event, 'Longitudinal')">Estudios Longitudinales</button>
  <button id="MetaScience_b"            class="tablinks" onclick="openStandard(event, 'MetaScience')">Meta-Ciencia</button>
  <button id="MixedMethods_b"           class="tablinks" onclick="openStandard(event, 'MixedMethods')">Métodos Mixtos</button>
  <button id="OptimizationStudies_b"    class="tablinks" onclick="openStandard(event, 'OptimizationStudies')">Estudios de Optimización</button>
  <button id="QualitativeSurveys_b"     class="tablinks" onclick="openStandard(event, 'QualitativeSurveys')">Encuestas Cualitativas</button>
  <button id="QuantitativeSimulation_b" class="tablinks" onclick="openStandard(event, 'QuantitativeSimulation')">Simulación Cuantitativa</button>
  <button id="QuestionnaireSurveys_b"   class="tablinks" onclick="openStandard(event, 'QuestionnaireSurveys')">Encuestas de Cuestionarios</button>
  <button id="RepositoryMining_b"       class="tablinks" onclick="openStandard(event, 'RepositoryMining')">Minado de Repositorios</button>
  <button id="SystematicReviews_b"      class="tablinks" onclick="openStandard(event, 'SystematicReviews')">Revisión Sistemática</button>
</div>
<br>
<br>
<div id="GeneralStandard" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/GeneralStandard_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="General Standard">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="ActionResearch" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/ActionResearch_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Action Research">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>
    <div id="Benchmarking" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/Benchmarking_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Benchmarking (of Software Systems)">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="CaseStudy" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/CaseStudy_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Case Study and Ethnography">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="CaseSurvey" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/CaseSurvey_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Case Survey">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="DataScience" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/DataScience_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Data Science">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="EngineeringResearch" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/EngineeringResearch_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Engineering Methods">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="Experiments" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/Experiments_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Experiments (with Human Participants)">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="GroundedTheory" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/GroundedTheory_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Grounded Theory">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="Longitudinal" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/Longitudinal_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Longitudinal">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>
<div id="MetaScience" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/MetaScience_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Meta Science">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>
<div id="MixedMethods" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/MixedMethods_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Mixed Methods">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="OptimizationStudies" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/OptimizationStudies_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Optimization Studies">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="QualitativeSurveys" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/QualitativeSurveys_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Qualitative Surveys (Interview Studies)">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="QuantitativeSimulation" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/QuantitativeSimulation_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Simulation">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="QuestionnaireSurveys" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/QuestionnaireSurveys_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Questionnaire Surveys">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="RepositoryMining" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/RepositoryMining_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Repository Mining">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<div id="SystematicReviews" class="tabcontent">
  <p>
    {% capture std %}{% include_relative docs/ES/SystematicReviews_ES.md %}{% endcapture %}
    {{ std | remove: '<standard name="Systematic Reviews">' | remove: '<checklist name="Essential">' | remove: '<checklist name="Desirable">' | remove: '<checklist name="Extraordinary">' | remove: '</checklist>' | remove: '</standard>' | remove: '<footnote>' | remove: '</footnote>' | remove: '<intro>' | remove: '<method>' | remove: '<results>' | remove: '<discussion>' | remove: '<other>' | replace: '- [ ]', '-' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/docs/', '../docs?standard=' | replace: 'https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Supplements/', '../Supplements?supplement=' | replace: '.md', '' | markdownify }}
  </p>
</div>

<script>
function openStandard(evt, standardName) {
  var i, tabcontent, tablinks;

  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(standardName).style.display = "block";
  evt.currentTarget.className += " active";
  window.history.replaceState('', '', '?standard='+standardName);
}
</script>
   
</body>
</html> 
