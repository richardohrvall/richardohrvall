---
title: Kombinera Zotero med Dropbox
author: Richard Öhrvall
date: '2016-07-01'
categories:
  - workflow
  - Zotero
slug: kombinera-zotero-med-dropbox
---

Jag har i ett tidigare blogginlägg beskrivit [hur mitt val av referenshanteringssystem landade i Zotero](https://richardohrvall.rbind.io/2016/04/val-av-referenshanteringssystem-zotero/) och i ett annat [gett tips om hur man kommer igång med Zotero](https://richardohrvall.rbind.io/2016/05/kom-igang-med-zotero/). Som jag nämnde i det senare inlägget kan man i Zotero, under Inställningar och fliken Avancerat\Filer och kataloger, ställa in att Zotero ska ha relativa länkar. Det är att föredra om man vill ha Zotero installerat på olika datorer. På den fliken kan man välja en Baskatolog under vilken man har samma mappstruktur på alla datorer, t.ex. den mapp där du har dina Zotero-filer på datorn. Var Zotero ska lagra sina filer anges under Lagringsplats. Där hamnar databasfilen med dina referenser, men även alla pdf:er du importerar i Zotero och en del annat.

Det är gratis att lagra filer som synkroniseras i Zotero, men bara upp till 300 MB. Sedan kan man köpa ytterligare lagringsutrymme, till ett rimligt pris. Men om man redan betalar för Dropbox (eller någon annan tjänst för lagring av data i molnet) kan ett alternativ vara att lägga filerna där istället. Den första tanken är kanske att göra det genom att under den ovan nämnda fliken ställa in att mappen med Zotero-filer ska ligga under Dropbox-mappen.  På Zoteros webbsida och många andra håll framhålls att det inte är att rekommendera. Detta eftersom det då finns risk att Zoteros och Dropbox olika  synkroniseringar hamnar i konflikt med varandra och din databasfil med alla referenser förstörs. Jag testade detta själv ett tag och råkade inte ut för detta, men däremot fick jag en del problem med Dropbox synkronisering (och ett antal "conflicted copies" av databasfilen), så rekommendationen är förmodligen klok.

Vad finns det då för andra lösningar? På några ställen föreslås att man slår av Dropbox:s synkronisering av just databasfilen. Den ligger direkt under din Zotero-mapp och heter zotero.sqlite. Jag har dock bara lyckats stänga av synkronisering av specifika mappar i Dropbox, och då mappen med alla pdf:er ligger i en undermapp till där databasfilen funkar inte det (för vi vill ju att pdf:erna ska synkroniseras).

Ett alternativ som däremot funkar är att använda så kallade symboliska länkar. Du slår av Zotero, letar upp din Zotero-mapp (den ligger där du valt i den ovan nämnda fliken där lagring anges i Zotero - OBS! Den ska alltså inte ligga under din Dropbox-mapp), klipper ut undermappen 'storage' och klistrar in den någonstans under din Dropbox-mapp, t.ex. i en ny mapp som du döper till Zotero (kom dock ihåg var!). Sedan ska vi skapa en symbolisk länk så att Zotero tror att mappen finns kvar. I Windows gör vi det genom att starta kommandoprompten i Richard Öhrvallistratörsläge (skriv cmd.exe i start-menyn, högerklicka och välj "Kör som Richard Öhrvallistratör"). I kommandoprompten skriver du  mlink _sökväg-till-där-mappen-låg_ _sökväg-till-där-du-lagt-mappen-i-dropbox_  /d och trycker enter. Till exempel kan det se ut så här

![Skärmklipp](/img/wp/Skärmklipp-3.png)

För att kolla att allt blev korrekt, kan du sedan gå till mappen där den mapp som du flyttade låg. Det ska där nu finnas en länk och om du klickar på den ska du hamna i mappen där den nu ligger, dvs. under Dropbox-mappen.

Ett annat alternativ för att kombinera Zotero med Dropbox, som även har andra fördelar, är att använda Zotfile. Det är ett tillägg till Zotero och laddas ned [här](http://zotfile.com/#install-zotfile). Om du använder Zotero i Firefox är det bara att installera det som ett tillägg. Ifall du använder någon annan webbläsare och därför Zotero som fristående program laddar du ned .xpi-filen. Sedan är det bara att i Zoteros menysystem välja Verktyg/Tillägg, klicka på det lilla kugghjulet och välja "Install Add-on From File".

För ändra inställningar i Zotfile är det bara klicka sig fram samma väg, det vill säga via Verktyg/Tillägg och sedan klicka på Options för tillägget Zotfile, som nu ska finnas där.  Under General Settings kan man välja var Zotero ska lagra alla pdf:er.  Dessutom kan man välja hur Zotero ska döpa mapparna. I vanliga fall använder Zotero en namnsättning som är helt obegriplig (som t.ex. Itunes gör, om någon fortfarande använder det).  Jag har valt "/%F/%y", vilket innebär att pdf:erna läggs i mappar efter författarnamn och år, se bilden nedan.

![Skärmklipp](/img/wp/Skärmklipp-4.png)

Under fliken "Renaming Rules" kan man välja hur Zotero ska döpa pdf-filerna. Jag har valt "{%a_}{%y_}{%t}", vilket innebär författare_år_titel. Och jag har valt maximalt två författare och "et al." om antalet författare är mer än två. Detta kan man så klart ställa in på olika sätt beroende på tycke och smak.  Zotfile gör det även lättare att läsa pdf:er i en läsplatta och där markera citat, men det får jag återkomma till i ett annat inlägg.

Efter att man har använt några av dessa sätt att lagra pdf:er i Dropbox kan man gå in i Zotero under Verktyg/Inställningar/Synkronisera och under fliken Inställningar bocka ur rutan för att synkronisera bifogade filer med Zotero.
