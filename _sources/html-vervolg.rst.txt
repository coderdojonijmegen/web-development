Onderdelen van een HTML-pagina (vervolg)
########################################

Nog een keer de standaardonderdelen
***********************************

.. code:: HTML

   <!DOCTYPE html>
   <html>
   <head>
     <title></title>
   </head>
   <body>
   </body>
   </html>

* Je ziet dat de ``<title>`` tag een stukje verder naar rechts
  staat dan de rest (2 spaties om precies te zijn). Dit is om
  goed te kunnen zien welke onderdelen *binnen* andere
  onderdelen zitten (in dit geval ``<title>`` binnen ``<head>``.
* Een uitzondering wordt vaak gemaakt voor de ``<head>`` en
  ``<body>`` tags, die worden gewoon helemaal links neergezet.

Blok en inline onderdelen
*************************

De bouwblokken van HTML zijn op verschillende manieren onder te verdelen. Eén
manier is om te kijken naar hoe ze zich gedragen op een webpagina.

Blok
++++
Deze onderdelen gebruiken alle ruimte die ze kunnen pakken. Ze beginnen dan ook
op een nieuwe regel. ``<p>`` is zo'n onderdeel:

.. code:: HTML

  <p style="border:solid red">Deze alinea is net zo breed als de pagina.</p>

ziet eruit als

.. cssclass:: blok

.. raw:: html

  <p style="border:solid red">Deze alinea is net zo breed als de pagina.</p>

Een ander belangrijk blok onderdeel is ``<div>``, dat veel gebruikt wordt om
verschillende stijlen toe te kunnen voegen aan verschillende stukken van de
webpagina. Hoe dit werkt wordt uitgelegd bij het :ref:`stijl-vervolg`.


Inline
++++++

Deze onderdelen gebruiken alleen de ruimte die ze nodig hebben. Een aantal
inline onderdelen zijn we al tegengekomen om tekst te benadrukken, waaronder
``<b>`` en ``<i>``. Je kunt inline onderdelen dus gebruiken *in* blok
onderdelen. Een ander voorbeeld is ``<span>``; dit kun je gebruiken om zelf een
stijl te bepalen voor een deel van een regel tekst:

.. code:: HTML

  <p>Er zit een <span style="border: solid red">inline onderdeel</span> in deze alinea.</p>

ziet eruit als

.. cssclass:: blok

.. raw:: html

  <p>Er zit een <span style="border: solid red">inline onderdeel</span> in deze alinea.</p>

**Opdracht** Maak deze regel tekst zo goed mogelijk na, gebruik hierbij
``<p>`` en ``<span>``.

.. cssclass:: blok

.. raw:: html

  <p><span style="color:red">Na</span> <span style="color:orange">regen</span> <span style="color:green">komt</span> <span style="color:blue">vaak</span> <span style="color:violet">zonneschijn</span>!</p>

Lijsten
*******

Stel dat je alle kleuren van de regenboog op wilt sommen: rood, oranje, geel,
groen, blauw, indigo en violet. Met een lijst wordt dit lekker overzichtelijk:

.. cssclass:: blok

.. raw:: html

  <ul>
    <li>rood</li>
    <li>oranje</li>
    <li>geel</li>
    <li>groen</li>
    <li>blauw</li>
    <li>indigo</li>
    <li>violet</li>
  </ul>

Om een lijst te maken zijn er de onderdelen ``<ul>`` voor een lijst zonder
nummers, en ``<ol>`` voor eentje met. De lijst hierboven maak je zo:

.. code:: HTML

  <ul>
    <li>rood</li>
    <li>oranje</li>
    <li>enzovoort</li>
  </ul>

**Opdracht** Maak zelf een genummerd lijstje met alle zeven kleuren van de
regenboog.


Video of kaart in je webpagina
******************************

YouTube
+++++++

YouTube maakt het je heel makkelijk om een filmpje *in* je eigen webpagina te
zetten (waarom zou dat zo zijn?). Als je naar `YouTube
<https://www.youtube.com>`_ gaat en op de *Share* knop klikt, is "Embed" een
van de keuzes die je dan hebt. De HTML-code die je ziet kun je vervolgens zo
aan je eigen pagina toevoegen. Het HTML-onderdeel dat hiervoor gebruikt wordt
is ``<iframe>``, wat het eigenlijk doet is de ene webpagina laten zien *in* een
andere.

Google Maps
+++++++++++

Op dezelfde manier kun je ook een landkaart van `Google Maps
<https://www.google.nl/maps>`_ toevoegen. Als je op het hamburgermenu (de drie
horizontale streepjes) klikt kun je daarna kiezen voor "Share or embed map".
Daarna kun je de HTML-code (weer een ``<iframe>``) in je pagina kopiëren.