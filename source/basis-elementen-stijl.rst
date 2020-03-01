Basisstijl voor een HTML-pagina
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

Je kun meer dan één eigenschap tegelijk instellen door ze met een punt-komma
achter elkaar te zetten, bijvoorbeeld: ``<p style="color:red;font-size:20px">``


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

``<style="font-size:XXXXX">``


Verschillende lettertypes gebruiken
***********************************

``<style="font-family:XXXXX">``
