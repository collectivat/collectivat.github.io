---
layout: post
title: "Apreciar mi lengua materna y amplificar la voz de los comunes: mis prácticas en Col·lectivaT"
ref: practicashindi
thumbnail: /img/blog/2023/hindi.png
lang: es
summary: "Rahul Rahul explica su trabajo durante sus prácticas en Col·lectivaT"
---

_En esta publicación, **Rahul Rahul**, estudiante de Máster Universitario en Traducción y Tecnologías de la Universitat Oberta de Catalunya, describe sus tareas y aprendizajes durante las prácticas en Col·lectivaT en otoño de 2022. Por un lado, habla sobre el proceso de entrenamiento de un bote conversacional (un programa que simula una conversación con una interlocutora) en la lengua hindi y, por otra, explica cómo ha trabajado en traducción de artículos sobre bienes comunes. Publicamos el texto en su idioma original._

<p align="center"><img src="/img/blog/2023/hindi.png" alt="Un libro escrito en Amazig" width="80%"></p>

During my internship, I had the opportunity to work on two exciting projects that allowed me to hone my skills and gain valuable experience. The first project focused on improving the input data for a voice activated chatbot. I was responsible for conducting research, analysing data and making recommendations to improve the accuracy and effectiveness of the chatbot's responses. The second project was a linguistic task where I was tasked with translating articles about commons from Catalan to English using a CAT tool new to me. This internship was a great opportunity for me to not only improve my language skills, but also to make a positive impact on the world by helping the organisation spread their message to a wider audience. Overall, these two projects gave me a well-rounded experience in both technical and language-related tasks, and I am grateful for the opportunity to have worked on them.

<p style="text-align: center;">
<span style="font-weight:700;font-size:25px">
    <i>"This internship was a great opportunity for me to not only improve my language skills, but also to make a positive impact on the world by helping the organisation spread their message to a wider audience."</i>
</span>
</p>

## Teaching my mother tongue to a chatbot

