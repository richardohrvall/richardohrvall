---
title: Anscombes kvartett
author: Richard Öhrvall
date: '2012-04-04'
categories:
  - statistik
  - Visualisering av data
slug: anscombes-kvartett
---

Att grafiskt åskådliggöra sina data är inte bara en möjlighet att underlätta för läsaren att förstå och tolka en undersöknings resultat. Det är inte konstigt att många inflytelserika forskare inom samhällsvetenskaperna, som Gary King och Andrew Gelman, på senare tid lyft fram vilket fantastiskt verktyg visualisering av data kan vara i dessa sammanhang (även om genomslaget än så länge varit ganska litet, i alla fall i Sverige). Grafiken kan även vara till stor hjälp vid analys av data. Vi har mycket lättare att snabbt ta till oss ett datamaterial som illustrerats grafiskt, och framför allt har vi en förmåga att urskilja mönster i grafer som går oss förbi ifall samma data skulle presenteras i tabellform.

Grafikens möjligheter i dessa sammanhang illustreras mycket tydligt genom _Anscombes kvartett_. Det är en kvartett dataset som blev kända genom Francis J Anscombes artikel ["Graphs in Statistical Analysis"](http://www.jstor.org/stable/2682899) i _The American Statistician,_ 1973. Artikeln är mycket läsvärd och den utgör en kraftfull argumentation för användandet av grafer i analys av datamaterial (frågan är om man i dag skulle komma undan med ett sådant språk i en vetenskaplig artikel). I artikeln presenterar Anscombe fyra dataset med värden för två variabler: x och y.
<table cellpadding="0" width="512" cellspacing="0" border="0" >
<tbody >
<tr >

<td width="64" height="20" >**1 **
</td>

<td width="64" align="right" >
</td>

<td width="64" >**2 **
</td>

<td width="64" align="right" >
</td>

<td width="64" >**3 **
</td>

<td width="64" align="right" >
</td>

<td width="64" >** 4**
</td>

<td width="64" align="right" >
</td>
</tr>
<tr >

<td height="20" >**x**
</td>

<td >**y**
</td>

<td >**x**
</td>

<td >**y**
</td>

<td >**x**
</td>

<td >**y**
</td>

<td >**x**
</td>

<td >**y**
</td>
</tr>
<tr >

<td align="right" height="20" >10
</td>

<td align="right" >8,04
</td>

<td align="right" >10
</td>

<td align="right" >9,14
</td>

<td align="right" >10
</td>

<td align="right" >7,46
</td>

<td align="right" >8
</td>

<td align="right" >6,58
</td>
</tr>
<tr >

<td align="right" height="20" >8
</td>

<td align="right" >6,95
</td>

<td align="right" >8
</td>

<td align="right" >8,14
</td>

<td align="right" >8
</td>

<td align="right" >6,77
</td>

<td align="right" >8
</td>

<td align="right" >5,76
</td>
</tr>
<tr >

<td align="right" height="20" >13
</td>

<td align="right" >7,58
</td>

<td align="right" >13
</td>

<td align="right" >8,74
</td>

<td align="right" >13
</td>

<td align="right" >12,74
</td>

<td align="right" >8
</td>

<td align="right" >7,71
</td>
</tr>
<tr >

<td align="right" height="20" >9
</td>

<td align="right" >8,81
</td>

<td align="right" >9
</td>

<td align="right" >8,77
</td>

<td align="right" >9
</td>

<td align="right" >7,11
</td>

<td align="right" >8
</td>

<td align="right" >8,84
</td>
</tr>
<tr >

<td align="right" height="20" >11
</td>

<td align="right" >8,33
</td>

<td align="right" >11
</td>

<td align="right" >9,26
</td>

<td align="right" >11
</td>

<td align="right" >7,81
</td>

<td align="right" >8
</td>

<td align="right" >8,47
</td>
</tr>
<tr >

<td align="right" height="20" >14
</td>

<td align="right" >9,96
</td>

<td align="right" >14
</td>

<td align="right" >8,1
</td>

<td align="right" >14
</td>

<td align="right" >8,84
</td>

<td align="right" >8
</td>

<td align="right" >7,04
</td>
</tr>
<tr >

<td align="right" height="20" >6
</td>

<td align="right" >7,24
</td>

<td align="right" >6
</td>

<td align="right" >6,13
</td>

<td align="right" >6
</td>

<td align="right" >6,08
</td>

<td align="right" >8
</td>

<td align="right" >5,25
</td>
</tr>
<tr >

<td align="right" height="20" >4
</td>

<td align="right" >4,26
</td>

<td align="right" >4
</td>

<td align="right" >3,1
</td>

<td align="right" >4
</td>

<td align="right" >5,39
</td>

<td align="right" >19
</td>

<td align="right" >12,5
</td>
</tr>
<tr >

<td align="right" height="20" >12
</td>

<td align="right" >10,84
</td>

<td align="right" >12
</td>

<td align="right" >9,13
</td>

<td align="right" >12
</td>

<td align="right" >8,15
</td>

<td align="right" >8
</td>

<td align="right" >5,56
</td>
</tr>
<tr >

<td align="right" height="20" >7
</td>

<td align="right" >4,82
</td>

<td align="right" >7
</td>

<td align="right" >7,26
</td>

<td align="right" >7
</td>

<td align="right" >6,42
</td>

<td align="right" >8
</td>

<td align="right" >7,91
</td>
</tr>
<tr >

<td align="right" height="20" >5
</td>

<td align="right" >5,68
</td>

<td align="right" >5
</td>

<td align="right" >4,74
</td>

<td align="right" >5
</td>

<td align="right" >5,73
</td>

<td align="right" >8
</td>

<td align="right" >6,89
</td>
</tr>
</tbody>
</table>
Som ni ser av tabellen har x samma värden i dataset 1 till 3, medan y varierar mellan samtliga dataset. Även i så här små dataset är det svårt att urskilja tydliga mönster och då man analyserar datamaterial med tusentals observationer eller fler, ja, då blir det en omöjlighet. Vanligtvis tar man därför fram ett antal mått för de variabler man är intresserad av, såsom medelvärden och mått på variation. Om vi ser till dataset 1 kan vi exempelvis ta fram följande värden:

Antal observationer (n)=11

Medelvärde för x=9

Medelvärde för y=7,5

Standardavvikelse för x=3,32

Standardavvikelse för y=2,03

Och en enkel regressionsmodell (OLS) ger y=3+0,5x med ett p-värde för koefficienten för x på 0,03 och ett R2 som uppgår till 0,67.

Det intressanta är att exakt samma värden även gäller för dataset 2, 3 och 4. Så om vi bara använder dessa standardmått kan vi lätt frestas att dra slutsatsen att sambandet mellan x och y ser ut på samma sätt i de fyra datamaterialen. Stämmer då inte det? Nej, om vi grafiskt illustrerar sambandet mellan x och y i dataseten med hjälp av punktdiagram och en regressionlinje ser vi att det är stora skillnader mellan dem.

![](/img/wp/anscombe.png)

I dataset 1 verkar sambandet mellan x och y vara linjärt och regressionsmodellen förefaller därmed vara lämplig. Punkterna ligger jämnt spridda kring regressionslinjen. Som framgår av graf 2 är den linjära regressionsmodellen däremot inte lämplig för dataset 2. Där verkar istället sambandet mellan x och y vara kurvlinjärt och en modell med en andragradspolynom hade antagligen varit mer lämplig. I dataset 3 verkar visserligen sambandet mellan x och y vara linjärt, men en observation verkar vara en så kallad uteliggare (outlier) och den observationen gör att regressionslinjen blir brantare än den annars skulle vara. Här bör den observationen kontrolleras för att se att det inte är något fel i datamaterialet. Även om datapunkten visar sig vara korrekt kan det finnas anledning att fundera på att utesluta den från modellen (det beror på sammanhanget) eller berätta om dess effekt i presentationen av analysen. I dataset 4 beror sambandet på endast en datapunkt. Om den utesluts finns inte längre något linjärt samband. Även här finns det anledning att studera datamaterialet närmare för att se om ett linjärt samband verkligen finns.

Även om dessa dataset är illustrerar extremfall är det inte ovanligt att motsvarande situationer kan uppstå, om än vanligtvis i lindrigare former. Så slutsatsen är glasklar: visualisera dina data!
