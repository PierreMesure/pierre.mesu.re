---
title: g0v.se
subtitle: regeringen.se as open data
excerpt: A scraper to make it easier to access data and documents from regeringen.se
date: 2024-04-15
tags:
  - Open data
  - Opengov
  - Scraping
---

{{< icon-button "g0v.se" "link" >}} g0v.se {{< /icon-button >}}
{{< icon-button "github.com/civictechsweden/g0vse" "github" >}} Source code {{< /icon-button >}}
{{< icon-button "github.com/civictechsweden/g0vse/tree/data" "github" >}} Data {{< /icon-button >}}

![Logo of g0v.se](g0vse.webp "The project's logo is inspired by the Swedish three crowns but they have been replaced by sunflowers to honour the Taiwanese sunflower movement that started the g0v philosophy")

I arrived in Sweden in 2016 and I quickly started to build services building on government and legislative data. The Swedish parliament (*Riksdagen*) publishes open data since 2010 on all its activities and production. Unfortunately, all the activity of the government as well as preparatory work for legislation is controlled by the government chancellery offices (*Regeringskansliet*) and they have very little interest in open data, transparency and democratic innovation. They are also generally struggling with digitalising themselves.

I know that because I have met with them countless times and tried to get them to improve the situation, with no avail. So I tried to make information from their website ([regeringen.se](https://www.regeringen.se)) more accessible through projects such as Din Riksdag, OpenRemiss. And with each one of them, I gained a better understanding of their systems, the way their data is organised. On the way, I also encountered with countless journalists, researchers, companies and even government bodies struggling with the same problem.

And so in 2024, I decided to put all that accumulated knowledge into g0vse, a project that downloads all information from the government's website every night and makes it available as open data in a format that people can actually reuse.

You can read more (in Swedish) on [g0v.se](https://g0v.se) and about the technical aspects (in English) on [Github](https://github.com/civictechsweden/g0vse).
