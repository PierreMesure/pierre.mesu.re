---
title: Hej Ulf!
subtitle: En djupdykning i en riktad politisk reklamkampanj och det första svenska crowdsourcade GDPR-klagomålet
excerpt: År 2022 fick jag ett personligt videomeddelande från dåvarande statsministerkandidaten Ulf Kristersson under valrörelsen. Det ledde mig in i ett grävprojekt för att förstå varför och hur Ulf gjorde det
date: 2022-09-30
tags:
  - GDPR
  - OSINT
---

{{< icon-button "webperf.se/articles/hej-ulf/" "pencil" >}} Ursprungliga inlägg (webperf.se) {{< /icon-button >}}
{{< icon-button "hejulf.mesu.re" "link" >}} hejulf.se {{< /icon-button >}}
{{< icon-button "hejulf.mesu.re/beskrivning-klagomal.pdf" "pencil" >}} Klågomål till IMY {{< /icon-button >}}
{{< icon-button "github.com/PierreMesure/hejulf.se" "github" >}} Webbsida (källkod) {{< /icon-button >}}
{{< icon-button "github.com/PierreMesure/hej-ulf" "github" >}} Scraper (källkod) {{< /icon-button >}}

## Hej Pierre

2022 var ett valår i Sverige. De politiska partierna kampanjade på nationell och regional nivå och kampanjanerna var alltmer digitala.

![Skärmdump av en video som visar Ulf Kristersson som säger "Hej Pierre"](hej-pierre.webp)

I början av september fick jag ett e-postmeddelande från Ulf Kristersson, dåvarande statsministerkandidat, med ämnesraden "Hej Pierre". Det bad mig öppna en video med ett personligt meddelande. Videon visade Ulf Kristersson sittande vid ett skrivbord där han tittade på mig och läste upp några punkter ur sitt valmanifest. Men flera saker fångade min uppmärksamhet: Ulf Kristersson inledde också med "Hej Pierre" (vilket fick mig att haja till, precis som jag gissar att många andra som fick detta meddelande gjorde) och vid ett tillfälle i sitt tal pekade Ulf Kristersson på en surfplatta på sitt skrivbord där kommunstyrelseordföranden i min stad, Solna, hade spelat in ett meddelande som uppmanade mig att rösta på deras parti lokalt.

> Läskigt, tänkte jag. Varför får jag det här? Hur känner Ulf Kristersson till mig, mitt namn och min adress?

## Analys av reklamkampanjen

Så jag bestämde mig för att undersöka saken. Jag började med att utforska webbplatsen där videomeddelandet var inbäddat. Jag hittade företaget bakom reklamkampanjen och den tekniska metoden som användes för att foga samman videosegment och skapa en personlig illusion när det mesta av innehållet i själva verket var identiskt för alla. Jag lyckades också algoritmiskt återskapa flera hundra tusen unika länkar som motsvarade lika många personliga meddelanden som skickats till andra människor: "Hej Annika", "Hej Waldemar", "Hej Anna". Det verkade som om Ulf Kristersson hade tillbringat en halv dag med att spela in över 2000 *hälsningar*, och man kunde till och med se hur ljuset från fönstret förändrades mellan klippen.

![Mosaik av skärmdumpar från liknande videor där Ulf säger hej till olika namn](mozaic.webp)

När jag pratade om det med vänner insåg jag att några av dem hade fått andra personliga varianter av videon. Alla reagerade likadant: obehagligt, och är det här ens lagligt?

Jag samlade en lista över GDPR-överträdelser från Ulf Kristerssons parti (*Moderaterna*) och deras tekniska partners och diskuterade den med flera specialister. Jag fick värdefull feedback och bestämde mig för att lämna in ett klagomål till Integritetsskyddsmyndigheten (IMY). Tyvärr är myndigheten ökänd för sin ovilja att utreda klagomål och jag visste att mina ansträngningar sannolikt också skulle hamna i papperskorgen.

## Bygga en motkampanj

Men jag visste också att många människor fick liknande videoannonser (utifrån min utredning tror jag att det var över 400 000) så jag bestämde mig för att ge dessa människor en möjlighet att ställa sig bakom klagomålet.

![Skärmdump av hejulf.se](hejulf.se.webp)

