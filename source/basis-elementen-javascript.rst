Onderdelen van javascript (basis)
###########################################

De HTML die je net hebt geleerd is statisch. 
Om hier acties aan toe te voegen zoals het klikken van een knop gebruiken we Javascript.
Net zoals HTML kent ook Javascript veel verschillende "woorden". Hier behandelen we er een aantal.

Toevoegen aan een HTML bestand
--------------------------------
Javascript wordt voor HTML bestanden geschreven in een speciaal blok:

.. code:: HTML

   <!DOCTYPE html>
   <html>
   <head>
     <script>
      javascript code hier!
     </script>
   </head>
   <body>
   </body>
   </html>

Dit ziet er als volgt uit met code (De code wordt verder toegelicht):

.. code:: HTML

   <!DOCTYPE html>
   <html>
   <head>
     <script>

      const telOp = function(getal1, getal2) {
        return getal1+getal2;
      }

      const resultaat = telOp(1,2);

      console.log(resultaat);

     </script>
   </head>
   <body>
   </body>
   </html>

Functies
--------------------------------
Een functie in javascript ziet er als volgt uit:

.. code:: Javascript

    const telOp = function(getal1, getal2) {
        return getal1+getal2;
    }


Hierbij zie je dat ``function`` aangeeft dat het een 'functie' is.
Vervolgens geven we de parameters op. Bij ons zijn dat getal1 en getal2.
Als laatst gebruiken we deze twee variabelen om een optelling te doen.
We geven dit getal terug door ``return`` te gebruiken.

Als we dit stukje code als volgt aanroepen:

.. code:: Javascript

   const resultaat = telOp(1,2);
   console.log(resultaat)

Dan zien we dat er 3 wordt geprint!
We slaan hierbij het resultaat op in ``resultaat``
en printen die vervolgens met ``console.log()``.
Om nu de output te zien van de ``console.log()`` functie moeten we de ``console`` openen.
Je kunt dit doen op verschillende manieren:

Windows:

* F12
* Rechtermuisknop + inspecteer
* Control+Shift+J

MacOs:

* Command+Option+J	

Variabelen
--------------------------------
Variabelen in javascript gebruiken net als andere talen een speciale `syntax`.
In javascript kennen we `var`, `const` en `let`.
Een goede tip om problemen tegen te gaan is om alleen `const` en `let` te gebruiken.

`const` gebruiken we als een variabelen niet meer veranderd,
en `let` als we de variabelen later nog aan willen passen.

Een veriabele resultaat maken doen we als volgt:

.. code:: Javascript

   let resultaat = 6; //Zo
   const resultaatConst = 6; //Of zo

In variabelen kunnen we data opslaan, dat is heel handig!


Voorbeeld 1: Knop
--------------------------------
Bij een knop gaan we `HTML` en `Javascript` combineren!

**Opdracht** Zorg allereest dat je een `HTML` pagina hebt met een knop.

.. code:: HTML

   <!DOCTYPE html>
   <html>
   <head>
   </head>
   <body>
      <button> Klik op mij! </button>
   </body>
   </html>

Wat gebeurt er nu als je op de knop klikt?

**Opdracht** Om nu interactie toe te voegen aan de knop gaan we javascript en html combineren.

* Op de knop kunnen we de volgende HTML toevoegen: **onclick=""**. Nu werkt het echter nog niet..!
* Nu moeten we een javascript functie schrijven die de knop aan gaat roepen, weet jij nog waar dit moet staan in het HTML bestand?:

   .. code:: Javascript

      const buttonClicked = function() {
         alert("Je hebt op de knop geklikt!");      
      }

* Als laatst gaan we deze twee elementen aan elkaar koppelen door de **onclick=""** aan te passen (Hier moet je wel de javascript nog toevoegen!):

   .. code:: HTML

      <!DOCTYPE html>
      <html>
      <head>
      </head>
      <body>
         <button onclick="buttonClicked()"> Klik op mij! </button>
      </body>
      </html>


Voorbeeld 2: Een element toevoegen op de pagina
-----------------------------------------------
We kunnen in `Javascript` nog veel meer doen dan interactie toevoegen aan bijvoorbeeld knoppen.
Zo kunnen we ook `HTML` toevoegen, aan de `HTML` pagina!

We hebben hier een aantal functies voor in Javascript

.. code::Javascript

   const element = document.getElementById("<id>");
   element.insertAdjacentHTML("afterend", "<p>My text</p>");

Er zijn nog veel meer mogelijkheden, maar dit is een van de simpelste.

   .. code:: HTML

      <!DOCTYPE html>
      <html>
      <head>
         <script>
            const voegElementToe = function() {
               const element = document.getElementById("mijnDivId");
               element.insertAdjacentHTML("afterend", "<p>My text</p>");
            }
         </script>
      </head>
      <body>
      <button onclick="voegElementToe()"> Klik op mij! </button>
      <div id="mijnDivId"> Dit is een div</div>
      </body>
      </html>


**opdracht** Kun jij nu met jouw kennis van Javascript en HTML een element toevoegen als je op een knop klikt?

Voorbeeld 3: Reageren op berichten van een gebruiker
-----------------------------------------------------

Met de volgende HTML code hebben we een invoer veld waar de gebruiker iets in kan typen:

 .. code:: HTML

   <!DOCTYPE html>
      <html>
      <head>
          <style>
              #inputId {
                  width: 300px;
                  height: 40px;
                  font-size: xx-large;
              }

              .container {
                  display: flex;
                  height: 100vh;
                  justify-content: center;
                  align-items: center;
                  background-color: blue;
              }
          </style>
         <script>
            //Javascript code hier!
         </script>
      </head>
      <body class="container">
        <span> Wat is je naam? </span>
        <input id="inputId"> </input>
      </body>
      </html>

Als de gebruiker nu iets typt, zie je alleen de tekst staan. Er gebeurt verder nog niet zo veel.
Kun jij ervoor zorgen dat de computer terugpraat?

* Voeg een knop toe aan de HTML pagina
* Als je op de knop klikt, log dan de text die in het input veld staat met ``console.log``.
  Om de tekst uit het invoer veld te halen kun je gebruik maken van:
  ``const input = document.getElementById("inputId").value;``

* Kun jij nu de computer ``Hallo <naam>`` laten zeggen?
  Je kan dit doen met de functie ``alert()``, hier moet je nog wel text aan meegeven.
  Dit is een voorbeeld: ``alert("Hoi Kevin!")``