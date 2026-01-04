---
title: Jag vill ha vaccin!
subtitle: A user-friendly platform to find a vaccine time no matter where you live in Sweden
excerpt: Finding a vaccine time was chaotic in Sweden. Each region went for their own solutions, often discriminating against vulnerable groups who struggled to find a time on unaccessible and hard to navigate webpages. In France, a group of hackers built a national platform in a few days that greatly simplified the process, and I decided to copy them.
date: 2021-05-01
author: Pierre Mesure
draft: false
tags:
  - COVID
  - OSINT
categories:
  - Open data
layout: single
---

## Finding a vaccine time in Sweden

Like the other countries, Sweden started vaccinating its population in the beginning of 2021. Starting with the most vulnerable and slowly expanding the campaign to younger age groups. Except, Sweden's healthcare system is regional, with surprisingly little collaboration between the regions. In particular, the digital systems used in Swedish healthcare are often criticised for the lack of common data standards, API, and a tendency to reinvent the wheel (or rather pay an expensive consultant to do so) or to fall into the claws of an expensive and ineffective monopoly.

This was not a good foundation for a successful vaccination campaign, when everyone expected to be able to book a vaccine time online. The result was exceptionnally... diverse, even though I could not foresee how bad it was when I started this project.

A few regions decided to use 1177, a robust solution in terms of authentication and user interface, but that completely lacked a way to get an overview of what vaccine times were available and were. The regions of Stockholm and Gotland decided to use their app Alltid Öppet, a proven solution used for all other healthcare bookings. Unfortunately, the app did not allow to see if there were times available without logging in with BankID, leading to numerous crashes when several hundred thousands tried to log in to access the few hundreds of times that were added every now and then, and hindering patients to access more important care. It was also reported that the region needed to invest several thousands of crowns in server costs to meet a demand that was for the most part unsuccessful and unneeded. One region simply gave up with online bookings and decided to contact all their citizens by phone individually. Finally, the rest of the regions went for private solutions, with surprisingly poor user-friendliness. In Region Sörmland, a user had to click manually on every vaccination centre to see if they had any time that week, then clicking forward several times to explore the following weeks. The worst was for citizens of the regions of Västra Götaland and Skåne, whose authorities decided to delegate the booking infrastructure to each individual center. Min Doktor, Din Doktor, Doktor.se, etc. In cities like Göteborg and Malmö, it wasn't uncommon to have to create 3-4 accounts to see the (un)available times in the various centres of your district.

In comparison, on the other side of the Öresund, the Danish government had set up a unique portal. Right next to the login button, a red sign deterred users from clicking it if no time was available.

## The French example

France was initially a lot more chaotic, and much like the worst Swedish examples, the government delegated the booking  responsibility to each vaccination centre. These health centres were in turn using 5-6 different e-healthcare platforms showing the times without login, a welcome centralisation but still way too much to make it easy for everyone.

France has a strong culture of hacktivism, people who can create software and use their skills for the common good. Many solutions were creating during the pandemic but one gained incredible traction. The platform Vite Ma Dose, started by Guillaume Rozier, aimed at gathering vaccine bookings in one simple user interface for the whole country. The code was open, and the website scraped, every minute, the available times from several hundreds vaccination centres.

Quickly, over 100 people joined the project, maintaining the data flows, improving the website's search functions and accessibility, Within days, mobile apps were on the App stores and communication material was created to reach out to all audiences. The traffic exploded. Seeing the benefit of this grass-root solution, the French government decided to support and promote the initiative. Vaccine platform providers also set up APIs to make it easier for their times to be republished, seeing this new webpage as a welcome buffer relieving their servers from the millions of visits they had experienced at the beginning of the campaign. At the end of the year, over 100 million visitors had used the website.

Guillaume Rozier ended up receiving the medal of national merit, the government praising his and others' initiative for saving lives and helping millions of people.

## Creating Jag vill ha vaccin!

