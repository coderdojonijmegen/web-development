Stijl toevoegen met CSS (basis)
###############################

Zonder *stijl* heeft tekst op een webpagina een standaardkleur (zwarte letters
op een witte achtergrond), standaardgrootte en standaardlettertype. Je kunt
eindeloos variëren met stijl, en er zijn verschillende manieren om stijl toe
te voegen aan je HTML.

De opdrachten in deze instructie beginnen met deze HTML-code:

.. code:: HTML

  <!DOCTYPE html>
  <html>
  <body>
    <p>
      Dit is de best gestijlde regel HTML ooit!
    </p>
    <p>
      Hoewel, misschien is deze nog wel mooier...
    </p>
  </body>
  </html>

Stijl toevoegen
***************

De makkelijkste manier om stijl toe te voegen aan je HTML is door een *style*
attribuut toe te voegen aan een HTML-element, bijvoorbeeld:
``<p style="color:red">``. In dit voorbeeld is *color* de *eigenschap* die je
wilt instellen, namelijk de kleur van de tekst. De *waarde* die je de tekst
geeft is hier *red*, dus rood.

Spelen met kleur
****************

De kleur van tekst bepaal je met de eigenschap *color*:
``<p style="color:....">``. Kleuren instellen kan op verschillende manieren,
bekijk hiervoor de pagina :ref:`html-kleuren`.

**Opdracht** Maak de tekst van de eerste alinea groen, en die van de tweede
paars:

.. cssclass:: blok

  .. raw:: html

    <p style="color:green">Dit is de best gestijlde regel HTML ooit!</p>
    <p style="color:purple">Hoewel, misschien is deze nog wel mooier...</p>


Je kunt niet alleen de kleur van de tekst zelf, maar ook de achtergrond
veranderen, dit doe je met de eigenschap *background-color*:
``<p style="background-color:....">``.

**Opdracht** Maak de tekst van de eerste alinea rood met een zwarte
achtergrond, en die van de wit met een oranje achtergrond:

.. cssclass:: blok

  .. raw:: html

    <p style="color:red;background-color:black">Dit is de best gestijlde regel HTML ooit!</p>
    <p style="color:white;background-color:orange">Hoewel, misschien is deze nog wel mooier...</p>


Tekstgrootte aanpassen
**********************

Eén manier om letters van verschillende grootte te maken is door :ref:`koppen`
te gebruiken. Dat is niet altijd handig (waarom is nu niet belangrijk) en het
kan ook met de eigenschap *font-size*. Een voorbeeld:

.. code:: HTML

  <p style="font-size:25px">Groot!</p>

geeft dit resultaat

.. cssclass:: blok

  .. raw:: html

    <p style="font-size:25px">Groot!</p>

In dit voorbeeld is *px* gebruikt om aan te geven hoe groot de tekst moet zijn,
dit is de grootte in pixels op het scherm. Je kunt ook procenten gebruiken,
waarbij 100% de "standaard" grootte is: ``<p style="font-size:100%">``.

**Opdracht** Maak de eerste zin van je pagina zo groot dat ie nog net op één
regel past, en de tweede zo klein dat je 'm nog nét kunt lezen.


Verschillende soorten letters gebruiken
***************************************

Naast de kleur en de grootte kun je ook nog het soort letters veranderen. Dit
doe je met de eigenschap *font-family*:
``<style="font-family:naam,backup-naam">``

Je ziet dat er *naam* en *backup-naam* als waarde staat ingevuld. De soort
letter *backup-naam* is niet verplicht, maar wordt gebruikt als de computer de
soort letter *naam* niet kent. Een voorbeeld:

.. code:: HTML

  <p style="font-family:broadway,serif">Broadway is niet zo goed te lezen.</p>
  <p style="font-family:verdana,sans-serif">Verdana een stuk beter.</p>

geeft dit resultaat

.. cssclass:: blok

  .. raw:: html

    <p style="font-family:broadway,serif">Broadway is niet zo goed te lezen.</p>
    <p style="font-family:verdana,serif">Verdana een stuk beter.</p>

Stijlen combineren
******************

Je kun meer dan één eigenschap tegelijk instellen door ze met een punt-komma
achter elkaar te zetten, bijvoorbeeld: ``<p style="color:red;font-size:20px">``

**Opdracht** Combineer nu in de twee zinnen verschillende kleuren,
lettergroottes en soorten letters. Leef je uit!

Toegankelijkheid
****************

Je hebt nu gezien dat je tekst op je webpagina er op heel veel verschillende
manieren kunt laten uitzien. Dat het kán betekent natuurlijk nog niet dat het
ook móét! Om te zorgen dat websites ook voor mensen die bijvoorbeeld minder
goed zien te gebruiken zijn is het belangrijk (en voor sommige websites
verplicht!) om bijvoorbeeld

* de letters groot genoeg te maken
* de kleur van de letters en die van de achtergrond verschillend genoeg te
  maken
* genoeg ruimte tussen regels tekst te laten.
