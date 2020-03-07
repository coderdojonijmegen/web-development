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
     <title></title>
   </head>
   <body>
   </body>
   </html>


* HTML onderdelen worden aangegeven met *tags*: de naam van
  het onderdeel tussen ``<>`` haakjes.
* De meeste onderdelen hebben een *start* en een *eind* tag.
* De eind tag heeft een *forward slash* dus ``/`` voor de naam,
  bijvoorbeeld ``</html>``.
* Tags worden altijd geschreven met *kleine letters*.

De standaardonderdelen
**********************

* ``<html>``: dit is het hoofdonderdeel van een pagina. Alle andere
  onderdelen zitten binnen de ``<html></html>``
* ``<head>``: binnen dit onderdeel wordt informatie *over* de pagina gezet.
* ``<title>``: een van de onderdelen in het ``<head>`` deel.

  **Opdracht** Neem de basisonderdelen over in een nieuw bestand en sla het op
  als html-bestand (bijvoorbeeld *ninja.html*). Geef je pagina nu een titel en
  bekijk de preview. Zie de titel ergens verschijnen? Hint: je moet het
  hiervoor in een echte browser openen.

* ``<body>``: binnen dit onderdeel staat alle tekst die *zichtbaar* is
  op de pagina.

  **Opdracht** Typ eens je naam in de ``<body>`` van de pagina. Komt deze
  inderdaad tevoorschijn?

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

**Opdracht** Maak deze zin na (zet 'm onder het hoofdstuk Aarde):

.. cssclass:: blok

  .. raw:: html

   De <b>dikke</b> <mark>gele</mark> bij vloog <i>schuin</i> over mijn
   <del>kop</del> hoofd.

Links
**********************
Een superbelangrijk onderdeel van webpagina's zijn natuurlijk verwijzingen
oftewel *links* naar andere pagina's, op dezelfde site of op een andere. Denk
maar eens aan zoekmachines! Voor het maken van een link gebruik je de ``<a>``
tag. Het *adres* van de link, dus waar deze naar verwijst, stop je in de tag
met *href=*, op deze manier: ``<a href=adres-van-de-pagina>``.

**Opdracht** Probeer op deze manier maar eens een link naar je favoriete
website te maken.

Zie je de link niet? Dat komt omdat je nog niets hebt toegevoegd om op te
klikken! Dit komt tussen de start- en eindtag en mag tekst zijn, maar ook
bijvoorbeeld een afbeelding.

**Opdracht** Maak op de pagina een link naar je favoriete website met de tekst
"**Mijn favoriete website!**" (let op: de tekst is dik gedrukt).


Plaatjes
**********************
Met alleen maar tekst zouden veel websites er maar saai uit zien. Plaatjes kun
je toevoegen aan je pagina met de ``<img>`` tag. Ook hier heb je weer een
*attribuut* nodig, dat heet *src* (van *source*, Engels voor bron).

**Opdracht**: Verander bij de vorige opdracht de tekst in onderstaand logo
(download het en sla het op in de map waar ook je .html pagina staat). Klik dan
op het plaatje om de link uit te proberen.

Tip 1: het is een *.png* bestand.
Tip 2: zet in de link *https://* voor de naam van de website.

.. image:: imgs/logo_coderdojo_nijmegen.png