The chatbot project involved assisting my tutor Alp Öktem in creating a voice-based chatbot by reviewing, editing, and translating phrases from English to Hindi. This project is an initiative by [CLEAR Global](https://clearglobal.org/) and involves placing voice-based information kiosks called TILES in low-connectivity regions of Bihar, India. Hindi is a widely spoken language in India and is the fourth most spoken language in the world, with over 615 million speakers globally. As my mother tongue, Hindi holds a special place in my heart, but it had been over 10 years since I had written in it. I had to "relearn" a few things and sought help from friends and family who lived in India when I needed assistance with specific terminology or cultural references. The process of working on the project allowed me to reconnect with my language and culture, and I am grateful for the opportunity to deepen my understanding and appreciation of Hindi.


### Data revision and testing

This section covers the corrections I made to the training data and the testing process of the chatbot. The chatbot I worked on was adapted from a text-based chatbot which informed about COVID-19 in northeastern Nigeria. The training and response data, which reflects the Nigerian context, needed to be updated to reflect Indian context, proper use of gender, and correct translation of verbs in Hindi. As an example of cultural translation, I proposed to place the influential yogi Ramdev Baba instead of Dr. Abdul as a prominent figure in alternative medicine in the following training data point: 


**Question**

_Can Ramdev Baba's medicine cure Covid?_

_क्या रामदेव बाबा की दवा से कोविड ठीक हो सकता है?_

**Answer**

_There is no specific cure for COVID-19 — only vaccines to prevent infection — but scientists around the world are running trials on antiviral and other medications as potential treatments, NCDC says._

_COVID-19 के लिए कोई विशिष्ट इलाज नहीं है-केवल संक्रमण को रोकने के लिए टीके-लेकिन दुनिया भर के वैज्ञानिक एंटीवायरल और अन्य दवाओं पर संभावित उपचार के रूप में परीक्षण चला रहे हैं, एनसीडीसी कहते हैं।_

I revised and corrected the data for grammatical errors and proper technical terms. I also tested if the speech recognition module was able to understand acronyms and commonly used terms such as BP (Blood Pressure) and Sugar (Diabetes).

During the testing process, the chatbot was tested for its ability to recognize intents and phrases in Hindi. My tutor Alp created a spreadsheet with the intents, English phrases, and translated Hindi phrases. The testing involved saying the phrases in Hindi and checking if the program recognized them. In case of positive results, the intent was marked as correct, and in case of negative results, the ASR result and intent detected were noted.

| Intent                   | English                                            | Hindi                                  | ASR result                | Detected | Comments                                                   |
|--------------------------|----------------------------------------------------|----------------------------------------|------------------------|-----------------|------------------------------------------------------------|
| how_spread               | How will I catch coronavirus?                      | मैं कोरोनवायरस को कैसे पकड़ूंगा?              | मैं कोरोना वायरस कैसे करूंगा | <span style="color: green;">how_spread</span>      | It detected “corona”, “virus” and “how”                    |
| protection_wash_ distance | Does washing your hands protect against infection? | क्या आपके हाथ धोने से संक्रमण से बचाव होता है? | हाथ धोने से कोविद        | <span style="color: red;">symptoms</span> | It detected hand, wash and covid but didn't get the intent |

<br>

During testing, we encountered several common errors, including the ASR's difficulty in detecting the auxiliary verb "है'' in Hindi and its variations, poor ability to detect fast speech, and incorrect detection of intent. We also observed that the ASR had trouble detecting the verb "can'' and often misidentified it as "need". However, the ASR was able to easily recognize certain keywords, such as "breastfeeding" and "child". 

Overall, the testing process highlighted the need for further improvements to the training data to enhance the chatbot's accuracy.


### Materials used 

I used several online resources for my project. The main website that I used was [Easy Hindi Typing](https://www.easyhindityping.com/). This website was instrumental in my project as it facilitated my ability to type in Hindi, a language with which I am unfamiliar when it comes to typing. Typing in Hindi using an English keyboard can be challenging, but this website made it easier.

I also found [SHABDKOSH](https://www.shabdkosh.com/) to be useful. This website acted as an online dictionary and was helpful in finding the correct spelling and meaning of various words.

Furthermore, I used the COVID-19 Glossary provided by [Translators without Borders](https://glossaries.clearglobal.org/covid19/). This glossary was particularly useful in providing technical terms and industry-specific jargon related to the pandemic.

In addition to these online resources, I also consulted my friends and family to gather specific terminology and cultural references. For example, I asked them about myths and misconceptions about COVID-19 that were prevalent in the community. These additional sources helped me to add a cultural aspect to my project, giving it a more rounded approach.


## Translating Commons with MateCAT

During the second part of my internship with Col·lectivaT, I had the opportunity to work with their translator Pelin Doğan, who introduced me to Computer-aided translation (CAT) tools and other subtitling software like SubtitleEdit. However, our main focus was on translating texts using MateCat, which is a user-friendly open-source CAT tool.

After an introduction to MateCat, I assisted Pelin with the translations for a project from a cooperative called [femProcomuns](https://femprocomuns.coop/). I was responsible for translating only some parts of an academic text and two other articles, all of which were from Catalan to English. Then, Pelin reviewed my work and helped me understand my errors, and discuss any terminology questions. She also provided me with useful websites and dictionaries so that I could independently work on the articles.

The first text that I helped translate was an extensive academic text about the Commons. The concept of Commons refers to shared resources that are managed and maintained by a community. These resources can be tangible, such as land, water, or forests, or intangible, such as cultural or knowledge resources. I also worked on the translation of two articles. The academic text served as an introduction to the topic of the Commons and helped me make correct choices when selecting terminology around and about the commons, as well as an introduction to all the translation processes.

### My experience with CAT tools

Computer-aided translation (CAT) tools are invaluable resources for the modern translator. They help streamline the translation process and make it more efficient and accurate. Under this section, I will compare two of the CAT tools: MateCat and Trados, one that I got familiarised with during the internship and one that I had already used, respectively.

MateCat is an easy-to-use open-source CAT tool, under the Lesser General Public License (LGPL), with a range of advanced features. It is designed for professional translators and is also suitable for beginners. Key features include machine translation, term base support, full text search, and a customizable user interface.

MateCat is ideal for smaller projects. It can be used to translate reasonably small texts such as emails, website content, and legal documents. It allows users to create multiple translation memories and store glossaries, making it easier to manage translations over time.

In contrast to MateCat, Trados has a restricted commercial licence, and is designed for more complex projects and is better suited for larger translation jobs. It comes with a range of powerful features, including full-text alignment, which allows users to ensure that the translated text is an exact match of the source text. It also offers built-in terminology management and project management tools, making it easier to manage large-scale translations.
Overall, both MateCat and Trados offer advantages and disadvantages, and it is up to the user to decide which is best for their specific needs. For simple projects, MateCat is usually a better option due to its user-friendly interface and comprehensive features. For more complex projects, Trados is often the go-to tool due to its powerful features and robust project management tools. Having used both I must say that learning the basics of MateCat was a much simpler task than Trados’.

Working with Pelin and using MateCat was an excellent experience that allowed me to develop my translation skills and gain experience in working with a professional translation tool. The opportunity to work on a project for a non-profit cooperative that is dedicated to promoting the Commons and supporting community-based initiatives was truly rewarding.

## Reflections

My internship at Col·lectivaT was a fantastic experience that gave me valuable insights into the translation and language technology industry. I had the opportunity to work with a dynamic and inspiring team and gain exposure to translation in various contexts. Most importantly, my internship helped me realise the importance of working with my mother tongue, Hindi. It was an incredibly empowering experience to be able to contribute to the translation of Hindi texts, and I am excited to continue exploring this field further. I am grateful for this opportunity and excited to continue exploring this field further.


_Rahul Rahul_

---

_Si vols col.laborar amb Col.lectivaT o vols fer pràctiques aquí, escriu-nos a [info@collectivat.cat](mailto:info@collectivat.cat)._