---
layout: default      
title: Acerca De
permalink: /about/
---   

{% capture std %}{% include_relative README_ES.md %}{% endcapture %}

{{ std | markdownify }}
