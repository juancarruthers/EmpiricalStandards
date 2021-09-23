---
layout: default
title: Suplementos
permalink: /Supplements/
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
  width: 25%;
}

.tablinks:hover {
  background-color: #ddd;
}

.tab {
  padding-bottom: 80px;
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
function openSupplementFromURL(evt) {
  supplementName = getParameterByName('supplement')[0].replaceAll('"', '');

  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(supplementName).style.display = "block";
  document.getElementById(supplementName+'_b').className += " active";
}
</script>
</head>
<body onload="openSupplementFromURL(event)">

<div class="tab">
  <button id="EthicsEngineering_b"           class="tablinks" onclick="openSupplement(event, 'EthicsEngineering')">Ethics (Engineering Research)</button>
<div class="tab">
  <button id="EthicsHumanParticipants_b"           class="tablinks" onclick="openSupplement(event, 'EthicsHumanParticipants')">Ética (Participantes Humanos)</button>
  <button id="EthicsSecondaryData_b"               class="tablinks" onclick="openSupplement(event, 'EthicsSecondaryData')">Ética (Datos Secundarios)</button>
  <button id="InformationVisualization_b"          class="tablinks" onclick="openSupplement(event, 'InformationVisualization')">Visualización de la Información</button>
  <button id="InterRaterReliabilityAndAgreement_b" class="tablinks" onclick="openSupplement(event, 'InterRaterReliabilityAndAgreement')">IRR/IRA</button>
  <button id="OpenScience_b"                       class="tablinks" onclick="openSupplement(event, 'OpenScience')">Ciencia Abierta</button>
  <button id="RegisteredReports_b"                 class="tablinks" onclick="openSupplement(event, 'RegisteredReports')">Reportes Registrados</button>
  <button id="Sampling_b"                          class="tablinks" onclick="openSupplement(event, 'Sampling')">Muestreo</button>
</div>

<div id="EthicsEngineering" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/EthicsEngineering_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="EthicsHumanParticipants" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/EthicsHumanParticipants_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>
  
  
<div id="EthicsSecondaryData" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/EthicsSecondaryData_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="InformationVisualization" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/InformationVisualization_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="InterRaterReliabilityAndAgreement" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/InterRaterReliabilityAndAgreement_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="OpenScience" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/OpenScience_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="RegisteredReports" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/RegisteredReports_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<div id="Sampling" class="tabcontent">
  <p>
    {% capture std %}{% include_relative Supplements/ES/Sampling_ES.md %}{% endcapture %}
    {{ std | replace: '- [ ]', '-' | markdownify }}
  </p>
</div>

<script>
function openSupplement(evt, supplementName) {
  var i, tabcontent, tablinks;

  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(supplementName).style.display = "block";
  evt.currentTarget.className += " active";
  window.history.replaceState('', '', '?supplement='+supplementName);
}
</script>
   
</body>
</html> 
