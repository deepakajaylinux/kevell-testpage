==========
Grafana
==========


Zusammenfassung
-----------------------

Grafana verfügt über eine erweiterte Graphit Abfrage-Editor, die Sie schnell den metrischen Raum navigieren können, fügen Sie Funktionen. Ändern Funktion Paramater und vieles mehr.

Grafana ist ein Open Source, funktionsreichen Metriken Armaturenbrett und Grafik-Editor für Graphit, InfluxDB & OpenTSDB.

Wir wollen sehen, wie dieses Modul ermöglicht den Benutzern bei der Installation der grafana.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Grafana Modul enthalten sind. Es listet einige der alternativen Parameter Grafana Modul. Es beschreibt auch die Syntax für die Installation des Grafana Moduls. Der Befehl help für Grafana Modul wird wie unten dargestellt.

.. code-block:: bash

	ptdeploy grafana help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Grafana Modul.

Installation
--------------


Der Befehl zum Installieren der grafana Module im Benutzer-Maschine verwendet wird unten dargestellt:

.. code-block:: bash
	
	ptdeploy grafana install


Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +------------------------------+------------------------------------+---------+--------------------------------------------------------+
 | Parameters                   | Alternative Parameters             | Options | Kommentare                                             | 
 +==============================+====================================+=========+========================================================+
 |Install Grafana? (Y/N)        | Statt Grafana können wir           | Y(Yes)  | Wenn der Benutzer wünschen, den Installationsprozess   |
 |                              | grafana auch.                      |         | können sie Eingang als Y. gehen                        |
 +------------------------------+------------------------------------+---------+--------------------------------------------------------+
 |Install Grafana? (Y/N)        | Statt Grafana können wir           | N(No)   | Wenn der Benutzer wünschen, den Installationsprozess   |
 |                              | grafana auch.                      |         | können sie Eingang als N. beenden|                     |
 +------------------------------+------------------------------------+---------+--------------------------------------------------------+


Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.


Vorteile
----------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.


Graphite Target Editor
----------------------

* Graphite Ziel Ausdruck Parser
* Feature reichen Abfrage Komponist
* Schnelles Hinzufügen und Bearbeiten von Funktionen und Parameter
* Templated Anfragen
* In Aktion sehen

Grafische Darstellung
-----------

* Schnelle Wiedergabe, auch über große Zeitspannen.
* Klicken und ziehen, um Zoom.
* Mehrere Y-Achse.
* Bars, Linien, Punkte.
* Smart-Y-Achse Formatierung
* Serie Knebel & Farbauswahl
* Legende Werte und Formatierung Optionen
* Grid Schwellen, Achsenbeschriftungen
* Anmerkungen


Dashboards
-----------

* Erstellen, bearbeiten, speichern und suchen Dashboards
* Spalte ändern Spannweiten und Zeilenhöhen
* Drag & Drop-Panels neu anordnen
* Verwenden Sie InfluxDB oder Elasticsearch als Dashboard Speicher
* Import & Export-Dashboard (JSON-Datei)
* Import Armaturenbrett aus Graphit
* Templating
* Scripted Dashboards
* Armaturenbrett Wiedergabelisten
* Zeitbereich steuert

