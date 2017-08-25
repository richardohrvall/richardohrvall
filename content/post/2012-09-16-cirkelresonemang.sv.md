---
title: Cirkelresonemang
author: Richard Öhrvall
date: '2012-09-16'
categories:
  - Visualisering av data
slug: cirkelresonemang
---

Cirkeldiagram (eller tårtdiagram som de också kallas) är vanligt förekommande i visualiseringar av data. Tyvärr används de ofta på ett mindre lyckat sätt. Detta har gjort att de fått ett väldigt dåligt rykte, men det finns tillfällen där cirkeldiagram fungerar riktigt bra. Jag påmindes om det häromdagen när jag läste en diskussion kring cirkeldiagram som uppstod med anledning av ett [inlägg från Quora](http://www.quora.com/How-and-why-are-pie-charts-considered-evil-by-data-visualization-experts).

I likhet med linjediagrammet och stapeldiagrammet så skapades cirkeldiagrammet av [William Playfair](http://en.wikipedia.org/wiki/William_Playfair). Playfair är en centralfigur i den statistiska grafikens historia och hans tidiga verk finns bland annat kommenterade i Edward Tuftes klassiska bok [The Visual Display of Quantitative Information](http://www.edwardtufte.com/tufte/books_vdqi) (som jag har tänkt kommentera i något senare inlägg).

Cirkeldiagram kan vara utmärkta för att illustrera hur en helhet fördelar sig på ett antal delar, exempelvis hur stor marknadsandel något eller några företag på olika marknader. En nackdel med diagrammen är att det är svårt att bedöma skillnader i storlek mellan olika tårtbitar, så om det är viktigt i presentationen finns det bättre alternativ. Exempelvis har forskning visat att stapeldiagram är bättre i det avseendet Detta illustreras tydligt i följande bild från [Wikipedia](http://en.wikipedia.org/wiki/Pie_chart) där fem ungefär lika stora andelar jämförs:

![](http://upload.wikimedia.org/wikipedia/commons/thumb/b/b4/Piecharts.svg/300px-Piecharts.svg.png)

Tyvärr används cirkeldiagram ofta i 3D, vilket aldrig är lyckat. Förutom att det är fult förvrängs även intrycket, vilket gör att tårtbitarnas storlek inte motsvarar deras faktiska andel. Detta visas tydligt i en bild från [ett inlägg på den utmärkta bloggen Visual.ly](http://blog.visual.ly/2ds-company-3ds-a-crowd/).

![Angle Distortion in 3D Pie Charts](http://blog.visual.ly/wp-content/uploads/2011/12/609x321xpie_angle.png,q547b7b.pagespeed.ic.6vNQPyCFR6.png)

Ett annat vanligt fel i cirkeldiagram är att alldeles för många tårtbitar används. Helst bör ett cirkeldiagram ha högst fem tårtbitar, men upp till sju brukar kunna funkar. Mer än så blir sällan bra, även om det kan i viss mån kompenseras med ett klokt val av färger. När det gäller färger bör man hålla sig till en färg och variera dess styrka, alternativt använda en diskret färg för alla tårtbitar förutom den som man vill hålla fram. När det gäller tårtbitarnas positioner bör den största biten (andelen) börja klockan 12 i diagrammet. Övriga bitar bör sedan komma i sjunkande storleksordning. Dock är det ofta bra att placera den näst största andelen sist, dvs. så att den tårtbiten slutar klockan 12. En annan variant av cirkeldiagram som man ska undvika är de där någon eller några tårtbitar lyfts ut en aning. Om man vill framhålla någon andel bör det istället göras med hjälp av färgval.

En släkting till cirkeldiagrammet är munkdiagrammet (donut chart). De är cirkeldiagram där mitten har tagits bort. Det ger möjlighet att ge information i det hål som skapas i mitten. Nackdelen är att det blir svårare att bedöma andelarnas storlek när man inte lika lätt kan utläsa vinklar då mitten saknas. Bland annat The Economist är väldigt förtjusta i sådana diagram, som i exemplet nedan.

![The Economist's Donut Chart Showing Changing Bank Pre-Tax Profits](http://peltiertech.com/images/2012-07/20120707_woc530.png)

Jag tycker att munkdiagram fungerar ok och att svårighet att avläsa andelarnas storlek i förhållande till cirkeldiagram är något överdrivna. Snarare är det så att det är svårt i båda typer av diagram. Styrkan ligger snarare i att snabbt kunna utläsa ungefär hur helheten fördelar sig på olika andelar. Men för att vara tydlig, Economists diagram ovan är inte lyckat. Ordningen på delarna är förvirrande och etiketterna ger ett väldigt rörigt och oroligt intryck. Samtidigt finns det grader i diagramhelvetet och Fox News är som vanligt värst.

![](/img/wp/foxpie.jpg)

Så för att sammanfatta: cirkeldiagram kan vara effektiva och bra, men det finns en rad fällor. Rätt använda är de dock inte alls dumma, eller annorlunda uttryckt: ett tårtdiagram kan vara riktigt smakfullt. Bloggen Eager Eyes ger en del ytterligare matnyttiga [tips i ämnet](http://eagereyes.org/techniques/pie-charts).
