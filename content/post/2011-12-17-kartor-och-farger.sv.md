---
title: Kartor och färger
author: Richard Öhrvall
date: '2011-12-17'
categories:
  - kartor
  - Visualisering av data
slug: kartor-och-farger
---

En vanlig form av kartor är så kallade [koropletkartor](http://en.wikipedia.org/wiki/Choropleth_map). Det är en form av tematiska kartor där områden får en viss färg (eller ett visst mönster) baserat på värdet för den statistiska variabel man vill illustrera, t.ex. kan man illustrera stödet för Socialdemokraterna efter kommun genom att ge kommunerna en röd färg som är mörkare ju starkare stöd partiet har i kommunen. Oftast delar man in områdena i klasser och ger alla områden i en viss klass samma färg, t.ex.genom alla kommuner där S har över 60 procents stöd får den mörkaste rödfärgen osv. Då måste man välja hur många klasser man vill ha och var gränserna mellan dessa klasser ska gå (man kan i och för sig även välja att ha en kontinuerlig skala). Beroende på dessa två val kan kartan förmedla olika intryck. Det visas på ett tydligt sätt på[ den här sidan](http://gabrielflor.it/counties). Det är även illustrerat på den utmärkta[ bloggen Vis4.net](http://vis4.net/blog/posts/choropleth-maps/) där följande bild är hämtad från:

![](http://vis4.net/blog/wp-content/uploads/2011/12/choropleth-classes.gif)

Kartan avser andel fattiga i USA och att diskussionen har kommit upp beror på ett inlägg på Guardians datablogg som kan läsas [här](http://www.guardian.co.uk/news/datablog/interactive/2011/sep/15/us-poverty-mapped). Märk väl att det är samma data som illustreras i den animerade bilden ovan, det enda som varierar är antalet klasser som används. Hur dessa data bäst illustreras diskuteras vidare [här](http://www.excelcharts.com/blog/the-same-data-the-same-map-different-stories/).

Ett ytterligare val är vilka färger som ska väljas för respektive klass. Det gäller att välja färger som uppfattas vara på samma avstånd från varandra som de klasser de ska illustrera. Här kan man få hjälp genom att använda tjänsten [Colorbrewer2](http://colorbrewer2.org/). Det viktiga här är att färger som ifråga om ljusstyrka befinner sig på samma avstånd från varandra kan uppfattas på annat sätt, och det är hur färgerna uppfattas som är det centrala. Den som vill nörda ner sig rejält kring färgval kan läsa vidare [här](http://vis4.net/blog/posts/avoid-equidistant-hsv-colors/). Ett besläktat tema gäller färgskalor som går från rött till grönt, vilka bör undvikas om man bryr sig om de färgblinda, läs mer [här](http://vis4.net/blog/posts/goodbye-redgreen-scales/).

Finns med andra ord en hel del att tänka på när det gäller statistik redovisad i kartform. Och en lärdom är att det intryck som en karta ger kan bero på beslut fattade av den den som gjort kartan.
