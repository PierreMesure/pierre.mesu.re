---
title: Din Riksdag
subtitle: Ett projekt för att göra den svenska lagstiftningsprocessen mer deltagande och transparent
excerpt: En plattform för att följa lagarnas tillkomst och delta i processen
date: 2018-05-01
tags:
  - Open Parliament
  - Citizen participation
  - Transparency
---

{{< button href="https://github.com/DinRiksdag/dinriksdag" target="_blank" >}}
{{< icon "github" >}} Källkod (plattform)
{{< /button >}}
{{< button href="https://github.com/DinRiksdag/decidim-module-riksdagen" target="_blank" >}}
{{< icon "github" >}} Källkod (skrapningsmodul)
{{< /button >}}
{{< button href="https://github.com/PierreMesure/pierre.mesu.re/tree/master/static/dinriksdag/presentations" target="_blank" >}}
{{< icon "link" >}} Presentationer
{{< /button >}}

## Insikten om att den svenska demokratin inte är perfekt

Jag kom till Sverige 2016 och så länge jag kan minnas har jag varit fascinerad av landets demokrati. Under mina första år i Stockholm besökte jag ofta riksdagen, satt på läktaren ovanför kammaren och lyssnade på debatterna. Den svenska parlamentariska demokratin hade något jag inte vuxit upp med: proportionellt valsystem, hög nivå av tillit, mindre polarisering och mycket konsensus och respekt för institutioner och processer.

I mitt hemland var misstron och ilskan på rekordnivåer. Men på grund av det bubblade Frankrike också av en enorm drivkraft att hålla politiker under uppsikt och ansvariga, och många medborgare hade en stark vilja att engagera sig i de beslut som påverkade dem. För att möta denna efterfrågan startades otaliga innovativa projekt under 2010-talet, och institutionerna reformerades (lite grann) för att låta dessa nya former av demokrati få genomslag.

När jag kom hit betraktade jag Sverige som demokratins högborg och var säker på att inget av detta var nytt här. Jag hade fel. Kanske på grund av denna höga tillit är information om förtroendevaldas privata intressen inte tillgänglig som öppna data. Tills nyligen var man tvungen att begära ut och hämta den fysiskt mot en rejäl avgift. Sverige är den enda demokratin runt Östersjön som inte ger medborgare möjlighet att skriva namninsamlingar för att starta debatter i sitt parlament. Den officiella processen för att ge feedback på framtida lagstiftning (remissprocessen) är skräddarsydd för särintressen och det organiserade civilsamhället men lämnar mycket litet utrymme för gräsrotsengagemang och saknar i hög grad transparens.

## Bygga Din Riksdag, en workshop i taget

Naivt, men med en genuin vilja att förbättra saker, startade jag ett projekt som hette **Din Riksdag**. Din Riksdags mål var att bli en plattform där medborgare och gräsrotsgrupper kunde få en bättre förståelse för lagstiftningsprocessen och ha inflytande över den.

Jag insåg snabbt hur litet intresset var från institutioner och politiska krafter att reformera det nuvarande systemet, så jag bestämde mig för att bygga något som skulle "hacka" det snarare än att vänta på förändring inifrån. Jag skissade på två potentiella mekanismer:

- ***medborgarremissvar*** som skickas till regeringen innan de börjar utforma propositionen.
- ***medborgarmotioner*** som skickas när propositionen diskuteras i riksdagen.

Båda kunde utformas gemensamt och samla stöd genom röster, vilket skulle ge ökad legitimitet åt populära förslag och göra det enkelt för både Regeringskansliet och riksdagens utskott att inkludera dem i lagstiftningsarbetet när de skapar propositionen respektive betänkandet.

Dessa idéer kom från personlig forskning men också genom feedback och idéer från olika workshops jag genomförde under 2017 och 2018.

## Svensk civic tech?

För att stödja denna nya process satte jag också upp en digital plattform där hela lagstiftningsprocessen replikerades och var interaktiv – en webbplats där medborgare kunde bläddra igenom utredningar, remisser, propositioner och riksdagsaktivitet, samt skicka in eller stödja medborgarremissvar och motioner. Jag använde tidens ledande civic tech-verktyg: först Consul, sedan Decidim, och utvecklade moduler för att integrera svensk lagstiftningsdata.

Tyvärr, trots riksdagsförvaltningens öppna API:er, är mycket av den datan fortfarande inte tillgänglig i ett strukturerat format. Det är därför jag startade projekt som [OpenRemiss](../openremiss) och slutligen [g0v.se](../g0vse) för att göra det enklare att återanvända data från regeringen.se.

## Att vända blad

Även om jag aldrig officiellt avslutade Din Riksdag, slutade jag investera min tid i det runt mitten av 2018. Vid den tiden träffade jag grundarna av Digidem Lab (Sanna, Anna och Petter) och bestämde mig för att gå samman med dem för att tillämpa mina nyförvärvade färdigheter i andra deltagandeprojekt i Sverige. Tillsammans använde vi Decidim i många kommuner här och utomlands och introducerade metoder som medborgarbudget och medborgaråd.

Min förhoppning var att om jag gav de nationella institutionerna några år skulle de mogna och bli mer intresserade av att låta medborgarna komma till tals. Som jag sa tidigare var jag väldigt naiv.
