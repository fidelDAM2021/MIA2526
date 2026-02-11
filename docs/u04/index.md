# Processament del llenguatge natural

El **Processament del Llenguatge Natural (PLN)** és una branca de la intel·ligència artificial que se centra en la interacció entre els ordinadors i el llenguatge humà. L'objectiu principal del PLN és permetre als ordinadors comprendre, interpretar i generar llenguatge natural de manera que siga útil per als humans.

## Introducció al Processament del Llenguatge Natural (PLN)

El camp del PLN combina coneixements de lingüística, informàtica i intel·ligència artificial per desenvolupar algoritmes i models que puguen processar textos i discursos humans. Això inclou tasques com l'anàlisi sintàctica, la comprensió semàntica, la traducció automàtica, la generació de text i el reconeixement de veu.

Per què una màquina puga processar llenguatge, caldrà aplicar l'estudi de diverses àrees, com ara:

- **Morfologia**: estudi de la formació de les paraules i de la información continguda en elles.
- **Sintaxi**: estudi de l'estructura de les frases i de les regles que governen la combinació de paraules per a formar oracions coherents.
- **Semàntica**: estudi del significat de les paraules i de les oracions.
- **Pragmàtica**: estudi de l'ús del llenguatge en contextos específics i de com el significat pot variar segons la situació.

## Aplicacions principals del PLN

El PLN té una àmplia gamma d'aplicacions pràctiques, entre les quals destaquen:

- reconeixement de veu i assistents virtuals (com Siri, Alexa, Google Assistant).
- anàlisi de sentiments (entendre les opinions i fins i tot les emocions expressades en textos).
- traducció automàtica (com Google Translate).
- classificació de textos (com filtres de correu brossa).
- creació de xatbots i sistemes de resposta automàtica en temps real.
- resum automàtic de documents.
- detecció i classificació d'entitats en un text (com noms de persones, llocs, organitzacions).

## Evolució

Els primers intents de fer PLN se remonten a 1954. Seguint la línia del conegut **Test de Turing** (que avaluava si una màquina podia comportar-se com un humà), se va portar a terme el **Test de Georgetown**. Com a resultat, se va aconseguir traduir un text del rus a l'anglès sense errors. Aquest èxit inicial va generar un gran optimisme sobre les possibilitats del PLN. No obstant això, els intents posteriors van revelar la complexitat inherent del llenguatge humà, incloent-hi ambigüitats, contextos culturals i variacions dialectals.

Les limitacions del hardware van fer que, com altres parts de la IA, el PLN no continuara desenvolupant-se fins als anys 1980. L'evolució posterior del PLN va estar impulsat per l'augment de la potència de càlcul, i per la disponibilitat de grans volums de dades textuals ("corpus") que permetien entrenar els models. 

Actualment el camp ha experimentat un salt qualitatiu gràcies a la integració de models de llenguatge avançats i profunds, com GPT o BERT, que utilitzen arquitectures de xarxes neuronals (transformers) per aconseguir una precisió sense precedents en la comprensió del llenguatge.

## Models de PLN

Els models de PLN són algorismes i estructures matemàtiques dissenyades per processar i analitzar el llenguatge natural. Estos models poden variar des de simples regles basades en gramàtica fins a complexos sistemes d'aprenentatge automàtic i xarxes neuronals profundes. Alguns dels models més comuns inclouen:

- **Models basats en regles**: Utilitzen un conjunt de regles lingüístiques per analitzar i generar llenguatge. Són útils per a tasques específiques però tenen limitacions en la gestió de la variabilitat del llenguatge.
- **Models estadístics**: Utilitzen tècniques estadístiques per identificar patrons en grans conjunts de dades textuals. Estos models poden aprendre a partir de l'experiència i millorar amb el temps.
- **Models d'aprenentatge profund**: Utilitzen xarxes neuronals profundes per capturar les complexitats del llenguatge. Estos models, com els transformers, han demostrat ser extremadament efectius en una àmplia gamma de tasques de PLN.

