---
title: Visualisering av vädret i Stockholm
author: Richard Öhrvall
date: '2017-01-24'
categories:
  - R
  - statistikprogram
  - Visualisering av data
slug: visualisering-av-vadret-i-stockholm
---

Ett nytt år har inletts. Min förhoppning är att 2017 ska visa sig vara ett produktivt år. Jag har även tänkt börja använda statistikprogrammet R i högre grad än tidigare. Det finns ett flertal skäl till det beslutet, men framför allt finns en växande rörelse kring programmet och inom den skapas en stadigt ökande mängd av nya, spännande funktioner.

Det bästa sättet att komma in i ett nytt statistikspråk är att använda det praktiskt. Så jag bestämde mig därför att försöka ta fram en variant av Edward Tuftes klassiska visualisering i NY Times av vädret under årets olika dagar. Det är en graf som har blivit känd genom Tuftes inflytelserika bok _[Visual Display of Quantitative Information](https://www.edwardtufte.com/tufte/books_vdqi). _

![](/img/wp/00014g-836.jpg)

Grafen har två delar. I den övre delen redovisas temperaturen för årets alla 365 dagar i vad som vid första anblick ser ut som tre linjer av olika tjocklek, men som egentligen är tre typer av staplar som ligger mycket tätt:

  1. Staplar som visar intervallet från den lägsta till den högsta temperaturen för respektive dag det aktuella året (staplarna i den lila färgen).

  2. Staplar som visar intervallet från den lägsta till den högsta temperaturen för respektive dag historiskt sett (de ljusa staplarna).

  3. Staplar som visar intervallet från den genomsnittligt lägsta temperaturen historiskt sett till den genomsnittlig högsta temperaturen historiskt sett.

Dessutom finns kumulativ nederbörd per månad redovisat i grafens nederkant.

Jag upptäckte att Brad Boehmke redan hade [skrivit kod i R](http://rpubs.com/bradleyboehmke/weather_graphic) för att ta fram en sådan graf. Den skiljer sig något från NY Times graf, framför allt genom att han inte hade tillgång till högsta och lägsta temperatur för respektive dygn, utan endast dygnsmedeltemperaturen. I hans grafen blir därmed det aktuella årets temperatur över dagar illustrerat som en linje. Dessutom hade han inte tillgång till nederbörd, så den delen av den ursprungliga grafen finns inte med. Men jag tycker ändå att hans resultat blev bra, se själva:

![](/img/wp/ladda-ned.png)

Så jag har utgått från den koden, men jag har ändrat den en del. Bland annat fick jag inte hans numrering av dagar att fungera och jag förstod inte varför han ritade samma graf för varje historiskt år. Dessutom valde Boehmke att låta intervallet avseende normala år representeras av konfidensintervallet för det historiska medelvärdet. Detta då han som sagt inte hade tillgång till varje dygns högsta och lägsta temperatur. Jag tycker inte att det är helt lyckat val då det visar osäkerheten i en skattning av ett historiskt medelvärde snarare än ett intervall som innefattar normala värden.

Man skulle i stället kunna låta intervallet motsvara två standardavvikelser i datamaterialet (dvs. inte dela med roten ur n) i förhållande till medelvärdet. Men jag föredrar att låta intervallet "normala temperaturer" avse de mittersta 50 procenten av tidigare års medeltemperaturer. Med andra ord: om man sorterar alla tidigare års medeltemperaturer för en viss dag från den lägsta till den högsta temperaturen så blir de procent av dagarna som ligger i mitten de dagar som betecknas "normala". Staplarna i grafen blir därmed en variant av ett [lådagram ](https://sv.wikipedia.org/wiki/L%C3%A5dagram)(eller boxplot på engelska), där den mörkare färgen blir själva lådan.

En rolig utveckling av Tuftes graf är att Boehmke har markerat de dagar som det aktuella året har rekordhög eller rekordlåg medeltemperatur. Det tillför något nytt och jag därför behållit den delen.

Jag har valt att illustrera medeltemperaturen i Stockholm 2016. Data har jag hämtat från SMHI. Där har jag hämtat historisk data från och med 1961. Och den resulterande grafen för vädret i Stockholm 2016 blev så här (klicka på grafen för att förstora):

![](/img/wp/sthm_2016x.png)

Inte så långt från originalet, eller hur? Möjligen skulle man kunna ändra proportionerna för att få grafen mer avlång som i Tuftes version, men jag gillar den nuvarande utformningen. Jag har även som ett experiment skapat en ny [blogg ](https://richardohrvall.github.io/)där jag kommer att lägga ut mer kring statistik och kodande. Det är en blogg som jag skapat direkt i statistikprogrammet R med hjälp av paketet [Blogdown](https://github.com/rstudio/blogdown). Där har jag lagt ut koden för att skapa den här grafen, se [det här inlägget](https://richardohrvall.github.io/2017/01/23/visualisering-av-temperaturen-i-stockholm-2016/), om ni vill utveckla den ytterligare.

Hos SMHI finns än äldre data och det finns även uppgifter om högsta och lägsta temperatur respektive dygn och om nederbörd, så det går att göra en graf som än mer liknar originalet, men det får bli en senare uppgift.
