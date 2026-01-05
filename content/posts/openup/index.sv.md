---
title: "Skapa innovation med öppna data i offentlig upphandling i Sverige"
date: 2019-09-03
author: Pierre Mesure
tags:
  - procurement
  - open-contracting
categories:
  - Open Up!
# layout options: single, single-sidebar
layout: single
---

I Sverige spenderade den offentliga sektorn 683 miljarder kronor i 2017 med bara offentlig upphandling[^fn:1]. Över 18000 upphandlingar startas varje år av offentliga institutioner.
{.dropcap}

![Bugs Bunny counting dollar bills](bugsbunny.gif)

Offentlig upphandling är en viktig del av en fungerande offentlig sektor. En rättvis och effektiv process har positiva konsekvenser över hela samhället. Den sparar resurser som behövs i välfärden och minskar utrymmet för korruption.

Upphandling utmanas också mycket av de stora förändringarna som har pågått i minst 40 år i den offentliga: nya behov, samhällets digitalisering, innovationsupphandling, privatiseringar m.m.

---

I denna artikel kommer vi att titta på offentlig upphandling i Sverige, lista vissa problem den står inför och jämföra med andra länder med fokus på öppenhet. Till slut kommer vi introducera ett projekt som vi startar på Civic Tech Sverige för att försöka lösa dessa problem och öka medvetenhet bland de relevanta institutionerna. Redo?

## Data överallt!

![The procurement lifecycle, visualisation from the Swedish procurement agency](upphandlingskedjan.webp "Bild från Upphandlingsmyndigheten")

Vi startar med något uppenbart: **offentlig upphandling är en data-intensiv process**. Från annonser till signerade avtal och fakturor, hela kedjan dokumenteras försiktigt, oftast digitalt.

Nästan all data är PSI (public sector information) och kan begäras ut med offentlighetsprincipen från myndigheten som äger den. För att göra processen smidigare kräver lagen i bland att informationen publiceras proaktivt. Det är väldigt viktigt för alla involverade parter:

* **journalister**, som begär ut dokument enligt offentlighetsprincipen regelbundet, behöver data för att utforska fel och korruption, vilket leder till en mer hälsomsam offentlig sektor;
* **privata bolag** behöver hålla sig informerade om anbud på ett enkelt och lämpligt sätt om de ska kunna skicka ett erbjudande. Att kunna kolla tidigare anbud hjälper dem att erbjuda den mest passande leveransen för det optimala priset;
* **offentliga myndigheter** behöver så många företag som möjligt som svarar till sina annonser för rättvis konkurrens, vilket leder till lägre priser och bättre service. De behöver även mäta hur bra de gör med sin inköp. Ett bra sätt att göra så är att jämföra sig t.ex. med en kommun av liknande natur och storlek;
* **medborgare** nyttar av allt detta eftersom de får bättre offentliga tjänster till en mindre kostnad.

## Situationen i 🇸🇪 idag

I Sverige har man kontinuerligt tryckt för att digitalisera hela processen. Senast blev det obligatoriskt för institutioner att acceptera e-fakturor[^fn:2] (med europeiska standard PEPPOL BIS Billing 3[^fn:3]). Förutom några undantag är det digitala normen på hela kedjan, och **Sverige är kanske ett av de mest avancerade länderna i just det här**.

Man hoppas då att dessa data används så mycket som möjligt av de ovannämnda aktörerna och att de hjälper att matcha efterfrågan och erbjudande på ett optimalt sätt. Jo, det tänkte vi också i början men vi förstod snabbt hur fel vi hade, och det är så vårt projekt föddes.

Just nu ser situationen ut så här:

* **journalister** måste skicka offentlighetsprincipsbegäran för att få tillgång till dokumenten de behöver. Det är en krånglig process, man får sällan dokumenten i standardiserad format och det kostar mycket tid för båda parter. I bästa fall får man ett svar på e-post med PDF:er, Excelarker om man har tur. Ibland är det bara mycket papper och kom ihåg att offentlighetsprincipen tillåter institutioner att ta 2kr per sida utan att rättfärdiga kostnaden…
* **privata bolag** måste betala för en privat tjänst för att bevaka och få notiser om anbud som de är intresserade av. Marknaden för dessa tjänster (Upphandlingsmyndigheten har en lista) är liten, nästan ett monopol på grund av datainlåsning av de som erbjuder upphandlingsmjukvaran som används i den offentliga sektorn. OPIC, det största av dem, har en dominant position och bygger på den genom att cirkulera datan mellan sina egna tjänster och köpa sina konkurrenter. Det är väldigt svårt att mäta hur mycket **denna kostnad avskräcker små och medelstora företag, hur mycket den gör att de inte ens ser den offentliga som en potentiell kund**, men det är omöjligt att förneka att det förmodligen minskar konkurrens.
* **offentliga institutioner** får väldigt lite insyn om sitt inköpsbeteende, mycket mindre än vad de borde ha i ett modernt land som Sverige. En del måste köpas till de som säljer dem upphandlingstjänsterna (och OPICs ägare utnyttjar där också sin dominant position för att erbjuda bättre statistik). Men oftast måste kommuner och myndigheter göra tidskrävande revisioner och de mindre kommunerna har inga resurser för något.

