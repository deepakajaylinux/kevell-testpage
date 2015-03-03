==================
System Detection
==================

Zusammenfassung
----------------------

Dieses Modul soll Erfassung der Benutzer-Maschine und in der Hand stellt ihnen die notwendigen Informationen, um sie in Bezug auf die Benutzer-System. Es bietet auch eine Möglichkeit, die Benutzer ihre Anwendungen zu konfigurieren. Die wenigen Beispiele für Anwendungen, Einstellungen enthält MySQL Admin-Benutzer, Host weiter.

Hilfe Befehl
----------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den System-Detektionsmodule enthalten sind. Der Befehl help Listen aus der alternativen Parameter der Systemerkennung. Es beschreibt auch die Syntax zum Detektieren des Nutzer-Maschine. Der Befehl help zur Systemerkennung wird unten gezeigt.

.. code-block:: bash

	ptconfigure systemdetection help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Systemerkennung.

.. code-block:: bash

	kevell@corp:/# ptconfigure SystemDetection help
	******************************


	This is a default Module and provides you with a method by which you can configure Application Settings.
	 You can configure default application settings, ie: mysql admin user, host, pass

	 SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

	------------------------------
	End Help
	******************************

Entdeckung
---------------

Der Befehl für die Systemerkennung verwendet wird unten gegeben.

.. code-block:: bash

		ptconfigure systemdetection detect

Nach der Eingabe des Befehls vor, den Prozess der Systemerkennung beginnt. Während des Systemerkennung die folgenden Informationen betreffend der entsprechenden Maschine gemeldet:

* Betriebssystem
* Linux Typ
* Distro
* Version
* Architektur
* Host-Name
* Die IP-Adresse 0.
* IP-Adresse ein.

Schließlich Nach Erfassung der Informationen zu den oben genannten Funktionen sind klar ausgewiesen. Der folgende Screenshot zeigt Ihnen über den Prozess der Systemerkennung.

Alternative Parameters
------------------------

Instead of systemdetection, the following parameters can be used:

* SystemDetection
* system-detection

Vorteile
------------

* Die Benutzer können die Anwendungseinstellungen mit diesem System Erkennungen konfigurieren.
* Die Hilfe Befehl deklarieren verwendeten Parameter werden Systemerkennung nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu andere.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.


