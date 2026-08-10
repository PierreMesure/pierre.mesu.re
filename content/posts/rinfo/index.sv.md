---
title: Lagar är en del av Sveriges infrastruktur
excerpt: Sverige har i över 25 år haft regler om ett offentligt rättsinformationssystem. Ändå publiceras vår rättsinformation fortfarande splittrad, svåråtkomlig och i format som inte lätt kan återanvändas.
date: 2026-08-07
tags:
  - Öppna data
  - Rättsinformation
  - Digitalisering
---

*Nul n’est censé ignorer la loi. Ignorantia juris non excusat* Ingen förväntas vara okunnig om lagen.

Det är en hård princip, men den bygger på en rimlig förutsättning: den som vill följa lagen måste också ha möjlighet att ta reda på vad den säger. [Högsta domstolen har uttryckt det tydligt](https://www.domstol.se/globalassets/filer/domstol/hogstadomstolen/avgoranden/2019/b-6130-18.pdf): om människor förutsätts känna till vad som är straffbart måste de också kunna ta del av regleringen.

![Svensk författningssamling i tryckt format på Riksdagsbiblioteket](thumbnail.jpeg "Svensk författningssamling i tryckt format på Riksdagsbiblioteket (CC-BY 4.0 Pierre Mesure)")

I dag betyder tillgång till lagen inte längre tillgång till en tryckt lagbok. Nästan all åtkomst är digital. Dessutom är det allt oftare inte en människa som först läser rättsinformationen, utan ett informationssystem, en algoritm eller en AI-agent.

Maskiner läser inte lagar som människor gör. De behöver beständiga identifierare, strukturerad text, tydliga versioner, metadata och länkar mellan dokument. Men den svenska staten publicerar fortfarande stora delar av vår rättsinformation som om det huvudsakliga behovet vore att öppna en PDF-fil i en webbläsare.

## Maskiner tillämpade regler långt före ChatGPT

Diskussionen om AI kan ge intrycket att maskiners användning av lagstiftning är något nytt. Det är det inte. Svenska myndigheter har byggt system (webbsidor, Excel-ark, algoritmer) som bygger på vårt regelverk ända sedan de har haft tillgång till datorer. Förvaltningslagen tillåter uttryckligen beslut som fattas automatiserat, och [Digg har omfattande vägledning](https://www.digg.se/kunskap-och-stod/automatisera-handlaggning-och-beslut/automatiserade-beslut) för myndigheter som vill automatisera handläggning och beslut. Och det finns såklart många användare av lagen i privatsektorn också.

Frågan är därför inte om maskiner ska använda våra regelverk. Det gör de redan. Frågan är om de ska kunna bygga på tillförlitlig, aktuell och officiell rättsinformation – eller på den kopia som råkar ha skrapats, tolkats och städats bäst av någon utomstående.

Behovet syns överallt. Jag får nästan varje vecka frågor från myndighetskollegor, doktorander, journalister och privatpersoner som försöker återanvända rättsinformation. Någon behöver följa ett ärende genom lagstiftningsprocessen. En annan vill samla forskningsmaterial, granska hur en regel har förändrats över tid eller skapa en tjänst som hjälper människor att förstå sina rättigheter.

De frågar ofta om samma sak: Var finns informationen? Finns det ett API? Går dokumenten att ladda ner samlat? Hur hänger en utredning, en proposition, en lag och senare ändringar ihop?

I andra länder har man gått betydligt längre. Det franska projektet [OpenFisca](https://openfisca.org/) gör stora delar av skatte- och bidragssystemet till körbar, öppen kod. Projektet visar vad som blir möjligt när regler behandlas som gemensam digital infrastruktur (*rules as code*) i stället för som dokument som varje aktör måste tolka på nytt.

![Skärmdump av franska regeringens webbsida "1 jeune 1 solution"](openfisca.png "Tack vare regler som kod lovar denna webbsida att visa om man uppfyller kriterierna för 1000 bidrag på 5 minuter, och att kunna söka vissa automatiskt ([länk](https://mes-aides.1jeune1solution.beta.gouv.fr)).")

Ett annat sätt att jämföra oss internationellt är att se på EU-samarbetet [European Legislation Identifier, ELI](https://eur-lex.europa.eu/eli-register/what_is_eli.html) Sverige anslöt sig äntligen 2024 men vi har fortfarande inte börjat publicerar data eftersom vi saknar datainfrastrukturen för det. Danmark, [Finland](https://eur-lex.europa.eu/eli-register/finland.html) och [Norge](https://eur-lex.europa.eu/eli-register/norway.html) använder redan ELI för att ge rättsinformation beständiga identifierare och strukturerade metadata.

![Länder som implementerar ELI, Sverige är ett av få EU-länder som inte gör det](eli.png "Källa: [EUR-lex](https://eur-lex.europa.eu/eli-register/implementing_countries.html)")

## Ett rättsinformationssystem som mest består av länkar

Sverige har inget fungerande offentligt rättsinformationssystem värdigt namnet. Vi har en förordning som säger att ett sådant system ska finnas, ett hundratal aktörer som ansvarar för olika fragment och en central webbplats som huvudsakligen länkar vidare till dem.

[Rättsinformationsförordningen](https://rkrattsbaser.gov.se/sfst?bet=1999:175) antogs 1999. Det var för sin tid en ambitiös text som skulle ha gjort Sverige till ett föregångarland med bra förutsättningar för att producera och tillgängliggöra digital rättsinformation. Men det blev [lagrummet.se](https://www.lagrummet.se), en samling av länkar och ett kollektivt misslyckande. 27 år senare innehåller webbplatsen fortfarande inte själva rättsinformationen och erbjuder inget gemensamt API.

I sin egen [redovisning av rättsinformationssystemet](https://www.domstol.se/globalassets/filer/gemensamt-innehall/rapporter/redovisning_en-saker-och-effektiv-tillgang-till-rattsinformation.pdf) från 2025 skriver Domstolsverket att dagens lösning "inte i något avseende" lever upp till de behov som myndigheten har identifierat. Rapporten konstaterar också att rättskällorna publiceras på många olika sätt, utan gemensamma metadata och ibland utan ens maskinläsbar uppmärkning av rubriker och ingresser.

Detta misslyckande kostar oss dyrt, sannolikt hundratals miljoner kronor. Men det försämrar också vår gemensamma demokrati, tilliten i vår offentlig förvaltning och det hindrar innovation och transparens.

Regeringskansliet producerar en stor del av den information som resten av systemet behöver: den svensk författningssamlingen, utredningar, departementspromemorior, propositioner, remisser och mycket annat som tusentals personer laddar ner och läser varje dag. Trots det, och trots att myndigheten själv har stora problem med att återanvända sin egen data... trots det finns inte början av ett sammanhållet öppet API till materialet.

Riksdagen har i omkring femton år publicerat omfattande öppna data, mycket tack vare ett antal eldsjälar. Där kan man även hitta propositioner, skrivelser och utredningar som ursprungligen kommer från regeringen. Deras arbete förtjänar beröm, men det är ett orimligt ansvar de har fått utan tydligt mandat, och det blir aldrig möjligt att uppnå tillfredställande datakvalitet när Riksdagsförvaltningen måste bearbeta gammaldags dokument som aldrig förväntas tillgängliggöras på ett annat sätt än som PDF-filer på regeringen.se

## Det lovande Rinfo-projektet som aldrig kom i mål

Det saknas inte kunskap om hur problemet kan lösas. Omkring 2010 drev Domstolsverket Rinfo-projektet för att skapa ett modernt rättsinformationssystem. Projektet tog fram gemensamma URI:er, en dokumentmodell och RDF-baserade metadata. Myndigheten rekryterade till och med Staffan Malmgren, som skapade [lagen.nu](https://lagen.nu) och länge varit en av Sveriges mest kunniga personer inom digital rättsinformation.

![En slide från Rinfo-projektet med skärmdumpar från myndigheters föreskriftssidor](rinfo_slide.png "Källa: [Domstolsverket](https://www.slideshare.net/slideshow/rttsinformationssystemet/5903008)")

Men projektet blev som mest en fin prototyp och beslutet saknades för att implementera det brett.

Domstolsverket konstaterar nu självt att Lagrummet ligger vid sidan av myndighetens kärnverksamhet. När varje organisation ansvarar för sitt dokument men ingen har verklig makt, finansiering och ansvar för helheten blir resultatet det vi ser i dag: ett system på papper och en länksamling i verkligheten.

## En osynlig men stor samhällsekonomisk kostnad

När rättsinformation inte publiceras strukturerat försvinner inte behovet. Arbetet flyttas bara nedströms. Och innovativa projekt uteblir.

Myndigheter bygger egna integrationer. Forskare ger tråkiga arbetsuppgifter till masterstudenter som ägnar månader åt att samla och rensa dokument innan analyser kan börja. Journalister får svårare att systematiskt följa lagstiftning och granska makten. Företag och ideella projekt skriver *scrapers* som går sönder varje gång en myndighet ändrar sin webbplats. Samma dokument laddas ner, konverteras, OCR-tolkas och klassificeras om och om igen.

Varje sådan bearbetning skapar dessutom avstånd till den officiella källan. En PDF kan ha ersatts utan tydlig versionshistorik. Metadata kan ha tolkats fel. Relationer mellan dokument kan saknas. Uppdateringar kan komma för sent. Ändå använder vi det vi har även om det leder till misstag.

Privata rättsdatabaser fyller en viktig funktion, men de ska inte behöva ersätta en offentlig grundinfrastruktur. När staten publicerar undermåliga råvaror och sedan köper tillbaka tillgång till förädlade versioner av sin egen information är det inte effektiv digitalisering. Det är att privatisera kostnaden för att förstå offentlig information och därefter skicka räkningen tillbaka till samhället.

## AI hjälper, men löser inte ansvarsflykten

Det finns ändå skäl att vara hoppfull. AI gör det mycket enklare att bygga och underhålla verktyg som hämtar, klassificerar och extraherar information ur dokument. Det går snabbare att skriva skrapor, tolka gamla format och upptäcka samband mellan rättskällor.

Men AI får inte bli ännu en ursäkt för att låta grundproblemet vara kvar. En språkmodell som försöker återskapa metadata ur en PDF är inte ett rättsinformationssystem. En sannolik tolkning är inte en officiell källa. Ju fler aktörer som måste reparera informationen efter publiceringen, desto fler möjligheter finns för fel och motstridiga versioner.

Arbetet måste göras där informationen produceras. Dokument ska från början få beständiga identifierare, strukturerad text, versionshistorik, tydliga metadata och maskinläsbara relationer. Det är först då AI och andra digitala verktyg kan användas på ett säkert, effektivt och granskningsbart sätt.

## Lagdata, ett litet steg i rätt riktning

Jag har inte byggt Lagdata för att själv lösa de problemen jag skriver om ovan. Snarare är detta ett sätt att hjälpa dem som idag vill återanvända rättsinformation trots att vi inte har rätt infrastruktur på plats. Det är en kollaborativ kartläggning av olika typer av rättsinformation och hur den i dag kan nås maskinellt.

Projektet dokumenterar var den finns, i vilka format den publiceras, vilka API:er och nedladdningar som går att använda och vilka oberoende projekt som kan konvertera och strukturera den. Målet är att myndigheter, forskare, journalister och utvecklare inte ska behöva börja från noll varje gång.

Dokumentationen är öppen och ofullständig. Jag har arbetat med vissa delar av rättsinformationen i många år men saknar erfarenhet av andra. Därför hoppas jag att fler som har slagits med samma PDF-filer, webbplatser och datastrukturer vill bidra med det de har lärt sig.

På kort sikt kan Lagdata sänka tröskeln för att använda den rättsinformation som faktiskt finns. På längre sikt hoppas jag fortfarande att staten (och i synnerhet Regeringskansliet) tar sitt ansvar för att lagar och andra rättskällor publiceras som den kritiska digitala infrastruktur som de redan utgör.

Den dag det fungerar har Lagdata blivit överflödigt och jag väldigt glad.
