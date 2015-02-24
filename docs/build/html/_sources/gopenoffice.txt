============
OpenOffice
============

Zusammenfassung
----------------------

Dieses Modul fungiert als Vermittler für die Installation Openoffice .Open-Büro ist die erste offene Suite von Office-bezogene Software. Wir wollen sehen, die Verwendung und Methoden der Installation von Open Office in kommenden Themen.

Hilfe Befehl
----------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Open Office-Modul enthalten sind. Es listet einige der alternativen Parameter der Open Office-Modul. Es beschreibt auch die Syntax für die Installation des Open Office-Modul. Der Befehl help für Open Office Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure OpenOffice help


Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Open Office.

.. code-block:: bash

 kevell@corp:/# ptconfigure openoffice help

 ******************************


  This command allows you to install OpenOffice.

  OpenOffice,openoffice,Openoffice

        - install
        Installs OpenOffice.
        example: ptconfigure openoffice install

 ------------------------------
 End Help
 ******************************

Installation
--------------

Der Befehl für die Installation des Open Office in der Benutzer-Maschine verwendet wird, wie folgt dar:

.. code-block:: bash

		ptconfigure openoffice install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +----------------------------+-------------------------------------------+------------+-----------------------------------------+
 | Parameter                  | Alternative Parameter                     | Option     | Kommentare                              |
 +============================+===========================================+============+=========================================+
 |Install Open Office? (Y/N)  | anstelle von openoffice, wir verwenden    | Y(Yes)     | Wenn der Benutzer wünschen, den         |
 |                            | können, OpenOffice, Openoffice also.      |            | Installationsprozess können sie Eingang |
 |                            |                                           |            | als Y. gehen                            |
 +----------------------------+-------------------------------------------+------------+-----------------------------------------+
 |Install Open Office? (Y/N)  | anstelle von openoffice, wir verwenden    | N(No)      | Wenn der Benutzer wünschen, den         |
 |                            | können, OpenOffice, Openoffice also.      |            | Installationsprozess können sie Eingang |
 |                            |                                           |            | als N. beenden|                         |
 +----------------------------+-------------------------------------------+------------+-----------------------------------------+


Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:

* Liest Paketlisten.
* Erstellt die Abhängigkeitsstruktur.
* Liest Statusinformationen.
* Liste outs die Pakete, die automatisch installiert werden.
* Liste outs das zusätzliche Paket installieren.
* Liste outs die vorgeschlagenen Pakete.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Schließlich ist der Prozess der Installation abgeschlossen wird. Der folgende Screenshot visuell darstellen, den Prozess der Installation des offenen Büro.

.. code-block:: bash

Vorteile
----------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die php apc in aktualisierte Version.
* Der Hauptvorteil der Verwendung von Apache Openoffice als Produktivitäts-Suite kommt von den Kosten. Es beinhaltet Textverarbeitung, Tabellenk  alkulation, Präsentationen, ein Vektorgrafikbearbeitung und Datenbank-Management-Komponenten.
* Es ist einfach für Anfänger zu lernen, zu verwenden, aber es leistungsfähig genug, um die erweiterten Aufgaben erfahrene Anwender wollen zu 
  tun ist. Es ist so konzipiert, dass die Befehle und Funktionen, die Sie in eine Komponente der Software Arbeitsleistung während der gesamten 
  Suite.


