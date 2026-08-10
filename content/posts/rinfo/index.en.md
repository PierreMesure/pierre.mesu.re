---
title: Laws are infrastructure
excerpt: "Over 25 years ago, Sweden decided to introduce a public legal information system to make laws available digitally. Unfortunately, this was never implemented and we still live with the consequences today: our legal information is fragmented, difficult to access and published in formats that are hard to reuse."
date: 2026-08-07
tags:
  - Open data
  - Legal information
  - Digitalisation
---

*Nul n’est censé ignorer la loi. Ignorantia juris non excusat.* No one is presumed to be ignorant of the law.

It is a harsh principle, but it rests on a reasonable premise: anyone who wants to obey the law must also be able to find out what it says. [The Supreme Court of Sweden has put it clearly](https://www.domstol.se/globalassets/filer/domstol/hogstadomstolen/avgoranden/2019/b-6130-18.pdf): if people are expected to know what constitutes a criminal offence, they must also be able to access the rules.

![The Swedish Code of Statutes in print at the Riksdag Library](featured-sfs-riksdagsbiblioteket.webp "The Swedish Code of Statutes in print at the Riksdag Library (CC BY 4.0 Pierre Mesure)")

Today, access to the law no longer means access to a printed statute book. Nearly all access is digital. On top of that, legal information is increasingly read and used by information systems, algorithms or AI-agents.

Machines do not read laws the way people do. They need persistent identifiers, structured text, clear versions, metadata and links between documents. Yet the Swedish state still publishes much of our legal information as if the primary need were to open a PDF file in a browser.

## Machines were reusing our laws long before ChatGPT

The discussion about AI may give the impression that machines using legislation is something new. It's not. Swedish public authorities have been building IT systems, algorithms and even spreadsheets based on our regulatory framework for as long as they have had access to computers. The Swedish Administrative Procedure Act expressly even permits automated decision-making, and [Digg provides extensive guidance](https://www.digg.se/kunskap-och-stod/automatisera-handlaggning-och-beslut/automatiserade-beslut) for public authorities seeking to automate case processing and decisions. That's just for government but the private sector also has many uses for the law.

The question, therefore, is not whether machines should use our regulatory frameworks. They already do. It is how to make sure they can rely on trustworthy, up-to-date and official legal information, not a poor copy that was extracted from a PDF or an old website.

Almost every week, I hear from colleagues at public authorities, doctoral students, journalists and private individuals trying to reuse legal information. One person needs to track a matter through the legislative process. Another wants to compile research material, examine how a rule has changed over time or create a service that helps people understand their rights.

They often ask the same questions: Where can the information be found? Is there an API? Can the documents be downloaded in bulk? How are an committee, a public investigation's report and a government bill connected?

Other countries have solved this many years ago. The French project [OpenFisca](https://openfisca.org/) turns large parts of the tax and benefits system into executable, open-source code. The project shows what becomes possible when rules are treated as shared digital infrastructure (*rules as code*), rather than as documents that every organisation must interpret from scratch.

![Screenshot of the French government's “1 jeune 1 solution” website](openfisca.webp "Thanks to rules as code, this website promises to show in five minutes whether you meet the eligibility criteria for 1,000 benefits, and to apply for some of them automatically ([link](https://mes-aides.1jeune1solution.beta.gouv.fr)).")

Another way to compare Sweden internationally is to look at the EU initiative [European Legislation Identifier (ELI)](https://eur-lex.europa.eu/eli-register/what_is_eli.html). Sweden finally joined in 2024, but we have yet to start publishing data because we lack the necessary data infrastructure. Denmark, [Finland](https://eur-lex.europa.eu/eli-register/finland.html) and [Norway](https://eur-lex.europa.eu/eli-register/norway.html) already use ELI to give legal information persistent identifiers and structured metadata.

![Countries implementing ELI; Sweden is one of the few EU countries that does not](eli.webp "Source: [EUR-Lex](https://eur-lex.europa.eu/eli-register/implementing_countries.html)")

## A legal information system made up mostly of links

Sweden has no functioning public legal information system worthy of the name. We have an ordinance stating that such a system must exist, around a hundred organisations responsible for different fragments and a central website that mainly links to them.

The [Legal Information Ordinance](https://rkrattsbaser.gov.se/sfst?bet=1999:175) (*Rättsinformationsförordningen*) was adopted in 1999. It was an ambitious text for its time and could have made Sweden a pioneer with excellent conditions for producing and providing access to digital legal information. Instead, we got [lagrummet.se](https://www.lagrummet.se): a collection of links and a collective failure. Twenty-seven years later, the website still does not contain the legal information itself and provides no common API.

In its own 2025 [review of the legal information system](https://www.domstol.se/globalassets/filer/gemensamt-innehall/rapporter/redovisning_en-saker-och-effektiv-tillgang-till-rattsinformation.pdf), the Swedish National Courts Administration writes that the current solution does not meet the needs identified by the authority “in any way. The report also notes that sources of law are published in many different ways, without common metadata and sometimes without even machine-readable markup for headings and preambles.

This failure is costing us dearly, probably hundreds of millions of kronor. It also weakens our shared democracy and trust in public administration, while impeding innovation and transparency.

The Government Offices of Sweden (*Regeringskansliet*) produce much of the information that the rest of the system needs: the Swedish Code of Statutes (*Svensk författningssamling*), government inquiries (*utredningar*), ministry publications (*promemorior*), government bills (*propositioner*), consultation documents (*remisser*) and countless material that thousands need to download and read every day. Despite this, and despite the authority itself facing major difficulties reusing its own data, there is not even the beginning of a coherent open API for the material.

For over fifteen years, the Riksdag has published extensive open data, largely thanks to very motivated employees who saw the need early. Its data also include government bills, written communications and inquiries that originally came from the government. Their work deserves praise, but they have been given an unreasonable responsibility without a clear mandate. Satisfactory data quality will never be possible as long as the Riksdag Administration has to process old document formats that were never intended to be made available in any way other than as PDF files on regeringen.se.

## The promising Rinfo project that never made it across the finish line

The worst part is that we know what needs to be done. Around 2010, the Swedish National Courts Administration (*Domstolsverket*) already ran the Rinfo project to create a modern legal information system. The project developed common URIs, a document model and RDF-based metadata. The authority even recruited Staffan Malmgren, who created [lagen.nu](https://lagen.nu) and has long been one of Sweden's foremost experts on digital legal information.

![A slide from the Rinfo project showing screenshots of public authorities’ regulatory pages](rinfo_slide.webp "Source: [Swedish National Courts Administration](https://www.slideshare.net/slideshow/rttsinformationssystemet/5903008)")

But the project remained an impressive prototype, and the decisions needed for broad implementation never came.

The Swedish National Courts Administration now acknowledges that Lagrummet lies outside its core activities. When every organisation is responsible for its own documents, but no one has real authority, funding or responsibility for the whole, the result is what we see today: a system on paper and a collection of links in practice.

## A hidden but substantial cost to society

When legal information is not published in a structured form, the need does not disappear. The work is merely pushed downstream. And innovative projects are abandoned before they see the light of day.

Public authorities each build their own integrations of variable quality. Researchers hand tedious tasks to master's students, who spend months collecting and cleaning documents before any analysis can begin. Journalists find it harder to follow legislation systematically and scrutinise those in power. Companies and non-profit projects write *scrapers* that break every time a public authority changes its website. The same documents are downloaded, converted, processed with OCR and classified again and again.

Each processing step also creates distance from the official source. A PDF may have been replaced without a clear version history. Metadata may have been misinterpreted. Relationships between documents may be missing. Updates may arrive too late. Even so, we use what we have, despite the mistakes it can cause.

Private legal databases serve an important purpose, but they can never replace a public foundational infrastructure. When the state publishes raw material of poor quality and then has to buy back access to refined versions of its own information, that is not efficient digitalisation. It means privatising the cost of understanding public information and then sending the bill back to us taxpayers.

## AI can help but not solve the problem

There are still reasons for optimism. AI makes it much easier to build and maintain tools that retrieve, classify and extract information from documents. It is faster to write scrapers, interpret old formats and identify connections between legal sources.

But AI must not become yet another excuse for leaving the fundamental problem unresolved. A language model attempting to reconstruct metadata from a PDF is not a legal information system. A probable interpretation is not an official source. The more organisations that must repair information after publication, the more opportunities there are for errors and conflicting versions.

The work must be done where the information is produced. From the outset, documents should have persistent identifiers, structured text, a version history, clear metadata and machine-readable relationships. Only then can AI and other digital tools be used safely, efficiently and in a way that can be audited.

## Lagdata, a small step in the right direction

I did not build Lagdata to solve all the problems described above by myself. Rather, it is a way to help those who want to reuse legal information today, despite the fact that we do not yet have the right infrastructure in place. It is a collaborative mapping of different types of legal information and how they can currently be accessed by machines.

The project documents where the information can be found, the formats in which it is published, the APIs and downloads that are available, and the independent projects that can convert and structure it. The goal is to ensure that public authorities, researchers, journalists and developers do not have to start from scratch every time.

The documentation is open and still quite incomplete as of now. I don't know enough about some documents to document how they should best be accessed. I therefore hope that more people who have wrestled with the same PDF files, websites and data structures will contribute what they have learned.

In the short term, Lagdata can lower the barrier to using the legal information that is actually available. In the longer term, I still hope that the state, and the Government Offices in particular, will take a bigger responsibility for publishing laws and other legal sources as the critical digital infrastructure they already are.

The day that happens, Lagdata will have become obsolete and I'll be immensely happy.
