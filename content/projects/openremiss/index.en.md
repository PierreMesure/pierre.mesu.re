---
title: OpenRemiss
subtitle: Swedish referrals as open data
excerpt: A script to download and structure referral data from regeringen.se
date: 2017-05-01
author: Pierre Mesure
draft: false
tags:
  - opengov
  - open parliament
  - transparency
categories:
  - Open data
layout: single
---

{{< button href="https://github.com/DinRiksdag/OpenRemiss" target="_blank" >}}
{{< icon "github" >}} Source code
{{< /button >}}

## What is a "remiss"?

The referral process (*remiss*) is a critical step in the Swedish legislative process. Before the Government Offices draft a formal bill (*proposition*) for Parliament, the public inquiries (*utredningar*) used to support the work are released and opened for a public round of feedback.

This process is sometimes criticised for being slow or because consulted public bodies do not always speak clearly or independently. Furthermore, the government has been accused of ignoring feedback or skipping the referral stage altogether. In my view, the primary issues are a lack of transparency and that the process is largely adapted for lobbying by corporate interests and organised civil society, often overlooking the voices and opinions of a large segment of the population, particularly marginalised groups.

To open up this process, I created *Din Riksdag* and designed a system for collaboratively written petitions called *medborgarremissvar* (citizen feedback). However, I needed access to all existing referral responses (*remissvar*), which led to the creation of OpenRemiss.

## Just PDFs on a plain website

![A visualisation of the problem with the government producing low-quality data](illustration.webp "A visualisation I made in 2017. Unfortunately, little has changed.")

Despite many requests from other government bodies, journalists, and researchers, the Government Offices (*Regeringskansliet*) refuse to provide their publications as open data. When it comes to the referral process, the essential data is structured as follows:

- The list of referral processes must be scraped from HTML pages, alongside metadata about the related public inquiries (*utredningar*).
- The list of files for each specific process also requires HTML scraping.
- The list of organisations invited to provide feedback (*remisslista*) is published as a PDF file. Furthermore, every department uses its own template for this list, so standardised extraction is not straight-forward. Organisations are often listed only by name, with a surprising number of typos and variations.
- The referral responses (*remissvar*) themselves are also PDFs, the format requested by the government. Each organisation uses its own template, making content extraction difficult without losing formatting or context.
- Feedback submitted by organisations not included in the original *remisslista* is not even published. These must be requested under the Freedom of Information Act and are often provided as physical paper for a fee.
- Similarly, the government's own analysis of the feedback (*remissammanställning*) is not public, though a brief summary is usually included at the end of the subsequent bill.

**OpenRemiss** is a script designed to automatically download this information (except for the last two items) and convert it into structured formats suitable for analysis, research, and innovative services. It downloads lists of referral processes with their metadata, fetches the files for each process, and converts *remisslistor* into structured lists while cleaning up organisation names.

Interestingly, this project led to my current role at the data lab of the [Swedish Agency for Financial and Public Management](https://www.statskontoret.se) (*Statskontoret*). I connected with them while they were building *Hitta remissvar* ("Find referral responses") and a similar scraper to collect the necessary data. The interface built  before my time there clearly demonstrates the potential of open, structured referral data, as do subsequent projects we have done with researchers and the Government Offices.

Since then, I have also built [g0vse](../g0vse), a scraper that can fetch any information from regeringen.se, though it does not handle *remisslistor* or name cleaning.

Don't hesitate to reach out if you're interested in using the code or data from this project! I’m happy to help you get started and to collaborate on making this data more accessible.
