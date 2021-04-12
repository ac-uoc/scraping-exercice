# Ejercicio de scraping
Autores: Antonio Nogueras y Alejandro Casanovas

Scraping de un agregador de noticias

Práctica PRA1 ejercicio de scraping de la asignatura M2.951 de ciencia de datos.

El objetivo del scraping es analizar las relaciones entre parámetros que aparecen en un agregador como el número de comentarios, los votos positivos o votos negativos.

Nos hemos centrado en un agregador, meneame.net, que proporciona un parámetro que califica al usuario que aporta la noticia, que denominan karma, junto con otros como "meneos", votos positivos, negativos y anónimos, clics, una variable cualitativa que clasifica el tema, el usuario que aporta la noticia o la fecha de aportación, entre otros.

Concretamente queremos comprobar si existe alguna relación entre el karma y los otros parámetros, por ejemplo, si más karma supone más clics o más votos positivos.
El karma es como un carnet de puntos: el karma inicial de un usuario nuevo es bajo, y puede subir (o bajar) en función del éxito de las aportaciones.

La dificultad de analizar un agregador es que es un mundo cambiante: clics, noticias, votos, meneos, ... cambian constantemente, así que conviene tomar una instantánea lo más amplia posible, ya que en diferentes tiempos compararemos cosas diferentes. Especialmente cabe evitar noticias duplicadas: en la cola de entrada ('nuevas' en meneame.net) estos duplicados son frecuentes y se insiste en la misma noticia.

Hemos trabajado en Jupyter de Anaconda3 y Python con las librerías específicas request y Beautiful Soup.
Lo que se adjunta es el fichero .ipynb y los ficheros de salida, en csv, por ejemplo.

Ejecutando el .ipynb se puede leer directamente el dataframe que se obtiene de escanear unos 250 noticias únicas y el análisis de gráficas y resultados que realizamos.
Nos hemos limitado a esa cantidad para no cargar la web con una lectura sucesiva de muchas páginas; esto es solo un ejercicio de scraping.

Concluimos, entre otras cosas, que el valor de karma de las noticias del hilo principal no parece depender de los otros parámetros, ya que debe ser obtenido probablemente por un periodo extraordinariamente largo de aportaciones; el karma promedio de estos aportadores puede estar en un valor de 350.

Hay una versión 2: meneame_scrapingV2.ipynb para el caso de que de fallos en Windows 10.  Produce además un fichero Excel de los datos.

# Exercici de scraping 

# Autors: Antonio Nogueras i Alexandre Casanovas

Scraping d'un agregador de notícies

Pràctica PRA1: exercici de scraping de l'assignatura M2.951 de ciència de dades.

L'objectiu del scraping és analitzar les relacions entre paràmetres que apareixen en un agregador com el nombre de comentaris, els vots positius o vots negatius.

Ens hem centrat en un agregador, meneame.net, que proporciona un paràmetre que qualifica a l'usuari que aporta la notícia, que denominen karma, juntament amb uns altres com "meneos", vots positius, negatius i anònims, clics, una variable qualitativa que classifica el tema, l'usuari que aporta la notícia o la data d'aportació, entre altres.

Concretament volem comprovar si existeix alguna relació entre el karma i els altres paràmetres, per exemple, si més karma suposa més clics o més vots positius.
El karma és com un carnet de punts: el karma inicial d'un usuari nou és baix, i pot pujar (o baixar) en funció de l'èxit de les aportacions.

La dificultat d'analitzar un agregador és que és un món canviant: clics, notícies, vots, meneos, ... canvien constantment, així que convé prendre una instantània el més àmplia possible, ja que en diferents temps compararem coses diferents. Especialment cal evitar notícies duplicades: en la cua d'entrada ('noves' en meneame.net) aquests duplicats són freqüents i s'insisteix en la mateixa notícia.

Hem treballat en Jupyter de Anaconda3 i Python amb les llibreries específiques request i Beautiful Soup.
El que s'adjunta és el fitxer .ipynb i els fitxers d'eixida, en csv, per exemple.

Executant el .ipynb es pot llegir directament el dataframe que s'obté d'escanejar uns 250 notícies úniques i l'anàlisi de gràfiques i resultats que realitzem.
Ens hem limitat a aqueixa quantitat per a no carregar la web amb una lectura successiva de moltes pàgines; això és només un exercici de scraping.

Concloem, entre altres coses, que el valor de karma de les notícies del fil principal no sembla dependre dels altres paràmetres, ja que ha de ser obtingut probablement per un període extraordinàriament llarg d'aportacions; el karma mitjà d'aquests aportadors pot estar en un valor de 350.

Hi ha una versió 2: meneame_scrapingV2.ipynb per al cas de fallades en Windows 10. Produeix a més un fitxer Excel de les dades.

# Scraping exercise

# Authors: Antonio Nogueras and Alexandre Casanovas

Scraping of a news aggregator

Practice PRA1: scraping exercise of the data science course M2.951.

The goal of this scraping exercise is to analyze the relationships between parameters that appear in an aggregator such as the number of comments, up-votes or down-votes.

We have focused on an aggregator, meneame.net, which provides a parameter that qualifies the user who contributes the news, which they call karma, along with others such as "meneos", positive, negative and anonymous votes, clicks, a qualitative variable that classifies the topic, the user who contributes the news or the date of contribution, among others.

Specifically, we want to check if there is any relationship between the karma- and the other parameters, for example, if more karma means more clicks or more votes that are positive. Karma is like the points of a driver's license: the initial karma of a new user is low, and can go up (or down) depending on the success of the contributions.

The difficulty of analyzing an aggregator is that it is an ever-changing world: clicks, news, votes, ‘meneos’, ... change constantly, so it is convenient to take as broad a snapshot as possible, since at different times we will be comparing different things. It is especially important to avoid duplicate news: in the input queue (http://meneame.net/queue) these duplicates are frequent.

We have worked in Jupyter of Anaconda3 and Python with the specific libraries ‘request’ and ‘Beautiful Soup’.
Attached are the .ipynb- and output files, for example, in csv format.

By running the .ipynb you can directly read the dataFrame obtained from scanning about 250 unique news items and the analysis of graphs and results we perform.
We have limited ourselves to that amount in order to avoid overload the web with a successive reading of many pages; this is just a scraping exercise.

We conclude, among other aspects, that the karma value of the main news thread does not seem to depend on the other parameters, as it is probably obtained by contributions along an extraordinarily long time period; the average karma of these contributors of the main thread may be at a value of 350.

There is a version 2: meneame_scrapingV2.ipynb in case of Windows 10 failures. It also produces an Excel file of the data.