Models preentrenats com **GPT (Generative Pre-trained Transformer)**, **BERT (Bidirectional Encoder Representations from Transformers)** i **T5 (Text-to-Text Transfer Transformer)** han revolucionat el camp del PLN, permetent aplicacions avançades com la generació de text coherent, la traducció automàtica i la comprensió contextual.

Els **models fundacionals** són una nova categoria de models de PLN que combinen la potència dels models preentrenats amb la flexibilitat per adaptar-se a tasques específiques. Aquests models permeten als usuaris personalitzar i ajustar els models segons les seves necessitats particulars, sense haver de començar des de zero. Vosaltres heu utilitzat en la pràctica que heu fet amb **AWS Bedrock** heu utilitzat alguns d'eixos models, i els heu anat ajustant modificant els seus paràmetres, afegint guardrails i entrenant-los amb dades específiques (les bases de coneixement) per a millorar el seu rendiment en tasques concretes.

## On podem trobar text per entrenar models de PLN?

Hi ha models que aprenen a partir de documents en format text, PDF, pàgines web, etc. Si voleu **corpus** grans de text, hi ha llocs on podeu trobar-los de forma gratuïta:

- **Projecte Gutenberg**: Una biblioteca digital de llibres de domini públic. (https://www.gutenberg.org/). Podeu trobar més informació a https://github.com/pgcorpus/gutenberg
- **Common Crawl**: Un arxiu massiu de dades web que conté pàgines web rastrejades des de fa anys. (https://commoncrawl.org/)
- **Wikipedia**: La base de dades de Wikipedia està disponible per a la descàrrega i pot ser utilitzada com a corpus de text. (https://dumps.wikimedia.org/)

Hi ha molts altres llocs. En castellà i català, per exemple, teniu:

- https://clic.ub.edu/corpus/ 
- https://www.corpusdelespanol.org/
- https://github.com/roquegv/spanishNLPModelCorpus

## Eines i biblioteques per al PLN

Hi ha moltes eines i biblioteques disponibles per al desenvolupament de projectes de PLN. Algunes de les més populars inclouen:

- **NLTK (Natural Language Toolkit)**: Una biblioteca de Python molt popular i senzilla que proporciona eines per al processament del llenguatge natural, incloent-hi tokenització, etiquetatge gramatical, eliminació de paraules de parada, anàlisi de sentiments, etc. (https://www.nltk.org/)
- **WordNet**: Un gran diccionari de sinònims i relacions semàntiques entre paraules, que es pot utilitzar per a tasques com la desambiguació de paraules i l'anàlisi semàntica. Sembla que només està en anglès, però hi ha alternatives per altres idiomes. (https://wordnet.princeton.edu/)
- **spaCy**: Una biblioteca de Python dissenyada per a l'ús en producció, amb un enfocament en la velocitat i l'eficiència. Destaca en la detecció de NERs (entitats nomenades) (https://spacy.io/)
- **TextBlob**: Una biblioteca de Python que facilita el processament del llenguatge natural amb una API senzilla per a tasques com l'anàlisi de sentiments, la traducció i la correcció ortogràfica. (https://textblob.readthedocs.io/en/dev/)
- **Transformers de Hugging Face**: Una biblioteca que proporciona accés a models preentrenats com BERT, GPT-2 i altres. (https://huggingface.co/transformers/)
- **Stanford NLP**: Un conjunt d'eines desenvolupades per la Universitat de Stanford per al processament del llenguatge natural. (https://stanfordnlp.github.io/CoreNLP/)

**Eines per a reconeixement de veu i síntesi de veu**:

- **SpeechRecognition**: Una biblioteca de Python que facilita la integració de reconeixement de veu en aplicacions. (https://pypi.org/project/SpeechRecognition/)
- **gTTS (Google Text-to-Speech)**: Una biblioteca que permet convertir text en veu utilitzant l'API de Google Text-to-Speech. (https://pypi.org/project/gTTS/)
- **PyAudio**: Una biblioteca que permet la reproducció i gravació d'àudio en Python. (https://people.csail.mit.edu/hubert/pyaudio/)
- **pyttsx3**: Una biblioteca de síntesi de veu (text a audio) que funciona fora de línia. (https://pypi.org/project/pyttsx3/)
- **NeMo de NVIDIA**: Una biblioteca per a la creació i entrenament de models de reconeixement de veu i síntesi de veu. És molt potent i està optimitzada per a GPUs (https://developer.nvidia.com/nemo)

Hi ha moltes altres eines i biblioteques que faciliten el desenvolupament de projectes de PLN i permeten als desenvolupadors implementar solucions avançades de processament del llenguatge natural amb relativa facilitat. Algunes estan especialitzades en reconeixement de veu (o síntesi de text a veu), traducció automàtica, comparació de textos, anàlisi de sentiments, detecció de NERs, etc. Bàsicament es tracta de definir el problema que volem resoldre, i veure quines eines i biblioteques són les més adequades per a la tasca concreta que volem dur a terme.

**Models existents**:

- **GPT (Generative Pre-trained Transformer)**: Desenvolupat per OpenAI, és un model de llenguatge avançat capaç de generar text coherent i realitzar diverses tasques de PLN.
- **BERT (Bidirectional Encoder Representations from Transformers)**: Desenvolupat per Google, és un model que excel·leix en la comprensió del context i les relacions entre paraules en un text.
- **MEGATRON**: Desenvolupat per NVIDIA, és un model de llenguatge massiu dissenyat per a tasques avançades de PLN i generació de text.

En principi treballarem principalment amb **NLTK** i **spaCy**, ja que són les més senzilles d'utilitzar i les que tenen més documentació i exemples disponibles. Si podem, també farem servir alguna de les eines de **Hugging Face** per a treballar amb models preentrenats. I si encara podem més, mirarem si podem utilitzar **NeMo**, la biblioteca de NVIDIA per a treballar amb models de PLN i de reconeixement de veu.

## Alguns conceptes bàsics en PLN

Abans de començar a veure com treballar en PLN, és important conèixer alguns conceptes bàsics que s'utilitzen habitualment en este camp:

- **Tokenització**: El procés de dividir un text en unitats més petites anomenades tokens (paraules, frases, etc.).
- **Lematització**: La reducció d'una paraula a la seua forma base o lema. Per exemple, "corrent", "corregut" i "corre" es redueixen al lema "córrer".
- **Stemming**: Similar a la lematització, però més agressiu, ja que redueix les paraules a la seua arrel, que pot no ser una paraula real. Per exemple, "corrent", "corregut" i "corre" es redueixen a "corr". També es coneix com ***derivació regressiva***
- **Vectorització**: El procés de convertir el text en una representació numèrica (vectors) que els models de PLN poden processar. Això es pot fer mitjançant tècniques com el bag of words, TF-IDF o embeddings de paraules. Alguns models que permeten vectoritzar el text són **Word2Vec**, **GloVe** i **FastText**.
- **Similitud de cosinus**: Una mesura de la similitud entre dos vectors que s'utilitza sovint en PLN per comparar la similitud entre textos o paraules. Torna un resultat entre -1 (totalment diferents) i 1 (idèntics).
- **Paraules de parada (stop words)**: Paraules comunes que sovint s'eliminen durant el processament del llenguatge, com "i", "el", "de", etc., ja que aporten poc significat al text.
- **N-grames (agregació sintagmàtica)**: Seqüències contigües de n elements (paraules o caràcters) en un text. Per exemple, els bigrames de la frase "El gat negre" serien "El gat" i "gat negre".
- **TTS**: Text to Speech, síntesi de veu a partir de text.
- **ASR**: Automatic Speech Recognition, reconeixement automàtic de veu.
- **NER**: Named Entity Recognition, reconeixement d'entitats nomenades (noms de persones, llocs, organitzacions, etc.) dins d'un text.
- **Transformers**: Arquitectura de xarxes neuronals utilitzada en models avançats de PLN, com BERT i GPT, que permeten una millor comprensió del context i les relacions entre paraules en un text. És la base principal dels models de llenguatge moderns.
- **LLM (Large Language Models)**: Models de llenguatge de gran escala que utilitzen arquitectures de transformers i són capaços de generar text coherent i realitzar diverses tasques de PLN amb alta precisió. Alguns exemples inclouen GPT-3, BERT i MEGATRON.
- **Fine-tuning**: Un concepte que se pot aplicar al PLN i a altres tipus de models. El procés d'ajustar un model preentrenat a una tasca concreta mitjançant l'entrenament amb un conjunt de dades específic per a aquesta tasca. Això permet al model adaptar-se millor a les necessitats particulars del problema que es vol resoldre.

## Preprocessament de text

El **preprocessament de text** és una etapa crucial en el processament del llenguatge natural, ja que permet preparar el text per a l'anàlisi i l'entrenament de models. Algunes de les tècniques més comunes de preprocessament ja les hem comentat en l'apartat anterior. En general s'utilitzen:

- **Normalització**: Convertir el text a una forma estàndard, com convertir totes les lletres a minúscules o eliminar signes de puntuació.
- **Tokenització**: Dividir el text en unitats més petites (tokens).
- **Lematització**: Reduir les paraules a la seua forma base o lema.
- **Stemming**: Reduir les paraules a la seua arrel.
- **Eliminació de paraules de parada**: Eliminar paraules comunes que aporten poc significat al text.
- **Gestió de negacions**: Identificar i gestionar les negacions en el text, ja que poden canviar significativament el significat d'una frase.

## Anàlisi de sentiments

L'**anàlisi de sentiments** és una tècnica de PLN que permet identificar i classificar les opinions i emocions expressades en un text. Esta tècnica és especialment útil per a empreses que volen entendre les opinions dels seus clients a través de ressenyes, comentaris en xarxes socials, etc. L'anàlisi de sentiments pot classificar els textos com a positius, negatius o neutres, i també pot identificar emocions específiques com la felicitat, la tristesa, la ira, etc.

Els mètodes principals utilitzats en l'anàlisi de sentiments inclouen:

- **Mètodes basats en regles**: Utilitzen un conjunt de regles lingüístiques per identificar les opinions i emocions en el text. En general se basen en llistes de paraules a les quals s'assigna una polaritat (positiva, negativa o neutra) i es compten les aparicions d'aquestes paraules en el text per determinar el sentiment general. També poden utilitzar regles gramaticals per identificar negacions o intensificadors que poden canviar el sentiment d'una frase.
- **Mètodes estadístics**: Utilitzen tècniques estadístiques per identificar patrons en grans conjunts de dades textuals i classificar els sentiments.
- **Mètodes d'aprenentatge automàtic supervisat**: Utilitzen algoritmes d'aprenentatge automàtic per entrenar models que puguen classificar els sentiments en funció de les característiques del text. El model s'ha d'entrenar amb un conjunt de dades etiquetades, on cada text té associada una etiqueta de sentiment (positiu, negatiu, neutre, etc.). Un cop entrenat, el model pot classificar nous textos en funció de les característiques que ha après durant l'entrenament.
- **Mètodes d'aprenentatge automàtic no supervisat**: Utilitzen tècniques d'aprenentatge automàtic per identificar patrons en grans conjunts de dades textuals sense necessitat d'etiquetes de sentiment. Estos mètodes poden utilitzar tècniques com el clustering o l'anàlisi de components principals per identificar grups de textos amb sentiments similars.
- **Mètodes d'aprenentatge profund**: Utilitzen xarxes neuronals profundes per capturar les complexitats del llenguatge i classificar els sentiments amb alta precisió.

Models com **BOW** (Bag of Words), **TF-IDF** (Term Frequency-Inverse Document Frequency), **Word Embeddings** (com Word2Vec, GloVe i FastText), **VADER** (per regles, en anglès) i **Transformers** com **BERT** estan entre els més utilitzats en l'anàlisi de sentiments. Alguns d'ells estan basats en regles, altres en estadístiques, altres en aprenentatge automàtic i altres en aprenentatge profund (xarxes neuronals). La tria del mètode adequat depèn de la complexitat de la tasca, la quantitat de dades disponibles i els recursos computacionals.

No cal que ens allarguem més en la part teòrica, anirem veient els concepts necessaris segons els anem necessitant en les pràctiques que farem. Ara anem a veure com treballar amb PLN utilitzant Python i algunes de les biblioteques més populars en este camp i aplicant-les a tasques concretes.