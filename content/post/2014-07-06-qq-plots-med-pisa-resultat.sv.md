---
title: QQ-plots med Pisa-resultat
author: Richard Öhrvall
date: '2014-07-06'
categories:
  - böcker
  - R
  - statistikprogram
  - Visualisering av data
slug: qq-plots-med-pisa-resultat
---

Sommaren är en utmärkt tid för att experimentera lite med data, metoder och program. Bland allt har jag tänkt använda statistikprogrammet R lite mer än jag brukar (vanligtvis använder jag Stata eller SAS - se min översikt av statistikprogram [här](https://richardohrvall.rbind.io/2014/01/att-valja-statistikprogram/)).

Den här bloggposten är en kombination av ovanstående. En intressant form av grafer är så kallade QQ-plots, eller quantile-quantile plots. De är ett alternativ till histogram om man vill studera fördelningar. Exempelvis kan de användas för att se om datamaterialet är normalfördelat (genom att jämföra en faktisk fördelning med en teoretisk). Eller som i det fall jag tänker titta på här, för att jämföra två olika fördelningar: hur väl pojkar och flickor presterar i Pisa-undersökningen 2012.

I nedanstående QQ-plots jämförs för ett antal länder hur bra flickor och pojkar presterade när det gäller läsförståelse och matematik i Pisa 2012. För respektive kön har eleverna delats in i likstora 100 grupper efter hur väl de presterade, från de sämsta till de sämsta. I diagrammet är flickornas resultat på y-axeln och pojkarnas på x-axeln. Den första punkten i diagrammet (nere till vänster) är alltså resultaten för den percentil som presterade sämst (de sämsta 1 procenten).

Som framgår av diagrammen är flickor bättre på läsförståelse i alla länderna som presenteras här. Skillnaden är rätt stor i Sverige och framför allt i Finland. När det gäller matematik är skillnaderna mindre. I Sverige är de sämsta tjejerna bättre än de sämsta killarna, men de bästa killarna är bättre än de bästa tjejerna. I övriga länder är könsskillnaderna lite större.

Exemplet och koden är hämtad från bloggen [SmarterPoland](http://smarterpoland.pl/index.php/2014/06/gender-gap-and-visualisation-challenge-user2014/), det är bara att kopiera och ändra för den som vill ta fram andra resultat. Om ni vill lära er mer om QQ-plots rekommenderas klassikern Visualizing Data av William S. Cleveland från 1993.

[slideshow_deploy id='2826']
