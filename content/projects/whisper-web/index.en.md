---
title: Whisper-Web
subtitle: Transcribe audio speech into text locally in your browser
description: Whisper-Web is a privacy-focused web application that allows you to transcribe audio files using OpenAI's Whisper models directly in your browser. By performing the transcription locally, your audio data never leaves your device.
date: 2025-02-24
tags:
  - AI
  - Privacy
  - Open Source
---

{{< icon-button "whisper-web.mesu.re" "link" >}} whisper-web.mesu.re {{< /icon-button >}}
{{< icon-button "github.com/PierreMesure/whisper-web" "github" >}} Source code {{< /icon-button >}}

On Valentine's day of 2025, the Swedish National library's AI lab (KB-labb) released their own fine-tuned version of OpenAI's Whisper models. They retrained the models using thousands of hours of audio from both SVT (the Swedish public service) and parliament debates. Unfortunately, to avoid legal issues and to stay focused on their mission, the lab only provides the [open weights of the models](https://huggingface.co/KBLab/kb-whisper-large).

So I took a few hours to build a web interface to use the models as simply as possible. I called it Whisper-Web.

![Main UI of Whisper-Web, with a few buttons to upload or record audio and a transcript underneath](screenshot.webp "Whisper-Web's main UI")

The first time you give it a file, it will download an open AI model and perform the transcription locally in your browser. This means that your audio file never leaves your device. It also means that the transcription will be slow or fail if your computer/smartphone is not powerful enough to perform it.

In the settings, you can pick among different models and various quantisation levels. A smaller model with a lower quantisation will be faster but make more mistakes. By default, Whisper-web uses small models but you can try a bigger one and see if it works on your device.

In the app, the user can choose between the Swedish models, Norwegian ones (from the [Norwegian national library](https://huggingface.co/collections/NbAiLab/nb-whisper)) and OpenAI's models that are the best in all other languages.

This project's code is actually a fork of a demo created by Xenova that I updated and improved. Both are available on Github. Feel free to reuse or contribute to it.
