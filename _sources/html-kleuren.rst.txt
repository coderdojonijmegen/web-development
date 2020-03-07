.. _html-kleuren:

Het instellen van kleuren op je webpagina
#########################################

Er zijn een een heel aantal manieren om een kleur in te stellen voor onderdelen
van je pagina, bijvoorbeeld

* met `namen`_ ``<p style="color:red">``
* met `RGB-waarden`_ ``<p style="color:rgb(255, 0, 0)">``
* met `HEX-waarden`_ ``<p style="color:#FF0000">``

Namen
*****

Er zijn 140 kleuren die een eigen naam hebben:

.. image:: imgs/recognized_color_keyword_names.svg
   :height: 250px


RGB-waarden
***********

RGB staat voor **R**\ ood **G**\ roen **B**\ lauw. Dit is ook de volgorde
waarmee je ze instelt in de code.  De waarde gaat van 0 (helemaal niks van
deze kleur) tot 255 (alles van deze kleur). Een paar voorbeelden:

+-----------------+-------+-------+-------+------------+
| RGB code        | Rood  | Groen | Blauw | Kleur      |
+=================+=======+=======+=======+============+
| (0, 255, 0)     | 0     | 255   | 0     | groen      |
+-----------------+-------+-------+-------+------------+
| (255, 0, 255)   | 255   | 0     | 255   | magenta    |
+-----------------+-------+-------+-------+------------+
| (173, 216, 230) | 173   | 216   | 230   | lichtblauw |
+-----------------+-------+-------+-------+------------+


HEX-waarden
***********

* HEX is een afkorting voor hexadecimaal, wat een manier van tellen is die vaak
  wordt gebruikt bij computers.
* In plaats van de 10 cijfers (0 t/m 9) waar we meestal mee tellen tel je hier
  met 16 "cijfers", namelijk 0 t/m 9 en A t/m F.
* De HEX code voor een kleur is zes cijfers lang: de linker twee bepalen
  hoeveel rood er in de kleur zit, de middelste twee hoeveel groen en de
  rechter twee hoeveel blauw. 00 is de laagste waarde (omgerekend 0), FF is de
  hoogste waarde (omgerekend 255).
* De zescijferige code staat in de HTML-code na een #.

De kleuren van de RGB-voorbeelden zijn in HEX code

+----------+------------+
| HEX code | Kleur      |
+==========+============+
| 00FF00   | groen      |
+----------+------------+
| FF00FF   | magenta    |
+----------+------------+
| ADD8E6   | lichtblauw |
+----------+------------+

|

Bronvermelding afbeelding:
`SVG_Recognized_color_keyword_names by Monaneko <https://commons.wikimedia.org/wiki/File:SVG_Recognized_color_keyword_names.svg>`_
