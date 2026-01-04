---
title: Hej Ulf!
subtitle: A deep dive into a targeted political advertisement campaign and the first Swedish crowdsourced GDPR complaint
excerpt: In 2022, I received a personalised video message from then prime minister candidate Ulf Kristersson during the election campaign. It led me down a rabbit hole to understand why and how Ulf was sending
date: 2022-09-30
author: Pierre Mesure
draft: false
tags:
  - GDPR
  - OSINT
categories:
  - GDPR
layout: single
links:
- icon: newspaper
  icon_pack: fas
  name: Original article (on webperf.se)
  url: https://webperf.se/articles/hej-ulf/
- icon: link
  icon_pack: fas
  name: hejulf.se
  url: https://hejulf.se
- icon: github
  icon_pack: fab
  name: website
  url: https://github.com/PierreMesure/hejulf.se
- icon: github
  icon_pack: fab
  name: scraper
  url: https://github.com/PierreMesure/hej-ulf
---

## Hej Pierre

2022 was an election year in Sweden. Political parties were campaigning at national and regional levels and following an ongoing trend, a larger share of the campaign was now digital.

![Screenshot of a video showing Ulf Kristersson saying "Hej Pierre"](hej-pierre.webp)

At the beginning of September, I received an e-mail from Ulf Kristersson, then prime minister candidate with the subject "Hej Pierre". It asked me to open a video with a personalised message. The video featured Ulf Kristersson seated at a desk looking at me and reciting some points of his program. But several things caught my attention: Ulf Kristersson was also starting with "Hej Pierre" (which startled me like I guess many others who received this message) and at some point of his speech, Ulf Kristersson pointed to a tablet on his desk where the mayor of my city, Solna, had recorded a message encouraging me to vote for their party locally.

> Freaky, I thought. Why am I receiving this? How does Ulf Kristersson know about me, my name and my address?

## Analysing the ad campaign

So I decided to investigate. I started by exploring the website on which the video message was embedded. I discovered the company behind the ad campaign, the technical method they used to stitch bits of videos and make it seem magical when most parts were in fact the same for everyone. I also managed to algorithmically recreate several hundreds of thousands of unique links corresponding to as many personalised messaged that were sent to other people: "Hej Annika", "Hej Waldemar", "Hej Anna". It seemed that Ulf Kristersson had spent half a day recording over 2000 *hälsningar*, and you could even see how the light from the window changed between the snippets.

![Mozaic of screenshots from similar videos where Ulf is saying hey to various names](thumbnail.webp)

When I talked about it with friends, I realised some of them had received other personalised variations of the video. All had the same reaction: spooky, and is this even legal?

I gathered a list of GDPR violations from Ulf Kristersson's party (*Moderaterna*) and their technical partners and I discussed it with several specialists. I got valuable feedback and decided to submit a complaint to the Swedish authority for privacy protection (*Integritetsskyddsmyndigheten, IMY*). Unfortunately, it is infamously known for its reluctance to investigate complaints and I knew that my efforts would likely end up in the bin as well.

## Building a counter-campaign

But I also knew that many people got similar video ads (from my investigation, I think they were over 400 000) so I decided to give these people an opportunity to stand behind the complaint.

![Screenshot of hejulf.se](hejulf.se.webp)

IMY doesn't accept group complaints so I created a simple website where anyone could send their own complaint with a few clicks (it used to be at hejulf.se but it's now moved to [my domain](https://hejulf.mesu.re)). I also wrote a [blog post on webperf.se](https://webperf.se/articles/hej-ulf/) and I posted everything on Twitter and LinkedIn with a funny video. I waited until after the election night both because I wasn't completely ready before and because I wasn't sure of the reception in the final days of the campaign.

It spread quicker than I imagined and I rapidly got hundreds of messages from people who had also received the message. About 150-250 managed to send a complaint despite some technical issues on my website. I also received a lot of hate messages on Twitter from political supporters on the right.

The story got picked up by specialised media and I got interviewed by [Dagens Media](https://www.dagensmedia.se/medier/digitalt/moderaternas-sms-utskick-massanmals-efter-kampanj-kande-mig-krankt/)/[Resumé](https://www.resume.se/marknadsforing/strategi/moderaternas-sms-utskick-massanmals-efter-kampanj-kande-mig-krankt/).

## What happened since then?

Six months later in March 2023, IMY decided to [start an investigation](https://www.imy.se/nyheter/imy-inleder-tillsyn-av-moderaterna/) (*tillsyn*), which was in itself a victory since they only did it for [less than 5%](https://www.datajurist.se/imy-lyssnar-inte-forsta-gangen/) of the complaints at that time. Most news outlets talked about it but few went into the details of what happened.

Unfortunately, this investigation seems to have disappeared in some kind of black hole as it is still unresolved 3 years and 3 appointed jurists later. I sincerely hope that IMY takes this issue seriously and publishes their decision soon since new jurisprudence will have an impact on how political parties use personal data in the next election.