As most frenchmen, I heard of this initiative when the media started talking about it, early April 2021. I had a look at the source code and it was easy to understand. I decided to spend a few hours investigating whether it would be possible to reproduce the same service in Sweden. I had a look at how vaccine bookings were made available in all the regions and I quickly realised that a lot of them could be scraped automatically. None provided open data but a script imitating a user and going through the websites could save the information in a structured way. I ended up spending a whole weekend in my room setting up a prototype. At the end, I had a copy of the original Vite Ma Dose, still in French, but with Swedish vaccination centres in the search results. I quickly translated the webpage and published it under the name "Jag vill ha vaccin!" with a quick post on LinkedIn and Twitter to ask for feedback. It quickly took off.

## The landing

Despite my limited audience on these platforms, the posts spread and over 10 000 people visited the website the first day. Several journalists started contacting me. I was taken aback, especially because their questions were often framing my little prototype as a solution to the failure of the regions and their big budgets. At the time, I knew too little about how bad some of their systems were and I had mostly started this little project as a fun experiment.

What I hadn't foreseen either was that the same journalists would go to the regions and ask them why a single person could deliver what they couldn't. The press secretaries answered without knowing what this was about and recommended not to use the service, citing potential data theft and security issues as risks. Several regions' platform providers changed their systems in an attempt to make it harder for me to get their vaccine times. None of the regions tried to contact me though, so I resorted to do it.

I contacted all regions and managed to get meetings with about half of them. Most were very adamant that I stop what I was doing. Their reasons were often confusing and driven by fear but a good argument was that users could miss the information they were required to read before booking by finding a time through my solution. I made sure to fix that by sending all users to the information pages on the respective region's website. Another one was the risk if the service started to send viruses to users. *Jag vill ha vaccin!* didn't track users and did not collect any personal information. But no matter who I spoke to, the region employees' of how it worked was very limited. I suggested the regions could just take the code I wrote and host it themselves on their own servers. But the culture of open source is unfortunately not strong in the Swedish public sector so no region accepted the offer.

I vividly remember a meeting with Daniel Forsberg, then a leading politician on the matter for Region Stockholm (now a lobbyist). I was offering to show their vaccine times on *Jag vill ha vaccin!* so their app would stop to be unavailable because of the heavy traffic. He kept repeating how pro-innovation he was and how important innovation and open data were for the region but how in that specific case, it was unfortunately not welcome.

In the end, only one region welcomed collaboration, Västra Götaland. The region's executives had noticed how disastrous the situation was in the region, with over 15 private providers releasing vaccine times on their proprietary platforms. Not even them could have an overview of how vaccine doses were used. A small team was tasked to build an official page to gather vaccine times and among them was Marcus Österberg, creator of webperf.se. A strong advocate of Internet standards and openness, he quickly published the data for the whole region as open data.

This enabled me to make the service more exhaustive and add providers that was unaccessible before. Ironically, Jag vill ha vaccin was still showing more times than the region's official platform as their team had to ask for the data from all the private providers. I simply scraped it without asking for permission, knowing the Freedom of Information act and public interest were on my side.

## The end

Unfortunately, the project never got the backing I hoped it would from the regions and despite some popular support and media coverage, I could only gather about half of the vaccine times in the country, with a number of regions insisting I stop publishing at all. I was even threatened personally of lawsuits by the manager of a healthcare centre, an uncomfortable half an hour of being agonised on the phone.

Although I never stopped the website, the number of visitors slowly decreased after the initial peak and Jag vill ha vaccin became irrelevant when everyone got their first vaccine dose and scarcity stopped being a problem.

Whenever journalists reached out to me, often asking me about the regions' solutions in the hope that I would give them critical quotes to use to build an antagony, I explained that all the vaccine time history that Jag vill ha vaccin! gathered every few minutes was available as open data and that a lot of it could be used to analyse the effectiveness of the vaccine rollout in each region. I used it myself to report on centres with hundreds of available times while other parts of the region had none. Unfortunately, this required more time than they seemed to have to write their article so this data remain mostly unused to this date (message me if you're an interested researcher, I archived it 😉).

## Morale of the story

Unlike its French counterpart, and to my initial disappointment, Jag vill ha vaccin never became a success story. But success was never the main goal and this project taught me a lot, not just technically but also on the Swedish public sector and its problems with digitalisation.