IMY accepterar inte gruppklagomål så jag skapade en enkel webbplats där vem som helst kunde skicka sitt eget klagomål med några få klick (den låg tidigare på hejulf.se men har nu flyttats till [min domän](https://hejulf.mesu.re)). Jag skrev också ett [blogginlägg på webperf.se](https://webperf.se/articles/hej-ulf/) och jag lade upp allt på Twitter och LinkedIn med en rolig video. Jag väntade till efter valnatten både för att jag inte var helt klar innan och för att jag inte var säker på mottagandet under kampanjens sista dagar.

{{< video src="https://github.com/PierreMesure/hejulf.se/raw/refs/heads/main/public/hejulf.mp4" type="video/mp4" preload="auto" >}}

Det spred sig snabbare än jag anat och jag fick snabbt hundratals meddelanden från människor som också hade fått meddelandet. Omkring 150-250 lyckades skicka ett klagomål trots vissa tekniska problem på min webbplats. Jag fick också en hel del hatmeddelanden på Twitter från politiska anhängare på högerkanten.

Historien plockades upp av specialiserade medier och jag blev intervjuad av [Dagens Media](https://www.dagensmedia.se/medier/digitalt/moderaternas-sms-utskick-massanmals-efter-kampanj-kande-mig-krankt/)/[Resumé](https://www.resume.se/marknadsforing/strategi/moderaternas-sms-utskick-massanmals-efter-kampanj-kande-mig-krankt/).

## Vad har hänt sedan dess?

Sex månader senare, i mars 2023, beslutade IMY att [inleda en tillsyn](https://www.imy.se/nyheter/imy-inleder-tillsyn-av-moderaterna/), vilket i sig var en seger eftersom de bara gjorde det för [mindre än 5%](https://www.datajurist.se/imy-lyssnar-inte-forsta-gangen/) av klagomålen vid den tiden. De flesta nyhetsmedier rapporterade om det men ingen gick in på detaljerna om vad som hänt (som [SVT](https://www.svt.se/kultur/myndighet-inleder-tillsyn-mot-moderaternas-videohalsningar), [DN](https://www.dn.se/sverige/myndighet-granskar-moderaternas-valhalsning/), [Aftonbladet](https://www.aftonbladet.se/nyheter/a/zEVjeq/myndighet-granskar-m-efter-valet), [Altinget](https://www.altinget.se/artikel/myndighet-ska-granska-moderaternas-valsatsning)...).

Sedan försvann denna utredning i något slags svart hål innan IMY till slut kom fram till ett [beslut](https://www.imy.se/tillsyner/moderata-samlingspartiet-riksorganisationen/) i slutet av oktober 2025. I [Sveriges Radio](https://www.sverigesradio.se/artikel/myndighet-fel-av-m-och-sd-att-skicka-reklam-pa-sms) förklarar den ansvariga juristen att beslutet bör leda till en förändrad rättspraxis för hur politiska partier riktar sig till väljare under val med SMS och e-post. Samtycke krävs nu mer eller mindre, särskilt om innehållet anpassas till mottagaren med hjälp av personuppgifter.

Enligt min åsikt är detta ett beslut som får långtgående konsekvenser: användningen av kontaktuppgifter från kommersiella aktörer som köper adresser från Skatteverket, telefonnummer från mobiloperatörer och gömmer sig bakom ett så kallat *utgivningsbevis* är utbredd inom reklam. Och även om IMY fortfarande är mycket ovilliga att angripa dessa aktörer, åtnjuter deras kunder inte samma skydd (som Moderaterna i det här fallet) och kommer nu förhoppningsvis att vara mindre villiga att använda dessa data utan samtycke.

Inom politiken hoppas jag att detta kan vara en liten sten i en större mur som skyddar väljare mot desinformation och manipulation. Vi har sett hur mycket riktad reklam i USA 2016 [kunde leda till polarisering och manipulation i massiv skala](https://en.wikipedia.org/wiki/Project_Alamo) och den senaste utvecklingen inom dark patterns och AI kommer att göra det lättare i framtiden. Å andra sidan väcker detta den demokratiska frågan om hur partier ska kunna nå ut till väljare för att informera om sina idéer. Som svar på EU:s försök att reglera politisk reklam (DSA och TTPA) har de flesta sociala medieplattformar [beslutat att förbjuda det helt och hållet](https://opentermsarchive.org/en/publications/political-advertising-after-the-ttpa-exit-adaptation-and-the-future-of-platform-governance/). Vi behöver utveckla nya och bättre demokratiska utrymmen för att debattera idéer och fostra upplysta medborgare.
