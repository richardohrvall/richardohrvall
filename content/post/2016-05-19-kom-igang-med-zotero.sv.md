---
title: Kom igång med Zotero
author: Richard Öhrvall
date: '2016-05-19'
categories:
  - workflow
  - Zotero
slug: kom-igang-med-zotero
---

I ett [tidigare blogginlägg](https://richardohrvall.rbind.io/2016/04/val-av-referenshanteringssystem-zotero/) beskrev jag kortfattat hur jag kom fram till att välja Zotero som mitt referenshanteringssystem. Det är ett program som framför allt hjälper till att hålla koll på referenser,  men även olika elektroniska dokument. Detta är ovärderligt om man skriver en vetenskaplig artikel, en akademisk eller populärvetenskaplig bok eller något liknande.

Det finns redan ett antal guider till Zotero, se till exempel programmets [webbsida](https://www.zotero.org/), googla eller sök på YouTube. Här tänker jag bara kortfattat redogöra för hur programmet fungerar. I några uppföljande bloggposter kommer jag att ge några tips kring hur man kan lagra filer och kombinera Zotero med andra program, vilket inte är alldeles enkelt att hitta information kring. Förhoppningsvis är det till nytta för någon.

Zotero laddas ned från programmets [webbsida](https://www.zotero.org/download/). Det finns två varianter att välja mellan: som tillägg i Firefox eller som separat program. Det förstnämnda är den ursprungliga varianten. Om du väljer den måste du även installera ett tillägg för Word (eller LibreOffice om du använder det). Väljer du det separata programmet följer kopplingen till Word (eller LibreOffice) med. Däremot måste du installera ett tillägg i den webbläsare du använder.

Då referenserna i Zotero synkroniseras kan man installera båda varianter, vilket jag har gjort. Men då jag framför allt använder Google Chrome som webbläsare är det Zotero som separat program i kombination med tillägg i Google Chrome (Zotero Connector hittar du [här](https://chrome.google.com/webstore/search/zotero%20connector?hl=sv)) som är den lösning som jag använder. De två varianterna ser i stort sett likadana ut och har samma funktionalitet, så det handlar främst om vilken webbläsare du vill använda (det finns dock inget stöd för Microsoft Edge, men vem använder den webbläsaren?).

När Zotero startas ser det ut så här:

![Skärmklipp](/img/wp/Skärmklipp.png)

Referenserna syns i mittenspalten och markerar man en referens ser man mer information om den i högerspalten. Klickar man på pilen intill en referens ser man olika filer kopplade till den, t.ex. anteckningar eller referensen i elektroniskt format. Om man exempelvis har en artikel sparad i pdf-format kan man klicka på den för att få upp den i den pdf-läsare som man använder. I vänsterspalten kan man skapa mappar (kallas samlingar i Zotero) och dra referenser dit för att samla dem.  Det går även att koppla etiketter till referenser och sortera efter det, eller söka efter referenser i sökrutan. Sökningar kan även innefatta innehållet i filer.

Om man redan har ett antal dokument i pdf-format kan man importera dem in i Zotero via Arkiv i menyn. Därefter  kan man markera referensen, högerklicka och välja 'Läs metadata för PDF' för att hitta information kring referensen. Zotero försöker då hitta information mot Google Scholar. Om man försöker hitta metadata för ett stort antal pdf:er kan det bli för många anrop mot Google Scholar så att det säger ifrån. Då får man vänta ett antal timmar och sedan fortsätta.

Under Verktyg\inställningar finns en del möjligheter att anpassa Zotero. I fliken Synkronisera anger du ditt användarnamn och lösenord för Zotero. Om du inte har något konto, klickar du på länken för att skapa ett konto hos Zotero. Det är gratis. Genom att ha ett konto kan Zotero synkronisera mellan olika datorer, och du kan även komma åt dina referenser via Zoteros webbsida. På samma flik kan du även ange om du vill att Zotero ska synkronisera dina pdf:er. Det är gratis upp till 300 MB. Det går att uppgradera för en rimlig kostnad om man vill ha mer utrymme.

Under Inställningar och fliken Avancerat\Filer och kataloger kan man ställa in att Zotero ska ha relativa länkar. Det är att föredra om man vill ha Zotero på olika datorer. Du väljer där en Baskatolog under vilken du har samma mappstruktur på alla datorer, t.ex. den mapp där du har dina Zotero-filer på datorn. Var Zotero ska lagra sina filer anger du under Lagringsplats. Där hamnar databasfilen med dina referenser, men även alla pdf:er du importerar i Zotero och en del annat. Om man använder Dropbox (eller någon annan tjänst för lagring av data i molnet) kan man få för sig att lägga mappen med Zotero-filer i sin Dropbox-mapp och synkronisera pdf:er på så vis snarare än via Zoteros webbplats (och därmed undvika att betala för två molntjänster). Det är inte att rekommendera! Detta då det finns risk att dessa två synkroniseringar hamnar i konflikt med varandra och din databasfil med alla referenser förstörs. Det finns dock bättre lösningar, bland annat med hjälp av tillägget Zotfile, vilket jag återkommer till i en senare bloggpost.

Det är när man ska lägga till nya referenser som Zotero visar hur kraftfullt det är. Om du har Zotero igång visas i webbläsaren en ikon som anpassas beroende på vilken webbsida du är inne på. Om du t.ex. är inne på en sida (såsom Jstor) där en vetenskaplig artikel presenteras ändras ikonen till ett dokument, se bilden nedan.

![Skärmklipp](/img/wp/Skärmklipp-1.png)

Du kan då klicka på ikonen för att ladda ned referensen i Zotero, inklusive pdf-filen. På motsvarande sätt går det att hämta referenser när du är inne på Amazon, Libris, osv. Är du på en webbsida där många olika verk presenteras kan du välja att ladda ned alla referenser på en och samma gång. De fullständiga referenserna finns sedan i Zotero. Otroligt smidigt! En liten nackdel är visserligen att om man laddar ned pfd-filer på det sättet lagrar Zotero dem i mappar med ytterst märkliga namn (ungefär som Itunes gör). Det är inget problem att hitta artiklarna via Zotero, men lite krångligt att hitta dem via utforskaren. Det går dock att ändra med hjälp av tillägget Zotfile, vilket jag får anledning att återkomma till i en senare bloggpost.

När du sedan öppnar Word har du en särskild flik för Zotero. Om du vill lägga in en referens i ditt dokument klickar du på "Add/Edit Citation" och sedan behöver du bara börja skriva författarnamnet och välja ur den lista som Zotero föreslår. När du lägger in första referensen i dokumentet får du även välja referenssystem. De flesta vanliga system finns inlagda, men det går även att ladda ned för en lång rad ytterligare tidskrifter. Det går självfallet att byta referenssystem om man senare ändrar sig. Från samma flik kan du även välja att lägga in en referensförteckning.

![Skärmklipp](/img/wp/Skärmklipp-2.png)

Om man använder LaTeX istället för Word kan man exportera referenserna till BibTeX. En lösning att kolla på är [Better BibTeX](https://github.com/retorquere/zotero-better-bibtex).

I nästa bloggpost ska jag försöka beskriva hur man kan kombinera Zotero med Dropbox och samtidigt lagra filer på ett bättre sätt och få en bra integration med läsplattor - allt med hjälp av tillägget Zotfile.
