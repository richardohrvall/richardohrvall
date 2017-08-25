---
title: Venn och Euler
author: Richard Öhrvall
date: '2012-03-08'
categories:
  - Visualisering av data
slug: venn-och-euler
---

Med det ökande intresset för visualiseringar av data har Euler- och framför allt Venndiagrammen fått en renässans. Det har på senare tid skrivits en del bra om dessa diagram på olika håll, så jag passar på att skriva ned några rader och ge ett par länkar (se längst ned).

Venndiagram är diagram som visar _alla_ logiskt möjliga kombinationer mellan mängder (klasser). De används flitigt i mängdlära. Vanligen tar de formen av två eller tre överlappande cirklar. I bilden nedan ses ett Venndiagram med cirkel A och B.

![](/img/wp/venn_a_b.png)

Allt som befinner sig inom cirkel A tillhör en viss kategori (eller mängd) och allt som befinner sig utanför cirkeln tillhör inte den kategorin. Samma gäller för cirkel B. Exempelvis kan vi tänka oss att cirkel A representerar hundar och cirkel B skådespelare. Den del av diagrammet faller inom både cirkel A och B brukar kallas snittet av A och B och avser dem som tillhör både kategori A och B, vilket i det här exemplet blir skådespelande hundar, såsom Rin Tin Tin, Lassie och Uggie. Den del av diagrammet som är inom antingen A eller B (tillhör minst en av kategorierna) brukar kallas unionen av A och B. Eftersom Venndiagram ska innehålla alla logiskt möjliga kombinationer av de kategorier som redovisas blir det komplext om antalet kategorier är många, så vanligen innehåller diagrammen två eller tre kategorier (ofta i form av cirklar).

![](http://blog.visual.ly/wp-content/uploads/2012/01/625x628xWorld_Reduced_to_Infographics_pg_33-1.png,q547b7b.pagespeed.ic.hdZ3CaEhqa.png)

_Bilden ovan är hämtad från [The World Reduced to Infographics](http://www.amazon.com/World-Reduced-Infographics-Hollywoods-Sociopathic/dp/1569759898) av Patrick Casey och Worm Miller._

Venndiagram kan ses som en underkategori till Eulerdiagram. Eulerdiagram behöver inte ha restriktionen att diagrammet ska innefatta alla möjliga kombinationer av de olika klasser som redovisas. De innefattar därmed fler typer av diagram än Venndiagram. Eulerdiagram brukar bland annat användas för att beskriva statistiska urvalsundersökningar, som i bilden nedan. Där har vi hela populationen, t.ex. svenska medborgare 18 år och äldre, ur vilken vi drar ett urval (sample). De som ingår i urvalet kontaktas sedan på något sätt, men tyvärr vill inte alla vara med i undersökningen, så de svarande blir en delmängd av dem i urvalet. Ofta komplicerar man bilden ytterligare genom att skilja på den population vi avser att undersöka och den population som ingår i den urvalram (den lista från vilken vi drar urvalet) vi har att tillgå när vi gör undersökningen.

![](/img/wp/Urval.png)

Det är förhållandevis enkelt att skapa ett Venn- eller Eulerdiagram i en mängd programvaror. Vanligen är inte kategorierna redovisade i storlekar som är proportionella mot deras faktiska storlekar. Om man ändå vill ha mer kontroll över proportionerna och även vill koppla dem till befintliga data är alternativen färre. I statistikprogrammet Stata finns det användarskrivna kommandot -pvenn-, som kan installeras via -ssc install pvenn- och som kan ta fram Venndiagram. Tyvärr blir det inte riktigt så snyggt som man skulle önska (diagrammet med cirkel A och B ovan är skapat i Stata). I statistikprogrammet R (fantastiskt gratisprogram) finns däremot funktionen [venneuler()](http://www.cs.uic.edu/~wilkinson/Publications/venneuler.pdf) som kan hantera både Venn- och Eulerdiagram och dessutom resulterar i ett riktigt snyggt resultat.

Venndiagram kan ofta användas för att illustrera roliga samband, som i diagrammet av Stehpen Wildish nedan (se fler Venndiagram av Stephen Wildish [här](http://www.buzzfeed.com/burnred/clever-venn-diagrams-by-stephen-wildish-281t)).

![](http://s3-ec.buzzfed.com/static/enhanced/web05/2012/3/4/8/enhanced-buzz-22604-1330869081-6.jpg)

_Läs bra inlägg om Euler- och Venndiagram hos [visual.ly](http://blog.visual.ly/euler-and-venn-diagrams/) och [EagerEyes](http://eagereyes.org/techniques/venn-diagrams). Även Wikipedia har matnyttig information om [Venndiagram ](http://en.wikipedia.org/wiki/Venn_diagram)och [Eulerdiagram](http://en.wikipedia.org/wiki/Euler_diagram). För den som blir riktigt biten rekommenderas [den tredje internationella workshopen kring Eulerdiagram](http://www.diagrams-conference.org/2012/content/3rd-international-workshop-euler-diagrams)._
