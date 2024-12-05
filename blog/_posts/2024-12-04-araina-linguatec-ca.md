---
layout: post
title: "El projecte Araina agafa impuls"
ref: araina2024
thumbnail: /img/blog/2024/linguatec.png
lang: ca
summary: "Aquesta tardor hem tornat a donar impuls al projecte Araina per promoure que les noves tecnologies parlin i entenguin l’aranès."
---

<br>

<p align="center"><img src="/img/blog/2024/linguatec.png" width="80%" ></p>

<!--

<iframe src="/player/localplayer.html?file=https://storage.googleapis.com/ttsreader/nou.collectivat.cat-2024-07-10-obrim-el-collectivat-tech-lab-.mp3&title=Escolta aquest article amb enVeu" type="text/html" width="100%" height="80px" frameborder="0" allowfullscreen></iframe> 

-->

<br>

Aquesta tardor hem tornat a donar impuls al <a href="https://www.projecte-araina.org/ca/" target="_blank" rel="noopener noreferrer">projecte Araina</a> per promoure que les noves tecnologies parlin i entenguin l’aranès. Des de Col·lectivaT, en col·laboració amb el Grup de Recerca en Sociolingüística i Geolingüística (SoGel) de la Universitat de Lleida i Lo Congrès Permanent de la Lenga Occitana, hem posat en marxa una recollida de dades de veu en entorns professionals d'enregistrament, optimitzada per a la creació de models de síntesi de veu (text-to-speech). Aquest procés requereix enregistraments d'alta qualitat en estudis equipats amb condicions òptimes de so.

La nova fase d’Araina forma part de POCTEFA Linguatec-IA, un projecte europeu més ampli que treballa per la digitalització de les llengües pirinenques minoritzades. Liderat per <a href="https://www.elhuyar.eus/ca" target="_blank" rel="noopener noreferrer">Elhuyar</a> i amb la participació d'institucions acadèmiques i culturals de tot el Pirineu, LinguaTec-IA s'ha aliat amb Araina, la primera iniciativa per desenvolupar tecnologies de veu en aranès que al 2022 va començar a recollir dades de veu a través de la plataforma Common Voice amb la col·laboració de Mozilla. Amb aquesta embranzida, volem avançar cap a la creació de tecnologies de síntesi de veu, la possibilitat de digitalitzar la llengua i la consolidació d’unes bases sòlides per a futures aplicacions interactives.

En aquest article expliquem tot el procés tècnic d'aquesta nova fase: la preparació del corpus de text a partir de materials històrics, els protocols dels enregistraments professionals, i la metodologia que seguim per garantir la qualitat necessària per entrenar els models de síntesi de veu.

### Cap a un corpus de veu robust i divers en aranès

Si bé a l’anterior fase del projecte vam organitzar una Marató de veus a Vielha oberta a la població per a recollir un gran gruix de dades, en aquesta ens hem proposat treballar amb un perfil concret de públic per continuar augmentant en quantitat i qualitat les dades de veu en aranès.

El primer pas per a dur a terme els enregistraments ha estat preparar el corpus de text, és a dir, un conjunt de fragments escrits perquè les locutores els puguin anar llegint en veu alta. Per ampliar el corpus de veu del que partíem, hem utilitzat materials històrics de la <a href="https://ddd.uab.cat/collection/honsaran" target="_blank" rel="noopener noreferrer">Premsa Aranesa</a> (UAB) des de 1921 fins l'actualitat, i hem revisat sistemàticament més de 500 entrades del catàleg, identificant documents amb contingut en aranès, fixant-nos en la qualitat i el format del text i l’adequació per al corpus segons el gènere (articles periodístics o informatius, poesia, teatre, etc.). Aquest treball manual ens ha permès crear una base de dades organitzada amb els millors textos per alimentar el corpus.

