---
title: PolitiX
subtitle: Is your Member of Parliament on X (and Bluesky, Mastodon...)?
excerpt: A mapping of our elected officials' social media presence to show how many remain on Elon Musk's platform and how many have found new channels.
date: 2026-02-02
tags:
  - Social Media
  - Open Data
  - OSINT
links:
  - label: PolitiX
    url: https://politix.mesu.re
    icon: link
  - label: Source code
    url: https://github.com/PierreMesure/politix-sweden
    icon: github
---

{{< project-links >}}

## X/Twitter has become a danger to our democracy

Researcher Carl Heath has written extensively[^fn:1] [^fn:2] [^fn:3] [^fn:4] about the problems that arise when X/Twitter is still used by our politicians and media, even though the platform has been hijacked by tech billionaire Elon Musk. Musk actively uses it to undermine our democracy, influence elections, and train his AI service Grok, which turns AI-revenge porn and deep fakes into a commodity.

## Yet most politicians remain there

Despite these developments, a surprisingly large part of the Swedish political establishment remains on X (ex-Twitter). It continues to be used as a primary channel for announcements and debate.

But what do the numbers actually show? Have Members of Parliament begun to seek out decentralized alternatives like Bluesky or Mastodon, or are they stuck in Musk's ecosystem? I wanted a clear overview so I decided to build **PolitiX** to find the answer.

The tool reveals that many politicians remain on X, and a significant portion is still active. Only 10% have joined Bluesky and 2.5% Mastodon, but very few remain active on these platforms. Most on the latter two platforms belong to left-leaning parties, but far from all. Overall, over 72% of the governing "Tidö" coalition remain on X, while less than 63% of the opposition have an account.

## How does PolitiX work?

PolitiX consists of several parts:

- A script that fetches data from Wikidata about who the current MPs are and what social media accounts they have. This allowed me to build on a dataset that was largely complete, although I needed to add about 50 accounts and review all data. The best part is that my contributions can be used by many others and everyone can help keep the data updated in the future.
- A "scraper" that visits each profile page on X to check if the profile still exists and when the user last tweeted. Since Musk shut down Twitter's API for researchers and journalists, it is unfortunately difficult to retrieve such information without paying a high price. Difficult, but apparently not impossible, as I succeeded after a few hours.
- An interface for browsing the data, filtering it by several interesting angles I chose, and visualizing it graphically in a way that resembles a parliament (using a fantastic JS package: [parliament-svg](https://github.com/juliuste/parliament-svg)).

[^fn:1]: [The threat of X and why Sweden cannot wait until the 2026 election (in Swedish, carlheath.se)](https://carlheath.se/hotet-x-och-varfor-sverige-inte-kan-vanta-till-valet-2026/)
[^fn:2]: [How Elon Musk can influence the Swedish election (in Swedish, carlheath.se)](https://carlheath.se/sa-kan-elon-musk-paverka-det-svenska-valet/)
[^fn:3]: [X – the platform that is itself the perpetrator (in Swedish, carlheath.se)](https://carlheath.se/x-plattformen-som-sjalv-ar-forovare/)
[^fn:4]: [Is our democratic conversations doomed to be shared on digital rollercoasters? (in Swedish, carlheath.se)](https://carlheath.se/maste-vara-demokratiska-samtal-vara-domda-att-delas-pa-digitala-tivolin/)
