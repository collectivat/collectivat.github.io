---
layout: post
title: "The Araina Project Gains Momentum"
ref: araina2024
thumbnail: /img/blog/2024/linguatec.png
lang: en
summary: "This autumn, we’ve reignited the Araina project that aims new technologies speak and understand Aranese."
---

<br>

<p align="center"><img src="/img/blog/2024/linguatec.png" width="80%"></p>

<br>

This autumn, we’ve reignited the [Araina Project](https://www.projecte-araina.org/en/) to promote the integration of Aranese into emerging technologies. Together with the Sociolinguistics and Geolinguistics Research Group (SoGel) at the University of Lleida and Lo Congrès Permanent de la Lenga Occitana, Col·lectivaT has initiated high-quality voice data collection in professional recording environments, optimized for developing text-to-speech (TTS) models. This process requires recordings captured in acoustically controlled studios.

This new phase of Araina is part of POCTEFA Linguatec-IA, a broader European initiative focused on digitizing minoritized languages of the Pyrenees. Led by [Elhuyar](https://www.elhuyar.eus/en) and involving academic and cultural institutions across the region, Linguatec-IA has partnered with Araina to advance the first voice technology solutions in Aranese. The project began in 2022 with a voice data collection effort through Mozilla’s Common Voice platform. Now, we’re building on this foundation to develop TTS systems, digitize the language, and lay the groundwork for future interactive applications.

In this article, we outline the technical process of this new phase: preparing the text corpus using historical materials, professional recording protocols, and the methodologies we’re applying to ensure the quality needed for training voice synthesis models.

### Building a robust and diverse speech corpus for Aranese

In the project’s earlier phase, we organized a Voice Marathon in Aran Valley, inviting the public to contribute large volumes of voice data. This time, we’re focusing on a specific participant profile to further enhance the quality and quantity of the Aranese voice corpus.

The first step involved preparing the text corpus—a collection of written fragments for speakers to read aloud. To expand our starting point, we utilized historical materials from the [Aranese Press Archive](https://ddd.uab.cat/collection/honsaran) (UAB), spanning from 1921 to the present. Over 500 catalog entries were systematically reviewed to identify documents in Aranese, ensuring the quality and relevance of texts based on genre (news articles, poetry, theater, etc.). This manual effort resulted in a curated database of texts ideal for building the corpus.

<a href="https://www.projecte-araina.org/en/" target="_blank"><img align="left" src="/img/blog/2024/araina-cases-logo.png" alt="Projecte Araina" width="35%" style="margin: 0 20px 0px 0px"></a>We developed an innovative automated system to process these texts, equipped with features such as extracting text from digitized PDFs, performing optical character recognition (OCR) on scanned images, correcting formatting and spelling errors with language models, and segmenting sentences suitable for recordings. 

Staying true to Col·lectivaT’s values of accessibility and collaboration, this system was built with open-source tools and is [available on GitHub](https://github.com/CollectivaT-dev/aranese-text-corpus/), adaptable for other minoritized languages. The processed data will be published in the [HuggingFace repository](https://huggingface.co/datasets/collectivat/araina-text-corpus).

Through this work, we’ve generated 10,000 optimized phrases for voice recordings, ensuring phonetic diversity with the phonetic transcription system from Lo Congrès. The corpus also reflects a variety of linguistic expressions, from everyday language to user-interface commands, and includes proper names in Catalan and Spanish for local context accuracy.

For professional recording sessions, we collaborated with four native speakers from the Aran Valley. Sessions were held at GumFM Studios in Vielha and Koala Studios in Barcelona under strict audio quality protocols. These efforts will yield 10 hours of high-quality voice recordings, featuring multiple speakers, to train a natural-sounding and multispeaker TTS system.

As the technical team, Col·lectivaT oversaw the sessions, documented proposed corrections and variations, verified sound quality, ensured proper prosody, and maintained detailed logs for post-processing.

### Next steps to make technology speak and understand Aranese

<img align="right" src="/img/blog/2024/Assistent-veu_1.png" alt="Aranese voice assistant" width="35%">In 2025, we plan to continue collecting voice data via the Common Voice platform, blending voluntary contributions with paid collaborations to ensure a diverse range of voices and dialectal variations. We also aim to organize controlled recording sessions with selected participants, balancing factors such as gender, age, and dialect, while processing existing materials with transcriptions to enrich the corpus. Our target is to gather at least 50 hours of recordings to develop automatic speech recognition (ASR) models.

The data generated through this process will feed into the development of Aranese voice technologies within the Linguatec-IA project, laying the groundwork for future interactive applications in the language.

This project opens up exciting possibilities for Aranese in the digital age, including educational tools with natural voice interfaces, virtual assistants, accessibility tools for individuals with reading challenges, public transit systems in Aranese, and more.

As we explored in our [article on Large Language Models](https://collectivat.cat/blog/2024-10-15-llm-demo-en/), these technologies could revolutionize the learning of minoritized languages. A virtual companion fluent in natural Aranese could provide a safe and engaging space to practice the language, especially for the youth with limited exposure outside the classroom.

<p align="center"><img src="/img/blog/2024/Logo LINGUATEC-IA.png" width="50%"></p>