<a href="https://www.projecte-araina.org/ca/" target="_blank"><img align="left" src="/img/blog/2024/araina-cases-logo.png" alt="Projecte Araina" width="35%" style="margin: 0 20px 0px 0px"></a>Per obtenir els textos, hem desenvolupat un sistema automatitzat innovador amb diverses característiques: pot extreure el text dels documents PDF digitalitzats, fer reconeixement òptic de caràcters (OCR) en imatges, corregir errors ortogràfics i de format utilitzant models de llenguatge i segmentar i seleccionar frases adequades per a gravacions. Alineades amb els valors de Col·lectivaT de fer el coneixement accessible i col·laboratiu, el sistema està creat amb codi obert i el trobareu <a href="https://github.com/CollectivaT-dev/aranese-text-corpus/" target="_blank" rel="noopener noreferrer">disponible a GitHub</a>, aplicable per a altres llengües minoritzades. La informació recollida la publicarem al repositori de <a href="https://huggingface.co/datasets/collectivat/araina-text-corpus" target="_blank" rel="noopener noreferrer">HuggingFace</a>.

Gràcies a aquesta feina, hem generat 10.000 frases optimitzades per a les gravacions de veu, tot assegurant la diversitat de sons de la llengua amb el mecanisme de transcripció fonètica de Lo Congrès. També hem preservat la diversitat d’expressions, incloent des del llenguatge quotidià fins a expressions comunes per interfícies d'usuari. I finalment, hem inclòs noms propis en català i castellà per assegurar que el model aprengui a pronunciar correctament els noms més comuns en el context local.

Per a les sessions de gravació professional, hem comptat amb quatre locutores natives de la Val d’Aran als estudis de GumFM a Vielha i Koala Studios a Barcelona, seguint protocols estrictes de qualitat d’àudio. Amb elles hem aconseguit sumar 10 hores de gravacions d'alta qualitat amb múltiples veus per crear un sistema de síntesi de veu (TTS), un tipus de tecnologia que permet convertir text escrit en parla natural.

Com a equip tècnic, des de Col·lectivaT hem dut a terme diverses tasques com supervisar les sessions, documentar correccions i variants proposades per les locutores, verificar la qualitat tècnica del so, assegurar-nos que cada frase es llegís amb la prosòdia adequada, mantenir un registre detallat de les sessions per al processament posterior.

### Les properes passes perquè la tecnologia parli i entengui l’aranès

<img align="right" src="/img/blog/2024/Assistent-veu_1.png" alt="Assistent de veu en aranes" width="35%">Durant el 2025, continuarem recollint dades de veu a través de la plataforma Common Voice, combinant la participació voluntària amb col·laboracions remunerades per assegurar la diversitat de veus i variants. També ens proposem organitzar sessions controlades de gravació amb participants seleccionades, buscant un equilibri en gènere, edat i variant dialectal, i processar els materials existents amb transcripcions per enriquir el corpus. L'objectiu és aconseguir un mínim de 50 hores de gravacions en total per poder desenvolupar models de reconeixement automàtic de veu (ASR). En aquest procés, tot el material generat alimentarà el desenvolupament de models de veu en aranès dins del projecte LinguaTec-IA, establint les bases per futures aplicacions interactives en aquesta llengua.

Des de la nostra perspectiva, aquest projecte obre noves possibilitats per a l'aranès en l'era digital. Algunes poden ser aplicacions educatives interactives amb veu natural en aranès, assistents virtuals, eines d'accessibilitat per a persones amb dificultats de lectura, sistemes de navegació i transport públic en aranès, etc.

Com vam explorar a l’<a href="https://collectivat.cat/blog/2024-10-15-llm-demo-ca/" target="_blank" rel="noopener noreferrer">article sobre els Grans Models de Llenguatge</a>, aquestes tecnologies poden transformar l'aprenentatge de les llengües minoritzades. Un company virtual que parli aranès natural pot oferir un espai segur per a practicar la llengua, especialment per a les joves que tenen una exposició limitada a l'aranès fora de l'escola.


<p align="center"><img src="/img/blog/2024/Logo LINGUATEC-IA.png" width="50%" >