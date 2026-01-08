---
title: Din Riksdag
subtitle: Making the Swedish legislative process more participative and transparent
excerpt: A platform to follow the creation of laws and participate in the process
date: 2018-05-01
author: Pierre Mesure
draft: false
tags:
  - open parliament
  - citizen participation
  - transparency
layout: single
---

{{< button href="https://github.com/DinRiksdag/dinriksdag" target="_blank" >}}
{{< icon "github" >}} Source code (platform)
{{< /button >}}
{{< button href="https://github.com/DinRiksdag/decidim-module-riksdagen" target="_blank" >}}
{{< icon "github" >}} Source code (scraping module)
{{< /button >}}
{{< button href="https://github.com/PierreMesure/pierre.mesu.re/tree/master/static/dinriksdag/presentations" target="_blank" >}}
{{< icon "link" >}} Presentations
{{< /button >}}

## Learning that Swedish democracy is far from perfect

I came to Sweden in 2016 and as far as I can remember, I have always been fascinated by its democracy. During my first years in Stockholm, I often visited the parliament, sitting above the main chamber and listening to the debates. Swedish parliamentary democracy had something I didn't grow up with: a proportional voting system, high levels of trust, less polarisation, and a great deal of consensus and respect for institutions and processes.

In my home country, distrust and anger were at record highs. But because of that, France was also bubbling with an enormous drive to hold politicians under scrutiny and accountable, and many citizens had a strong will to get involved in the decisions that affected them. To meet this demand, countless innovative projects were started in the 2010s, and institutions were reformed (slightly) to allow these new forms of democracy to have an impact.

When I arrived, I regarded Sweden as the pinnacle of democracy and was certain none of this was new here. I was wrong. Perhaps because of this high trust, information on elected representatives' private interests is not available as open data. Until recently, it had to be requested and collected physically for a hefty fee. Sweden is the only democracy around the Baltic Sea that doesn't give citizens the possibility to write petitions to start debates in its parliament. The official process to give feedback on future legislation (called *remissprocessen*) is tailored to corporate interests and organised civil society but leaves very little room for grass-roots engagement and significantly lacks transparency.

## Building Din Riksdag, one workshop at a time

Naively, but with a genuine drive to improve things, I started a project called **Din Riksdag**. Din Riksdag's goal was to become a platform where citizens and grass-roots groups could get a better understanding of the legislative process and have an impact on it.

I quickly realised how little interest there was from institutions and political forces to reform the current system, so I decided to build something that would "hack" it rather than await change from within. I drafted two potential mechanisms:

- ***citizen referral responses*** (*medborgarremissvar*) to be sent to the government before they start drafting the bill.
- ***citizen motions*** to be sent when the bill is discussed in parliament.

Both could be crafted collaboratively and gather support through votes, giving increased legitimacy to popular proposals and making it easy for both the Government Offices and parliament committees to include them in the lawmaking process when creating the bill (*proposition*) and the committee report (*betänkande*), respectively.

These ideas came from personal research but also through feedback and ideas from various workshops I conducted throughout 2017 and 2018.

## Swedish civic tech?

To support this new process, I also set up a digital platform where the entire legislative process was replicated and interactive, a website where citizens could browse through public inquiries (*utredningar*), referrals (*remisser*), bills (*propositioner*), and parliament activity, as well as submit or support citizen feedback and motions. I used the leading civic tech tools of the time: first Consul, then Decidim, and developed modules to integrate Swedish legislative data.

Unfortunately, despite the parliamentary administration's best efforts, a lot of that data remains unavailable in a structured format. That is why I started projects like [OpenRemiss](../openremiss) and ultimately [g0v.se](../g0vse) to make it easier to reuse data from regeringen.se.

## Turning the page

Although I never officially ended Din Riksdag, I stopped investing my time in it around mid-2018. At that time, I met the founders of Digidem Lab (Sanna, Anna, and Petter) and decided to join them to apply my newly acquired skills to other participatory projects in Sweden. Together, we used Decidim in many municipalities here and abroad and introduced methods such as participatory budgeting and citizens' assemblies.

My hope was that if I gave the national institutions a few years, they would mature and become more interested in letting citizens have their say. As I said earlier, I was very naive.