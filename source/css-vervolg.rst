.. _stijl-vervolg:

Maak voor de opdrachten in deze instructie een HTML-bestand met deze inhoud:

.. code:: HTML

  <!DOCTYPE html>
  <head>
  <style>
     /* hier komt je styling! */
  </style>
  </head>
  <body>
    <h1>Deze pagina gaan we stylen!</h1>
    <h2>Dit is een h2 kop</h2>
    <div>
      <h2>Dit is ook een h2 kop!</h2>
        <p>Wat zullen we met <span>deze</span> alinea gaan doen?</p>
        <p>Deze alinea wordt nog mooier dan de vorige.</p>
    </div>
    <div>
      <p>De vorige alinea's zijn <span>jaloers</span> op mij.</p>
      <p>Jaloers op mij zul je bedoelen!</p>
    </div>
  </body>
  </html>


Stijl toevoegen met CSS (vervolg)
#################################

Tot nu toe heb je stijl toegevoegd door ``style="..."`` te gebruiken in de
HTML-onderdelen. Dat heeft voordelen en nadelen. Het is handig dat je meteen
kunt zien hoe de inhoud van je webpagina eruit komt te zien. Minder handig is
dat je aan *ieder* stukje HTML op deze manier een stijl moet toevoegen. Dat is
én veel werk, én wordt al snel onoverzichtelijk als je veel stijlen hebt.

Het is daarom gebruikelijk bij webpagina's om de inhoud en stijl op
verschillende plekken neer te zetten. Een manier om dit te doen is binnen het
``<style>`` onderdeel. De code binnen het ``<style>`` onderdeel ziet er wat
anders uit dan je tot nu toe gezien hebt. Om tekst rood te maken gebruikte je

.. code:: HTML

  <p style="color:red">Dit stukje tekst is rood</p>

Binnen ``<style>`` moet je deze code schrijven, een soort *regel* voor hoe de
HTML zich moet gedragen:

.. code:: CSS

  p {
    color: red;
  }

**Opdracht** Wat denk je dat er gebeurt als je dit stukje code in het
``<style>`` onderdeel zet? Probeer het eens. Had je gelijk?

Stijl toevoegen aan sommige, maar niet alle elementen
#####################################################

Als je de opdracht van net hebt uitgevoerd, heb je gezien dat *alle* ``<p>``
onderdelen, dus alle alinea's, rode tekst hebben. Dit is dus wat deze code
doet:

* de *eigenschap* kleur krijgt
* de *waarde* rood
* voor *alle* ``<p>`` onderdelen

Maar stel nou dat je alleen bepaalde alinea's rood wilt maken?

Class
+++++

Dat kan bijvoorbeeld door het HTML-onderdeel lid te maken van een zogenaamde
*class*:

.. code:: HTML

  <p class="naamvandeclass">Welke kleur is dit?</p>

In de CSS maak je een class door een *punt* aan het begin te gebruiken:

.. code:: CSS

  .naamvandeclass {
    color: red;
  }


**Opdracht** Gebruik een *class* met de naam "rodealinea" om de 1e en 4e alinea
rood te maken, dus zo:

.. cssclass:: blok

  .. raw:: HTML

    <!DOCTYPE html>
    <head>
    <style>
      .rodealinea {
        color: red;
      }
    </style>
    </head>
    <body>
      <h1>Deze pagina gaan we stylen!</h1>
      <h2>Dit is een h2 kop</h2>
      <div>
        <h2>Dit is ook een h2 kop!</h2>
          <p class="rodealinea">Wat zullen we met <span>deze</span> alinea gaan doen?</p>
          <p>Deze alinea wordt nog mooier dan de vorige.</p>
      </div>
      <div>
        <p>De vorige alinea's zijn <span>jaloers</span> op mij.</p>
        <p class="rodealinea">Jaloers op mij zul je bedoelen!</p>
      </div>
    </body>
    </html>

ID
++

Een andere manier is om een HTML-onderdeel een uniek *id* te geven:

.. code:: HTML

  <p id="ikbenuniek">Welke kleur is dit?</p>

In de CSS verwijs je naar een id door een *hashtag* aan het begin te gebruiken:

.. code:: CSS

  #ikbenuniek {
    color: red;
  }

**Opdracht** Maak de tekst van de eerste h1 kop blauw, en de 1e h2 kop groen
(tip: je hebt hiervoor twee id's nodig, "ikbenblauw" en "ikbengroen"):

.. cssclass:: blok

  .. raw:: HTML

    <!DOCTYPE html>
    <head>
    <style>
      .rodealinea {
        color: red;
      }
      #ikbenblauw {
        color: blue;
      }

      #ikbengroen {
        color: green;
      }
    </style>
    </head>
    <body>
      <h1 id="ikbenblauw">Deze pagina gaan we stylen!</h1>
      <h2 id="ikbengroen">Dit is een h2 kop</h2>
      <div>
        <h2>Dit is ook een h2 kop!</h2>
          <p class="rodealinea">Wat zullen we met <span>deze</span> alinea gaan doen?</p>
          <p>Deze alinea wordt nog mooier dan de vorige.</p>
      </div>
      <div>
        <p>De vorige alinea's zijn <span>jaloers</span> op mij.</p>
        <p class="rodealinea">Jaloers op mij zul je bedoelen!</p>
      </div>
    </body>
    </html>

Samengevat heb je nu gezien dat je stijl kunt geven aan

* alle onderdelen van een bepaalde soort
* bepaalde onderdelen door ze lid te maken van een class
* losse onderdelen door ze een (uniek) id te geven

Combineren van stijlen
######################

Een grote kracht van CSS is dat je stijlen ook kunt combineren. Zo kun je
meerdere eigenschappen tegelijk instellen in een CSS regel:

.. code:: CSS

  p {
    color: red;
    font-weight: bold;
  }

**Opdracht** Voeg een tweede eigenschap toe aan de "rodealinea", bijvoorbeeld
*background-color* of *font-family*.

Je kunt een onderdeel ook lid maken van meer dan één *class* (in dit voorbeeld
heten die "rodealinea" en "box"):

.. code:: HTML

  <p class="rodealinea box"

**Opdracht** Maak een class "box" die de eigenschap ``border`` instelt op ``1px
solid black``, en voeg deze toe aan een van de rode alinea's:

.. cssclass:: blok

  .. raw:: HTML

    <!DOCTYPE html>
    <head>
    <style>
      .rodealinea {
        color: red;
      }
      #ikbenblauw {
        color: blue;
      }

      #ikbengroen {
        color: green;
      }
      .box {
        border: 1px solid black;
      }
    </style>
    </head>
    <body>
      <h1 id="ikbenblauw">Deze pagina gaan we stylen!</h1>
      <h2 id="ikbengroen">Dit is een h2 kop</h2>
      <div>
        <h2>Dit is ook een h2 kop!</h2>
          <p class="rodealinea box">Wat zullen we met <span>deze</span> alinea gaan doen?</p>
          <p>Deze alinea wordt nog mooier dan de vorige.</p>
      </div>
      <div>
        <p>De vorige alinea's zijn <span>jaloers</span> op mij.</p>
        <p class="rodealinea">Jaloers op mij zul je bedoelen!</p>
      </div>
    </body>
    </html>
