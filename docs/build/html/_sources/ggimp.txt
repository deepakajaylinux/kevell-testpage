=======
GIMP
=======


Zusammenfassung
-----------------------

Dieses Modul ermöglicht es Anwendern, GIMP, die ein beliebtes Bild-Editor zu installieren.

GIMP ein Akronym für GNU Image Manipulation Program) ist für die Bildretusche und Bearbeiten, Freiform-Zeichnung verwendet, Skalieren, Beschneiden, Fotomontagen, die Konvertierung zwischen verschiedenen Bildformaten und mehr spezialisierte Aufgaben.

GIMP ist frei (und nach) jeder verteilt, und jeder kann in ihrem Inhalt und ihrer Quellcode schauen und können Funktionen hinzufügen oder Probleme beheben. Es wird unter LGPLv3 und GPLv3 + Lizenzen freigegeben. GIMP begann 1995 als Schulprojekt von zwei Studenten; Jetzt GIMP ist eine vollwertige Anwendung, auf allen Distributionen von GNU / Linux und die jüngsten Versionen von Microsoft Windows und Mac OS X.

Lassen Sie uns sehen, wie dieses Modul erleichtert die Installation von GIMP aus den anstehenden Themen.


Hilfe Befehl
-------------------

Der Befehl help ist eine kurze Bedienungsanleitung, die die Benutzer über den Zweck dieses Moduls Die Listen outs sein alternatives Parameter, die in den Erklärungen für die Installation von GIMP durch verwendet werden kann, zusammen mit der Syntax Apt-get stellt. Die Syntax für die Hilfe-Option im Rahmen dieses Moduls ist unten dargestellt,

.. code-block:: bash

	ptconfigure GIMP help


Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter GIMP.


Installation
--------------

Der Befehl für die Installation von GIMP durch verwendet apt-get mit diesem Modul ist einfach nur mit Hilfe von unter dem Befehl,

.. code-block:: bash

	ptconfigure GIMP install

Nach der Eingabe des Befehls vor, werden die folgenden Schritte, wie in der Tabelle dargestellt, durchgeführt,

.. cssclass:: table-bordered

 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+
 | Parameters          | Alternative Parameters               | Options      | Kommentar                                               |
 +=====================+======================================+==============+=========================================================+
 |GIMP Install? (Y/N)  | anstelle von GIMP wir verwenden      | Y(Yes)       | Wenn der Benutzer auf Wunsch Installation               |
 |                     | können, gimp also.                   |              | fortzusetzen, können sie Eingang als Y.                 |
 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+
 |GIMP Install? (Y/N)  | anstelle von GIMP wir verwenden      | N(No)        | Wenn der Benutzer wünschen, um die Installation         |
 |                     | können, gimp also.                   |              | zu beenden, können sie Eingang als N.|                  |
 +---------------------+--------------------------------------+--------------+---------------------------------------------------------+

Der folgende Screenshot zeigt visuell über den Prozess der Installation.


Vorteile
----------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von apt erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.


GIMP bietet auch "intelligente" Werkzeuge, die einen komplexeren Algorithmus verwenden, um Dinge, die sonst zeitaufwändig oder unmöglich machen. Dazu zählen ein:

* Klonen-Werkzeug, das Kopien Pixel mit einem Pinsel
* Reparatur-Pinsel, die Kopien Pixel aus einem Bereich und Ton und Farbe korrigiert
* Perspective Klon-Werkzeug, das wie das Klon-Werkzeug funktioniert, aber korrigiert Abstandsänderungen
* Unschärfe und schärfen Werkzeug Unschärfen und schärft mit einem Pinsel
* Dodge und Burn-Tool ist ein Pinsel, der Zielbildpunkte heller (Winkelzüge) oder dunkler (Verbrennungen) macht


GIMP verwandeln Tools gehören:

* Richten
* Sich Bewegen
* Crop
* Drehen
* Skala
* Shear
* Perspective
* Flip

