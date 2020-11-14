---
title: "Web - Development"
date: 2020-10-22T20:01:11+02:00
draft: false
toc: true
headercolor: "teal-background"
taal: HTML, CSS & JavaScript
---

Er zijn een paar verschillende *talen* die samen voor een belangrijk deel
bepalen wat er op websites staat (HTML), hoe ze eruit zien (CSS) en hoe ze
werken (JavaScript). 

<!--more-->

## Introductie

Afhankelijk van hoeveel ervaring je al hebt met deze talen kun je beginnen
bij de basis, of een vervolgpagina kiezen. De instructies bestaan uit een
deel uitleg met tussendoor opdrachten om te oefenen met alle onderdelen.

![web logo's](imgs/html-css-js-logos.png)


## Benodigdheden

Voor deze instructies gebruiken we Visual Studio Code (VS Code) om de code te
schrijven, en om het resultaat te bekijken. Download en installeer eerst
VS Code:
[Download Visual Studio Code](https://code.visualstudio.com/download)

![Visual Studio Code extensie](imgs/vscode_extensions_online.png)

1. Ga nu naar het Extensions menu.
2. Zoek naar de extensie *HTML Preview*.
3. Installeer de extensie en herstart VS Code.

Om een html-pagina te laten zien in VS Code moet je op het `preview` icoon
klikken, dit bevindt zich rechtsboven in het scherm (let op: het is alleen
zichtbaar als je een bestand van het soort .html open hebt, niet bij
bijvoorbeeld een .txt bestand):

![preview](imgs/vscode_preview.png)

Je bent nu klaar om te beginnen met de instructies!

## Onderdelen van een HTML-pagina (basis)

### Structuur van een pagina

Websites worden geschreven in de taal van het internet: HTML. Er zijn veel
verschillende "woorden", of "bouwblokken", in HTML. Een aantal van de meest
gebruikte leer je hier kennen.

Een HTML-pagina heeft een paar standaard onderdelen:

{{< highlight html>}}

  <!DOCTYPE html>
  <html>
  <head>
  </head>
  <body>
    <h1>Dit is een kop</h1>
    <p>Dit is een alinea.</p>
  </body>
  </html>
{{< /highlight >}}


 - HTML onderdelen worden aangegeven met *tags*: de naam van het onderdeel tussen `<>` haakjes.
 - De meeste onderdelen hebben een *start* en een *eind* tag.
 - De eind tag heeft een *forward slash* dus `/` voor de naam, bijvoorbeeld `</html>`.
 - Tags worden altijd geschreven met *kleine letters*.


**Opdracht** Kopieer en plak de basisonderdelen in een nieuw bestand en sla dit
op als html-bestand (bijvoorbeeld *ninja.html*). **Let op**: pas nadat je het
bestand hebt opgeslagen krijgt de tekst ook verschillende kleuren. Als je deze
kleuren niet ziet kan het zijn dat je het bestand als tekst, dus eindigend op
*.txt* hebt opgeslagen. Zet nu ook de preview aan. Het resultaat zou er
ongeveer zo uit moeten zien:

{{< html_voorbeeld >}}
      <h1>Dit is een kop</h1>
      <p>Dit is een alinea.</p>
{{< /html_voorbeeld >}}

### De standaard onderdelen

 - `<html>`: dit is het hoofdonderdeel van een pagina. Alle andere onderdelen komen binnen de `<html></html>`
 - `<head>`: binnen dit onderdeel wordt informatie *over* de pagina gezet, bijvoorbeeld de titel.
 - `<body>`: binnen dit onderdeel staat alle tekst die *zichtbaar* is op de pagina, in het voorbeeld een kop `<h1>` en een alinea `<p>`.

**Opdracht** Voeg eens een alinea met als tekst je naam in de `<body>` van de
pagina toe. Zie je je naam verschijnen?

### Koppen

Om verschillende niveau's aan te geven op een pagina kun je *koppen* gebruiken.
Hiervoor zijn de `<h1>`, `<h2>`, `<h3>` (enzovoort) tags. Met deze tags
kun je je pagina een duidelijke indeling geven.

**Opdracht** Tot hoe ver gaan de niveau's eigenlijk? Bestaat `<h20>`?

**Opdracht** Maak een pagina die er zo uitziet:

{{< html_voorbeeld >}}
    <h1>Heelal</h1>
    <h2>Melkwegstelsel</h2>
    <h3>Zonnestelsel</h3>
    <h4>Aarde</h4>
{{< /html_voorbeeld >}}

### De stijl van tekst

Je kunt op een aantal manieren tekst extra benadrukken: door woorden **dik** te
maken, of `schuin`. Hiervoor kun je bijvoorbeeld de tags `<b>` (voor bold) en
`<i>` (voor italic) gebruiken. Een aantal andere tags om extra effect aan je
tekst te geven zijn `<mark>` en `<del>`. De HTML-code

{{< highlight html >}}
  Dit is <b>dik</b>
{{< /highlight >}}

wordt dus

{{< html_voorbeeld >}}
    Dit is <b>dik</b>
{{< /html_voorbeeld >}}

**Opdracht** Gebruik de onderdelen die hierboven genoemd zijn eens uit en maak
deze zin na (zet deze bijvoorbeeld onder de kop Aarde):

{{< html_voorbeeld >}}
   De <b>dikke</b> <mark>gele</mark> bij vloog <i>schuin</i> over mijn
   <del>kop</del> hoofd.
{{< /html_voorbeeld >}}

### Links

Een superbelangrijk onderdeel van webpagina's zijn natuurlijk *links* naar
andere pagina's, op dezelfde site of op een andere. Denk maar eens aan
zoekmachines! Voor het maken van een link gebruik je de `<a>` tag. Het
*adres* van de link, dus waar deze naar verwijst, voeg je toe door het
*attribuut* `href` in de tag te zetten met als *waarde* het adres, op deze
manier:

{{< highlight html >}}
  <a href="https://scratch.mit.edu">
{{< /highlight >}}

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

### Plaatjes

Met alleen maar tekst zouden veel websites er maar saai uit zien. Plaatjes kun
je toevoegen aan je pagina met de `<img>` tag. Ook hier heb je weer een
*attribuut* nodig, dat heet `src` (van *source*, Engels voor bron):

{{< highlight html >}}
  <img src="naam-van-het-plaatje.png">
{{< /highlight >}}

**Opdracht**: Pas de link van de vorige opdracht zo aan dat je het CoderDojo
logo hieronder gebruikt in plaats van de tekst die er staat. Download Hiervoor
het plaatje en sla het op in de map waar ook je html-pagina staat. Werkt de
link nu ook weer? **Let op**: je moet de hele naam van het plaatje gebruiken,
in dit geval is het een *png*-bestand.

![Logo CoderDojo Nijmegen](imgs/logo_coderdojo_nijmegen.png)

## Stijl toevoegen met CSS (basis)

Zonder *stijl* heeft tekst op een webpagina een standaardkleur (zwarte letters
op een witte achtergrond), standaardgrootte en standaardlettertype. Je kunt
eindeloos variëren met stijl, en er zijn verschillende manieren om stijl toe
te voegen aan je HTML.

De opdrachten in deze instructie beginnen met deze HTML-code:

{{< highlight html >}}
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
{{< /highlight >}}

Dit zou er in de preview zo uit moeten zien:

{{< html_voorbeeld >}}
      <p>
        Dit is de best gestijlde regel HTML ooit!
      </p>
      <p>
        Hoewel, misschien is deze nog wel mooier...
      </p>
{{< /html_voorbeeld >}}

### Stijl toevoegen

De makkelijkste manier om stijl toe te voegen aan je HTML is door een `style`
attribuut toe te voegen aan een HTML-element, bijvoorbeeld:

{{< highlight html >}}
  <p style="color:red">Wat zou de kleur van deze tekst zijn?</p>
{{< /highlight >}}

In dit voorbeeld is *color* de *eigenschap* die je
wilt instellen, namelijk de kleur van de tekst. De *waarde* die je de tekst
geeft is hier *red*, dus rood.

### Spelen met kleur

De kleur van tekst bepaal je met de eigenschap *color*:
`<p style="color:....">`. Kleuren instellen kan op verschillende manieren,
bekijk hiervoor de pagina :ref:`html-kleuren`.

**Opdracht** Maak de tekst van de eerste alinea groen, en die van de tweede
paars:

{{< html_voorbeeld >}}
    <p style="color:green">Dit is de best gestijlde regel HTML ooit!</p>
    <p style="color:purple">Hoewel, misschien is deze nog wel mooier...</p>
{{< /html_voorbeeld >}}

Je kunt niet alleen de kleur van de tekst zelf, maar ook de achtergrond
veranderen, dit doe je met de eigenschap *background-color*:
`<p style="background-color:....">`.

**Opdracht** Maak de tekst van de eerste alinea rood met een zwarte
achtergrond, en die van de wit met een oranje achtergrond:

{{< html_voorbeeld >}}
    <p style="color:red;background-color:black">Dit is de best gestijlde regel HTML ooit!</p>
    <p style="color:white;background-color:orange">Hoewel, misschien is deze nog wel mooier...</p>
{{< /html_voorbeeld >}}

### Tekstgrootte aanpassen

Eén manier om letters van verschillende grootte te maken is door :ref:`koppen`
te gebruiken. Dat is niet altijd handig (waarom is nu niet belangrijk) en het
kan ook met de eigenschap *font-size*. Een voorbeeld:

{{< highlight html >}}
  <p style="font-size:25px">Groot!</p>
{{< /highlight >}}

geeft dit resultaat

{{< html_voorbeeld >}}
    <p style="font-size:25px">Groot!</p>
{{< /html_voorbeeld >}}

In dit voorbeeld is *px* gebruikt om aan te geven hoe groot de tekst moet zijn,
dit is de grootte in pixels op het scherm. Je kunt ook procenten gebruiken,
waarbij 100% de "standaard" grootte is: `<p style="font-size:100%">`.

**Opdracht** Maak de eerste zin van je pagina zo groot dat ie nog net op één
regel past, en de tweede zo klein dat je 'm nog nét kunt lezen.

### Verschillende soorten letters gebruiken

Naast de kleur en de grootte kun je ook nog het soort letters veranderen. Dit
doe je met de eigenschap *font-family*:
`<style="font-family:naam,backup-naam">`

Je ziet dat er *naam* en *backup-naam* als waarde staat ingevuld. De soort
letter *backup-naam* is niet verplicht, maar wordt gebruikt als de computer de
soort letter *naam* niet kent. Een voorbeeld:

{{< highlight html >}}
  <p style="font-family:broadway,serif">Broadway is niet zo goed te lezen.</p>
  <p style="font-family:verdana,sans-serif">Verdana een stuk beter.</p>
{{< /highlight >}}

geeft dit resultaat

{{< html_voorbeeld >}}
    <p style="font-family:broadway,serif">Broadway is niet zo goed te lezen.</p>
    <p style="font-family:verdana,serif">Verdana een stuk beter.</p>
{{< /html_voorbeeld >}}

### Stijlen combineren

Je kun meer dan één eigenschap tegelijk instellen door ze met een punt-komma
achter elkaar te zetten, bijvoorbeeld: `<p style="color:red;font-size:20px">`

**Opdracht** Combineer nu in de twee zinnen verschillende kleuren,
lettergroottes en soorten letters. Leef je uit!

### Toegankelijkheid

Je hebt nu gezien dat je tekst op je webpagina er op heel veel verschillende
manieren kunt laten uitzien. Dat het kán betekent natuurlijk nog niet dat het
ook móét! Om te zorgen dat websites ook voor mensen die bijvoorbeeld minder
goed zien te gebruiken zijn is het belangrijk (en voor sommige websites
verplicht!) om bijvoorbeeld

 - de letters groot genoeg te maken
 - de kleur van de letters en die van de achtergrond verschillend genoeg te
  maken
 - genoeg ruimte tussen regels tekst te laten.


## Actie toevoegen met JavaScript (basis)

De HTML die je net hebt geleerd is statisch.  Om hier acties aan toe te voegen,
zoals het klikken van een knop gebruiken we JavaScript (JS). Net zoals HTML
kent ook JS veel verschillende "woorden". Hier behandelen we er een aantal.

### Toevoegen aan een HTML bestand

JS wordt voor HTML bestanden geschreven in een speciaal blok:

{{< highlight html >}}
   <!DOCTYPE html>
   <html>
   <head>
     <script>
      JavaScript code hier!
     </script>
   </head>
   <body>
   </body>
   </html>
{{< /highlight >}}

Dit ziet er als volgt uit met code (De code wordt verder toegelicht):

{{< highlight html >}}
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
{{< /highlight >}}

### Functies

Een functie in JS ziet er als volgt uit:

{{< highlight javascript >}}
    const telOp = function(getal1, getal2) {
        return getal1+getal2;
    }
{{< /highlight >}}


Hierbij zie je dat `function` aangeeft dat het een 'functie' is.
Vervolgens geven we de parameters op. Bij ons zijn dat getal1 en getal2.
Als laatst gebruiken we deze twee variabelen om een optelling te doen.
We geven dit getal terug door `return` te gebruiken.

Als we dit stukje code als volgt aanroepen:

{{< highlight javascript >}}
   const resultaat = telOp(1,2);
   console.log(resultaat)
{{< /highlight >}}

Dan zien we dat er 3 wordt geprint!
We slaan hierbij het resultaat op in `resultaat`
en printen die vervolgens met `console.log()`.
Om nu de output te zien van de `console.log()` functie moeten we de
`console` openen. Je kunt dit doen op verschillende manieren:

Windows:

* F12
* Rechtermuisknop + inspecteer
* Control+Shift+J

MacOs:

* Command+Option+J

### Variabelen

Variabelen in JS gebruiken net als andere talen een speciale `syntax`.
In JS kennen we `var`, `const` en `let`. Een goede tip om problemen tegen
te gaan is om alleen `const` en `let` te gebruiken.

`const` gebruiken we als een variabelen niet meer veranderd,
en `let` als we de variabelen later nog aan willen passen.

Een variabele `resultaat` maken doen we als volgt:

{{< highlight javascript >}}
   let resultaat = 6; //Zo
   const resultaatConst = 6; //Of zo
{{< /highlight >}}

In variabelen kunnen we data opslaan, dat is heel handig!

#### Voorbeeld 1: Knop

Bij een knop gaan we `HTML` en `JS` combineren!

**Opdracht** Zorg allereest dat je een `HTML` pagina hebt met een knop.

{{< highlight html >}}
   <!DOCTYPE html>
   <html>
   <head>
   </head>
   <body>
      <button> Klik op mij! </button>
   </body>
   </html>
{{< /highlight >}}

Wat gebeurt er nu als je op de knop klikt?

**Opdracht** Om nu interactie toe te voegen aan de knop gaan we JS en html
combineren.

 - Op de knop kunnen we de volgende HTML toevoegen: **onclick=""**. Nu werkt
  het echter nog niet..!
 - Nu moeten we een JS functie schrijven die de knop aan gaat roepen, weet jij
  nog waar dit moet staan in het HTML bestand?:

{{< highlight javascript >}}
      const buttonClicked = function() {
         alert("Je hebt op de knop geklikt!");
      }
{{< /highlight >}}

 - Als laatste gaan we deze twee elementen aan elkaar koppelen door de
  **onclick=""** aan te passen (Hier moet je wel de JS nog toevoegen!):

{{< highlight html >}}
      <!DOCTYPE html>
      <html>
      <head>
      </head>
      <body>
         <button onclick="buttonClicked()"> Klik op mij! </button>
      </body>
      </html>
{{< /highlight >}}


#### Voorbeeld 2: Een element toevoegen op de pagina

We kunnen in `JS` nog veel meer doen dan interactie toevoegen, bijvoorbeeld aan
knoppen. Ook kunnen we `HTML` toevoegen aan de `HTML` pagina!

We hebben hier een aantal functies voor in JS.

{{< highlight javascript >}}
   const element = document.getElementById("<id>");
   element.insertAdjacentHTML("afterend", "<p>My text</p>");
{{< /highlight >}}

Er zijn nog veel meer mogelijkheden, maar dit is een van de simpelste.

{{< highlight html >}}
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
{{< /highlight >}}

**Opdracht** Kun jij nu met jouw kennis van JS en HTML een element toevoegen
als je op een knop klikt?

#### Voorbeeld 3: Reageren op berichten van een gebruiker

Met de volgende HTML code hebben we een invoer veld waar de gebruiker iets in
kan typen:

{{< highlight html >}}
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
            //JavaScript code hier!
         </script>
      </head>
      <body class="container">
        <span> Wat is je naam? </span>
        <input id="inputId"> </input>
      </body>
      </html>
{{< /highlight >}}

Als de gebruiker nu iets typt, zie je alleen de tekst staan. Er gebeurt verder
nog niet zo veel. Kun jij ervoor zorgen dat de computer terugpraat?

 - Voeg een knop toe aan de HTML pagina
 - Als je op de knop klikt, log dan de text die in het input veld staat met
  `console.log`. Om de tekst uit het invoer veld te halen kun je gebruik
  maken van: `const input = document.getElementById("inputId").value;`
 - Kun jij nu de computer `Hallo <naam>` laten zeggen? Je kan dit doen met de
  functie `alert()`, hier moet je nog wel text aan meegeven. Dit is een
  voorbeeld: `alert("Hoi Kevin!")`


## Stijl toevoegen met CSS (vervolg)

Maak voor de opdrachten in deze instructie een HTML-bestand met deze inhoud:

{{< highlight html >}}
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
{{< /highlight >}}

Tot nu toe heb je stijl toegevoegd door `style="..."` te gebruiken in de
HTML-onderdelen. Dat heeft voordelen en nadelen. Het is handig dat je meteen
kunt zien hoe de inhoud van je webpagina eruit komt te zien. Minder handig is
dat je aan *ieder* stukje HTML op deze manier een stijl moet toevoegen. Dat is
én veel werk, én wordt al snel onoverzichtelijk als je veel stijlen hebt.

Het is daarom gebruikelijk bij webpagina's om de inhoud en stijl op
verschillende plekken neer te zetten. Een manier om dit te doen is binnen het
`<style>` onderdeel. De code binnen het `<style>` onderdeel ziet er wat
anders uit dan je tot nu toe gezien hebt. Om tekst rood te maken gebruikte je

{{< highlight html >}}
  <p style="color:red">Dit stukje tekst is rood</p>
{{< /highlight >}}

Binnen `<style>` moet je deze code schrijven, een soort *regel* voor hoe de
HTML zich moet gedragen:

{{< highlight css >}}
  p {
    color: red;
  }
{{< /highlight >}}

**Opdracht** Wat denk je dat er gebeurt als je dit stukje code in het
`<style>` onderdeel zet? Probeer het eens. Had je gelijk?

### Stijl toevoegen aan sommige, maar niet alle elementen

Als je de opdracht van net hebt uitgevoerd, heb je gezien dat *alle* `<p>`
onderdelen, dus alle alinea's, rode tekst hebben. Dit is dus wat deze code
doet:

 - de *eigenschap* kleur krijgt
 - de *waarde* rood
 - voor *alle* `<p>` onderdelen

Maar stel nou dat je alleen bepaalde alinea's rood wilt maken?

### Class

Dat kan bijvoorbeeld door het HTML-onderdeel lid te maken van een zogenaamde
*class*:

{{< highlight html >}}
  <p class="naamvandeclass">Welke kleur is dit?</p>
{{< /highlight >}}

In de CSS maak je een class door een *punt* aan het begin te gebruiken:

{{< highlight cs >}}
  .naamvandeclass {
    color: red;
  }
{{< /highlight >}}

**Opdracht** Gebruik een *class* met de naam "rodealinea" om de 1e en 4e alinea
rood te maken, dus zo:

{{< html_voorbeeld >}}
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
{{< /html_voorbeeld >}}

### ID

Een andere manier is om een HTML-onderdeel een uniek *id* te geven:

{{< highlight html >}}
  <p id="ikbenuniek">Welke kleur is dit?</p>
{{< /highlight >}}

In de CSS verwijs je naar een id door een *hashtag* aan het begin te gebruiken:

{{< highlight css >}}
  #ikbenuniek {
    color: red;
  }
{{< /highlight >}}

**Opdracht** Maak de tekst van de eerste h1 kop blauw, en de 1e h2 kop groen
(tip: je hebt hiervoor twee id's nodig, "ikbenblauw" en "ikbengroen"):

{{< html_voorbeeld >}}
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
{{< /html_voorbeeld >}}

Samengevat heb je nu gezien dat je stijl kunt geven aan

 - alle onderdelen van een bepaalde soort
 - bepaalde onderdelen door ze lid te maken van een class
 - losse onderdelen door ze een (uniek) id te geven

### Combineren van stijlen

Een grote kracht van CSS is dat je stijlen ook kunt combineren. Zo kun je
meerdere eigenschappen tegelijk instellen in een CSS regel:

{{< highlight css >}}
  p {
    color: red;
    font-weight: bold;
  }
{{< /highlight >}}

**Opdracht** Voeg een tweede eigenschap toe aan de "rodealinea", bijvoorbeeld
*background-color* of *font-family*.

Je kunt een onderdeel ook lid maken van meer dan één *class* (in dit voorbeeld
heten die "rodealinea" en "box"):

{{< highlight html >}}
  <p class="rodealinea box"
{{< /highlight >}}

**Opdracht** Maak een class "box" die de eigenschap `border` instelt op `1px
solid black`, en voeg deze toe aan een van de rode alinea's:

{{< html_voorbeeld >}}
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
{{< /html_voorbeeld >}}

## Actie toevoegen met JavaScript (vervolg)

Nu je de basis van JS hebt gezien, gaan we wat verder met moeilijker
onderdelen.

### Een klok maken

![klok](imgs/clock.png)

We gaan een klok maken op een `HTML` pagina. Je kan de volgende `HTML`
gebruiken:

{{< highlight html >}}
    <html>
    <head>
        <style>
            body {
                background: linear-gradient(45deg, #1870ed 0, #f18f88 100%);
                font-family: 'Montserrat', 'sans-serif';
                min-height: 100vh;
                display: flex;
                align-items: center;
                justify-content: center;
            }

            .clock-container {
                margin-top: 30px;
                margin-bottom: 30px;
                background-color: #080808;
                border-radius: 5px;
                padding: 60px 20px;
                box-shadow: 1px 1px 5px rgba(255, 255, 255, .15), 0 15px 90px 30px rgba(0, 0, 0, .25);
                display: flex;
            }

            .clock-col {
                text-align: center;
                margin-right: 40px;
                margin-left: 40px;
                min-width: 90px;
                position: relative;
            }

            .clock-col:not(:last-child):before,
            .clock-col:not(:last-child):after {
                content: "";
                background-color: rgba(201, 166, 166, 0.3);
                height: 5px;
                width: 5px;
                border-radius: 50%;
                display: block;
                position: absolute;
                right: -42px;
            }

            .clock-col:not(:last-child):before {
                top: 35%;
            }

            .clock-col:not(:last-child):after {
                top: 50%;
            }

            .clock-timer {
                color: #fff;
                font-size: 4.2rem;
                text-transform: uppercase;
            }

            .clock-label {
                color: rgba(255, 255, 255, .35);
                text-transform: uppercase;
                font-size: 0.7rem;
                margin-top: 10px;
            }

            @media (max-width: 825px) {
                .clock-container {
                    flex-direction: column;
                    padding-top: 40px;
                    padding-bottom: 40px;
                }

                .clock-col+.clock-col {
                    margin-top: 20px;
                }

                .clock-col:before,
                .clock-col:after {
                    display: none !important;
                }
            }
        </style>
    </head>

    <body>
        <div class="clock-container">
            <div class="clock-col">
                <p class="clock-hours clock-timer" id="clock-day">
                </p>
                <p class="clock-label">
                    Dag
                </p>
            </div>
            <div class="clock-col">
                <p class="clock-hours clock-timer" id="clock-hour">
                </p>
                <p class="clock-label">
                    Uren
                </p>
            </div>
            <div class="clock-col">
                <p class="clock-minutes clock-timer" id="clock-minute">
                </p>
                <p class="clock-label">
                    Minuten
                </p>
            </div>
            <div class="clock-col">
                <p class="clock-seconds clock-timer" id="clock-second">
                </p>
                <p class="clock-label">
                    Seconden
                </p>
            </div>
        </div>

        <script>
            //Hier moet jij je code gaan schrijven voor de clock!

            let dagElement = document.getElementById("clock-day");
            let urenElement = document.getElementById("clock-hour");
            let minutenElement = document.getElementById("clock-minute");
            let secondenElement = document.getElementById("clock-second");

            const dagenInText = ["Zo", "Ma", "Di", "Wo", "Do", "Vr", "Za"];

            function updateTime() {
                var today = new Date(); //Dit geeft je een datum terug,
                                        //hier kun je de uren, minuten en seconden van halen.
                                        //Met getHours() krijg je de uren
                                        //Met getMinutes() krijg je de minuten
                                        //Met getSeconds() krijg je de seconden

                                        //De dag hebben wij voor je gedaan!
                dagElement.innerText = dagenInText[today.getDay()];
                urenElement.innerText = "1";
                minutenElement.innerText = "1";
                secondenElement.innerText = "1";
            }

            //Dit voert de functie iedere seconde opnieuw uit,
            //De tijd gaat natuurlijk met 1 seconde per keer vooruit!
            setInterval(updateTime, 1000);

        </script>
    </body>

    </html>
{{< /highlight >}}

De klok werkt nu nog niet.. Kan jij dit oplossen? In het `<script></script>`
blok moet jij de code gaan aanpassen, daarmee kun je de klok weer aanslingeren
;) !

## Het instellen van kleuren op je webpagina

Er zijn een een heel aantal manieren om een kleur in te stellen voor onderdelen
van je pagina, bijvoorbeeld

 - met `namen`_ `<p style="color:red">`
 - met `RGB-waarden`_ `<p style="color:rgb(255, 0, 0)">`
 - met `HEX-waarden`_ `<p style="color:#FF0000">`

### Namen

Er zijn 140 kleuren die een eigen naam hebben:

![kleur woorden](imgs/recognized_color_keyword_names.svg)

### RGB-waarden

RGB staat voor **R**ood **G**roen **B**lauw. Dit is ook de volgorde
waarmee je ze instelt in de code.  De waarde gaat van 0 (helemaal niks van
deze kleur) tot 255 (alles van deze kleur). Een paar voorbeelden:

| RGB code        | Rood  | Groen | Blauw | Kleur      |
|:---------------:|:-----:|:-----:|:-----:|:----------:|
| (0, 255, 0)     | 0     | 255   | 0     | groen      |
| (255, 0, 255)   | 255   | 0     | 255   | magenta    |
| (173, 216, 230) | 173   | 216   | 230   | lichtblauw |


### HEX-waarden

 - HEX is een afkorting voor hexadecimaal, wat een manier van tellen is die vaak
  wordt gebruikt bij computers.
 - In plaats van de 10 cijfers (0 t/m 9) waar we meestal mee tellen tel je hier
  met 16 "cijfers", namelijk 0 t/m 9 en A t/m F.
 - De HEX code voor een kleur is zes cijfers lang: de linker twee bepalen
  hoeveel rood er in de kleur zit, de middelste twee hoeveel groen en de
  rechter twee hoeveel blauw. 00 is de laagste waarde (omgerekend 0), FF is de
  hoogste waarde (omgerekend 255).
 - De zescijferige code staat in de HTML-code na een #.

De kleuren van de RGB-voorbeelden zijn in HEX code

| HEX code | Kleur      |
|:--------:|:----------:|
| 00FF00   | groen      |
| FF00FF   | magenta    |
| ADD8E6   | lichtblauw |

## Bronvermelding afbeeldingen
 - [HTML logo by W3C](https://commons.wikimedia.org/wiki/File:HTML5_logo_and_wordmark.svg)
 - [CSS logo by Rudloff](https://commons.wikimedia.org/wiki/File:CSS3_logo_and_wordmark.svg)
 - [JS logo by Omed Habib](https://commons.wikimedia.org/wiki/File:Javascript-shield.svg)
 - [SVG_Recognized_color_keyword_names by Monaneko](https://commons.wikimedia.org/wiki/File:SVG_Recognized_color_keyword_names.svg)

{{< licentie rel="http://creativecommons.org/licenses/by-nc-sa/4.0/">}}
