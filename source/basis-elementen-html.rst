Structuur van een HTML-pagina
#############################
Websites worden geschreven in de taal van het internet: HTML. Er zijn veel
verschillende "woorden" in HTML. Een aantal van de meest gebruikte leer je hier
kennen.

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
######################

* ``<html>``: dit is het hoofdonderdeel van een pagina. Alle andere
  onderdelen zitten binnen de ``<html></html>``
* ``<head>``: binnen dit onderdeel wordt informatie *over* de pagina gezet.
* ``<title>``: een van de onderdelen in het ``<head>`` deel.

  **Opdracht**: neem de basisonderdelen over en geef je pagina een titel.
  Zie je waar de titel verschijnt?

* ``<body>``: binnen dit onderdeel staat alle tekst die *zichtbaar* is
  op de pagina.

  **Opdracht**: Typ eens je naam in de ``<body>`` van de pagina. Komt deze
  inderdaad tevoorschijn?


Koptekst / hoofdstukken
#######################
Om verschillende niveau's aan te geven op een pagina zijn er de ``<h1>``,
``<h2>``, ``<h3>`` (enzovoort) tags. Met deze tags kun je je pagina een
duidelijke indeling geven.

**Opdracht**: Bestaat ``<h20>``? Tot hoe ver gaan de niveau's?

**Opdracht**: Maak een pagina die er zo uitziet:

.. cssclass:: blok

  .. raw:: html

    <h1>Heelal</h1>
    <h2>Melkwegstelsel</h2>
    <h3>Zonnestelsel</h3>
    <h4>Aarde</h4>

De stijl van tekst
######################
Je kunt op een aantal manieren tekst extra benadrukken: door woorden **dik** te
maken, of `schuin`. Hiervoor kun je bijvoorbeeld de tags ``<b>`` (voor bold) en
``<i>`` (voor italic) gebruiken. Een aantal andere tags om extra effect aan je
tekst te geven zijn ``<mark>`` en ``<del>``.

**Opdracht**: Maak deze zin na:

.. cssclass:: blok

  .. raw:: html

   De <b>dikke</b> <mark>gele</mark> bij vloog <i>schuin</i> over mijn
   <del>kop</del> hoofd.

Links
######################


Afbeeldingen
######################
