---
title: PolitiX
subtitle: Finns din riksdagsledamot på X (och Bluesky, Mastodon...)?
excerpt: En kartläggning av våra folkvaldas närvaro på sociala medier för att visa hur många som är kvar på Elon Musks plattform och hur många som hittat nya kanaler.
date: 2026-02-02
tags:
  - Social Media
  - Open Data
  - OSINT
links:
  - label: PolitiX
    url: https://politix.mesu.re
    icon: link
  - label: Källkod
    url: https://github.com/PierreMesure/politix-sweden
    icon: github
---

{{< project-links >}}

## X/Twitter har blivit en fara för vår demokrati

Forskaren Carl Heath har vid flera tillfällen skrivit[^fn:1] [^fn:2] [^fn:3] [^fn:4] om problemen när X/Twitter fortfarande används av våra politiker och medier när plattformen har kapats av techmiljardären Elon Musk som aktivt använder den för att underminera vår demokrati, driva påverkanskampanjer och träna sin AI-tjänst Grok som utsätter kvinnor för sexuella nätbrott.

## Ändå är de flesta politikerna kvar där

Trots utvecklingen är en förvånansvärt stor del av det svenska politiska etablissemanget kvar på X (tidigare Twitter). Det används fortfarande som en primär kanal för utspel och debatt.

Men hur ser det egentligen ut i siffror? Har riksdagsledamöterna börjat söka sig till decentraliserade alternativ som Bluesky eller Mastodon, eller är de fast i Musks ekosystem? Jag saknade en tydlig överblick och bestämde mig för att bygga **PolitiX** för att ta reda på svaret.

I verktyget ser man att många politiker är kvar på X och en betydande andel är fortfarande aktiv. Bara 10% har skaffat Bluesky och 2,5% Mastodon men väldigt få är fortsatt aktiva på dessa plattformar. De flesta på de två sista plattformarna tillhör partier till vänster, men långt ifrån alla. Totalt sett är över 72% av Tidökoalitionen kvar på X medan under 63% av oppositionen har ett konto.

## Hur fungerar PolitiX?

PolitiX består av flera delar:

- ett skript som hämtar uppgifterna från Wikidata om vilka är riksdagsledamöter och vilka social konton dessa personer har. På detta sätt kunde jag bygga på en datamängd som var i stort sett färdigt även om jag behövde lägga till ett 50-tals konton och granska alla uppgifter. Det bästa är att mina kompletteringar kan användas av många fler och att alla kan hjälpa att hålla datan uppdaterad i framtiden.
- ett så-kallat *scraper* som besöker varje profilsida på X och kollar om profilen fortfarande finns och när användaren twittrade senast. Sedan Musk lade ner Twitters API för forskare och journalister är det tyvärr svårt att hämta sådana uppgifter utan att betala dyrt. Svårt men tydligen inte omöjligt eftersom jag lyckades efter några timmar.
- ett gränssnitt för att bläddra i uppgifterna, filtrera dem efter flera olika intressanta vinklar som jag valde, och visualisera dem på ett grafiskt sätt som liknar ett parlament (det finns ett fantastiskt JS-paket som gör just detta: [parliament-svg](https://github.com/juliuste/parliament-svg))

[^fn:1]: [Hotet X och varför Sverige inte kan vänta till valet 2026 (carlheath.se)](https://carlheath.se/hotet-x-och-varfor-sverige-inte-kan-vanta-till-valet-2026/)
[^fn:2]: [Så kan Elon Musk påverka det svenska valet (carlheath.se)](https://carlheath.se/sa-kan-elon-musk-paverka-det-svenska-valet/)
[^fn:3]: [X – plattformen som själv är förövare (carlheath.se)](https://carlheath.se/x-plattformen-som-sjalv-ar-forovare/)
[^fn:4]: [Måste våra demokratiska samtal vara dömda att delas på digitala tivolin? (carlheath.se)](https://carlheath.se/maste-vara-demokratiska-samtal-vara-domda-att-delas-pa-digitala-tivolin/)
