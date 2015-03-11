===================
SystemDetection
===================


Zusammenfassung
-------------------------

Dieses Modul zielt auf die Erkennung der Maschine des Benutzers und in der Hand stellt ihnen die notwendigen Informationen, um sie in Bezug auf die Benutzer-System. Es bietet auch eine Möglichkeit, die Benutzer ihre Anwendungen zu konfigurieren. Die wenigen Beispiele für Anwendungen, Einstellungen gehören MySQL Admin-Benutzer, Architektur, Admin-Benutzer, Host, Version, linux-Typ, Distro. Es ist bequem mit Ubuntu und Cent-OS.

Hilfe Befehl
---------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den System-Detektionsmodule enthalten sind. Der Befehl help Listen aus der alternativen Parameter der Systemerkennung unter pttest Modul. Es beschreibt auch die Syntax zum Erfassen theuser der Maschine. Der Befehl help zur Systemerkennung wird unten gezeigt.

.. code-block:: bash

	pttest systemdetection help

Die Syntax für die Hilfe Befehl ist nicht case sensitive, was ein Vorteil für dieses Modul erstellt. Der folgende Screenshot Visualisierung über das Hilfe-Befehl unter Systemerkennung.

.. code-block:: bash

 kevell@corp:/# pttest systemdetection help
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

entdecken
-----------

Wenn der Benutzer benötigt, um die Systemeinstellungen zu erkennen, wird die unten angegeben Befehls alle Informationen, die über das System Anwendung zu erhalten.

.. code-block:: bash
	
	pttest systemdetection detect

System endet mit Bereitstellung der unten angegebenen Details:

* Betriebssystem
* Linux Typ
* Distro
* Version
* Architektur
* Host-Name
* Die IP-Adresse 0.

Der folgende Screenshot zeigt Ihnen über den Prozess der Systemerkennung.

.. code-block:: bash

 kevell@corp:/# pttest system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 172.16.201.1
 IP Address 1: 172.16.39.1
 IP Address 2: 192.168.1.16

 ------------------------------
 Detection Finished
 ******************************

Alternative Parameter
----------------------------------

Statt System erkennen können die folgenden Parameter verwendet werden:

* SystemDetection
* system-detection
* systemdetection


Vorteile
-------------

* Die Benutzer können die Anwendungseinstellungen mit diesem System Erkennung konfigurieren.
* Die Hilfe Befehl deklarieren verwendeten Parameter werden Systemerkennung nicht beachtet, die einen zusätzlichen Vorteil, während im Vergleich   zu andere.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Schutz und Sicherheit möglich ist. Vermeiden von Schäden an der Anlage und zu Ressourcen, durch interne Prozesse oder böswillige Außenseiter.
  Authntication, Eigentum und Zugangsbeschränkungen sind offensichtlich Teile dieses Systems.
* Systemadministratoren in der Regel fest, welche Schnittstelle ein Benutzer mit, wenn sie zum ersten Mal eingeloggt beginnt.
* In der Regel in PHP geschrieben, obwohl einige sind in der Montage für eine optimale Leistung geschrieben.
