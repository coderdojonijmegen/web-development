Onderdelen van een HTML-pagina (basis)
######################################

Structuur van een pagina
************************
Websites worden geschreven in de taal van het internet: HTML. Er zijn veel
verschillende "woorden", of "bouwblokken", in HTML. Een aantal van de meest
gebruikte leer je hier kennen.

Een HTML-pagina heeft een paar standaard onderdelen:

.. code:: HTML

  <!DOCTYPE html>
  <html>
  <head>
  </head>
  <body>
    <h1>Dit is een kop</h1>
    <p>Dit is een alinea.</p>
  </body>
  </html>


* HTML onderdelen worden aangegeven met *tags*: de naam van
  het onderdeel tussen ``<>`` haakjes.
* De meeste onderdelen hebben een *start* en een *eind* tag.
* De eind tag heeft een *forward slash* dus ``/`` voor de naam,
  bijvoorbeeld ``</html>``.
* Tags worden altijd geschreven met *kleine letters*.


**Opdracht** Kopieer en plak de basisonderdelen in een nieuw bestand en sla dit
op als html-bestand (bijvoorbeeld *ninja.html*). **Let op**: pas nadat je het
bestand hebt opgeslagen krijgt de tekst ook verschillende kleuren. Als je deze
kleuren niet ziet kan het zijn dat je het bestand als tekst, dus eindigend op
*.txt* hebt opgeslagen. Zet nu ook de preview aan. Het resultaat zou er
ongeveer zo uit moeten zien:

.. cssclass:: blok

  .. raw:: HTML

    <!DOCTYPE html>
    <html>
    <head>
    </head>
    <body>
      <h1>Dit is een kop</h1>
      <p>Dit is een alinea.</p>
    </body>
    </html>

De standaard onderdelen
***********************

* ``<html>``: dit is het hoofdonderdeel van een pagina. Alle andere
  onderdelen komen binnen de ``<html></html>``
* ``<head>``: binnen dit onderdeel wordt informatie *over* de pagina gezet,
  bijvoorbeeld de titel.
* ``<body>``: binnen dit onderdeel staat alle tekst die *zichtbaar* is
  op de pagina, in het voorbeeld een kop ``<h1>`` en een alinea ``<p>``.

**Opdracht** Voeg eens een alinea met als tekst je naam in de ``<body>`` van de
pagina toe. Zie je je naam verschijnen?

.. _koppen:

Koppen
******
Om verschillende niveau's aan te geven op een pagina kun je *koppen* gebruiken.
Hiervoor zijn de ``<h1>``, ``<h2>``, ``<h3>`` (enzovoort) tags. Met deze tags
kun je je pagina een duidelijke indeling geven.

**Opdracht** Tot hoe ver gaan de niveau's eigenlijk? Bestaat ``<h20>``?

**Opdracht** Maak een pagina die er zo uitziet:

.. cssclass:: blok

  .. raw:: html

    <h1>Heelal</h1>
    <h2>Melkwegstelsel</h2>
    <h3>Zonnestelsel</h3>
    <h4>Aarde</h4>

De stijl van tekst
******************
Je kunt op een aantal manieren tekst extra benadrukken: door woorden **dik** te
maken, of `schuin`. Hiervoor kun je bijvoorbeeld de tags ``<b>`` (voor bold) en
``<i>`` (voor italic) gebruiken. Een aantal andere tags om extra effect aan je
tekst te geven zijn ``<mark>`` en ``<del>``. De HTML-code

.. code:: HTML

  Dit is <b>dik</b>

wordt dus

.. cssclass:: blok

  .. raw:: html

    Dit is <b>dik</b>

**Opdracht** Gebruik de onderdelen die hierboven genoemd zijn eens uit en maak
deze zin na (zet deze bijvoorbeeld onder de kop Aarde):

.. cssclass:: blok

  .. raw:: html

   De <b>dikke</b> <mark>gele</mark> bij vloog <i>schuin</i> over mijn
   <del>kop</del> hoofd.

Links
*****

Een superbelangrijk onderdeel van webpagina's zijn natuurlijk *links* naar
andere pagina's, op dezelfde site of op een andere. Denk maar eens aan
zoekmachines! Voor het maken van een link gebruik je de ``<a>`` tag. Het
*adres* van de link, dus waar deze naar verwijst, voeg je toe door het
*attribuut* ``href`` in de tag te zetten met als *waarde* het adres, op deze
manier:

.. code:: HTML

  <a href="https://scratch.mit.edu">

**Opdracht** Probeer op deze manier maar eens een link naar je favoriete
website te maken. **Let op**: vergeet niet de aanhalingstekens om het adres
van de website.

Zie je de link niet? Dat komt omdat je nog niets hebt toegevoegd om op te
klikken! Dit komt tussen de start- en eindtag en mag tekst zijn, maar ook
bijvoorbeeld een afbeelding.

**Opdracht** Maak op de pagina een link naar je favoriete website met de tekst
"**Mijn favoriete website!**" (let op: de tekst is dik gedrukt, hoe moest dat
ook weer?). Werkt de link? Tip: zet in de link *https://* voor de naam van de
website.

Plaatjes
********

Met alleen maar tekst zouden veel websites er maar saai uit zien. Plaatjes kun
je toevoegen aan je pagina met de ``<img>`` tag. Ook hier heb je weer een
*attribuut* nodig, dat heet ``src`` (van *source*, Engels voor bron):

.. code:: HTML

  <img src="naam-van-het-plaatje.png">

**Opdracht**: Pas de link van de vorige opdracht zo aan dat je het CoderDojo
logo hieronder gebruikt in plaats van de tekst die er staat. Download Hiervoor
het plaatje en sla het op in de map waar ook je html-pagina staat. Werkt de
link nu ook weer? **Let op**: je moet de hele naam van het plaatje gebruiken,
in dit geval is het een *png*-bestand.

.. image:: imgs/logo_coderdojo_nijmegen.png
