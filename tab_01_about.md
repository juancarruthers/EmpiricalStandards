---
layout: default      
title: Acerca De
permalink: /about/
---   

{% capture std %}{% include_relative README.md %}{% endcapture %}

{{ std | markdownify }}