Allt detta för att säga att, även om Sverige har kanske en av de effektivaste och minst korrumperade systemen i världen är **förbättringspotentialen enorm!**

## Men gör man annorlunda utanför Sverige?

Spoiler: ja, det gör man.

I utvecklade länder brukar man veta att en gratis offentlig annonsdatabas är en viktig del av ett rättvist och effektivt upphandlingsekosystem. I norden har dessa tjänster söta namn som [udbud.dk](https://udbud.dk) i Danmark, [doffin.no](https://doffin.no) i Norge, [hilma.fi](https://www.hankintailmoitukset.fi/sv/) i Finland. Enligt forskning av EU-projekt Digiwhist och Open Knowledge Tyskland[^fn:4] från 2017 hade nästan alla europeiska länder en sådan (31 av 34). En snabb uppdatering 2019 visar oss att Sverige är faktiskt ensam nu när Österrike och Luxemburg har skapat sina egna annonsdatabaser. Sverige är alltså ensam i EU som inte har en offentlig annonsdatabas. Det bör uppmärksammas mer.

Det är bara logiskt. Ju mer man begränsar tillgång till information om anbud, desto mindre konkurrens man får. En betalvägg är kanske det effektivaste sättet att avskräcka företag som vill möta offentliga behov.

---

Många länder och kommuner har också börjat att publicera öppna data för andra steg i processen, för att öka transparens men också effektivitet.

Det mest berömda exemplet är Ukraina, där plattformen **ProZorro** skapades av Transparency International för att bevaka och effektivisera offentlig upphandling. Det blev en stor succé[^fn:5].

![Screenshot of Prozorro's BI visualisations](prozorro-thumbnail.png "ProZorro har en kraftig Business Intelligence modul som aktivister kan använda för att bevaka processen, men också ge insyn till regeringen om sin upphandling (bi.prozorro.org)")

Kanske närmare Sverige finns det Kanada[^fn:6], Storbritannien[^fn:7] och Frankrike[^fn:8], som började publicera så mycket data som möjligt tidigt på 2010-talet.

Finland är bästa exemplet i norden och publicerar statistik för alla sina myndigheter som öppna data och på en interaktiv plattform, [granskaupphandlingar.fi](https://granskaupphandlingar.fi). Tidigare i år bestämde de också att lägga till information från kommuner och regioner.

## Att kämpa mot status quo

Varför ligger Sverige så mycket efter?

Svårt att säga men situationen lär inte förbättras. Nyligen gav regeringen uppdraget till Upphandlingsmyndigheten att samla statistikdata om upphandlingsprocessen och inte ens en gång nämnde man att det vore möjligt att öppna rådata först, även när deras rapport hyllade Finland som ett exempel att följa[^fn:9]...

När vi frågade en av myndighetens chefer om det i somras fick vi för svar:

> Vi har offentlighetsprincipen och det är väldigt få länder i världen som har den. Vi borde ju nöja oss med den.

~~Incompetence~~ Ignorance is bliss.

---

I ett land som ofta är övertygat av sitt överlägsenhet är idéen att Sveriges offentlighetsprincip skulle vara unik eller åtminstone bättre ganska vanlig. Sanningen är att de flesta demokratierna har en offentlighetsprincip och allt fler har moderniserat sin lagstiftning för att anpassa sig efter digitalisering och njuta av öppna data, vilket Sverige inte har gjort.

Det förklarar varför vi fick negativa svar när vi frågade Upphandlingsmyndigheten, Konkurrensverket, DIGG, SKL och dess inköpsbolag Kommentus om de hade en kontaktperson som jobbade på att öppna inköpsdata…

När vi kollade på vilka lokala administrationer hade börjat att publicera sina fakturor hittade vi bara tre kommuner ([Göteborg](https://catalog.goteborg.se/catalog/6/datasets/75), [Örebro](https://www.orebro.se/fordjupning/fordjupning/fakta-statistik-priser--utmarkelser/information-tillganglig-for-ateranvandning/inkomna-leverantorsfakturor-reskontra--kontoklasser.html) och [Lidingö](https://lidingo.dataplattform.se/#/data/leverantorsfakturor)). Varje gång tack vare en pionjär som såg tidig potentialen av att göra det, såsom Kim Lantto eller Björn Hagström som redan skrev om det på sin blogg 2015[^fn:10]. Dessa initiativ måste hyllas men de visar knappt en positiv utveckling och kan inte dra nytta av en storskalig publicering.

Om vi fortsätter på samma takt kan vi anta att SKR kommer börja driva frågan i 2050 och alla kommuner publicera vid 2070. Det här är helt oacceptabelt.

![Quote by Greta Thunberg: We have not come to beg world leaders to care. We have come to let them know change is coming.](greta.webp "Gretas kamp är kanske 100x viktigare men hon är inspirerande när man försöker att agera och att bryta den status quo som ofta finns i den offentliga sektorn")

## Vårt projekt!

På grund av allt detta har Civic Tech Sverige bestämt att starta ett projekt om detta ämne. Vi hoppas att kunna:

* **Skapa medvetenhet!**
* Utforska vilka möjligheter finns för att öppna denna data och vilka svårigheter skulle finnas;
* Skriva vägledningar och sätta standarder för att hjälpa offentliga aktorer att publicera data på ett enkelt sätt;
* Skapa prototyper för att visa vad man skulle kunna göra med data;
* (och slutmålet) Skapa ett ekosystem för innovation kring upphandlingsdata som gynnar alla involverade aktorer och spara offentliga pengar!

Projeket heter nu *Öppen Upphandling* eftersom vi hittade inget bättre namn men vi välkomnar kreativa förslag!

Låter det spännande? Vad väntar du på? Alla är välkomna att bygga något med vad vi gör så länge man följer principer av öppen innovation och öppna data!

Hör av dig om du jobbar för en offentlig institution, ett privat bolag eller en journalist och du vill delta! Vi håller på att starta en arbetsgrupp och vi är väldigt intresserade av dina behov!
Kontakta oss på [e-post](mailto:pierre@mesu.re) eller direkt på vår [Matrix.org chatt](https://app.element.io/#/room/#civictechsweden:matrix.org).

---

**UPPDATERING**: Vi fick finansiering från Vinnova för att driva detta projekt med Open Knowledge Sweden, DIGG och partners som FGJ och Transparency International Ukraine. Projektet heter nu OpenUp! och har [sin egen webbplats](https://openup.okfn.se).

**UPPDATERING 2025**: Tyvärr har vårt projekt inte lett till de stora förändringarna vi hoppades för. Jag (Pierre) kämpar fortfarande på alla möjliga sätt för öppna upphandlingsdata och du får gärna kontakta mig om du vill prata eller samarbeta om det. 🙂

## Fotnoter

[^fn:1]: [Statistikrapport: Offentlig upphandling 2018 (konkurrensverket.se)](https://www.konkurrensverket.se/globalassets/publikationer/rapporter/rapport_2018-9_statistikrapport_2018_webb.pdf)
[^fn:2]: [DIGG om obligatorisk e-faktura (Arkiverad, digg.se)](https://web.archive.org/web/20200103195603/https://www.digg.se/nationella-digitala-tjanster/e-handel-och-e-faktura/obligatorisk-e-faktura-till-offentlig-sektor)
[^fn:3]: [SFTI om PEPPOL (sfti.se)](https://sfti.se/sfti/standarder/peppolbisehandel/peppolbisbilling3.49021.html)
[^fn:4]: [Recommendations for the Implementation of Open Public Procurement Data (Arkiverad, opentender.eu)](https://web.archive.org/web/20220331045834/https://opentender.eu/blog/2017-03-recommendations-for-implementation/)
[^fn:5]: [From the fires of revolution, Ukraine is reinventing government (wired.com)](https://www.wired.com/story/ukraine-revolution-government-procurement/)
[^fn:6]: [Jaimie Boyd on transparency in Canadian procurement (medium.com)](https://jaimieboyd.medium.com/canadas-open-by-default-procurement-pilot-an-experiment-in-agility-e10c9acd5806)
[^fn:7]: [Improving and opening up procurement and contract data (gds.blog.gov.uk)](https://gds.blog.gov.uk/2015/11/19/improving-and-opening-up-procurement-and-contract-data/)
[^fn:8]: [Open Data Laws in France Increase Competition for Public Contracts (ogpstories.org)](https://www.ogpstories.org/open-data-laws-in-france-increase-competition-for-public-contracts/)
[^fn:9]: [Förberedande studie om vissa inköpsvärden (upphandlingsmyndigheten.se)](https://www.upphandlingsmyndigheten.se/kunskapsbank-for-offentliga-affarer/publikationer/slutrapport-vissa-inkopsvarden/)
[^fn:10]: [Från pappersarkiv till öppna data (Arkiverad, blogg.orebro.se)](https://web.archive.org/web/20231206053715/https://blogg.orebro.se/enklarevardag/2015/09/10/fran-pappersarkiv-till-oppna-data/)
