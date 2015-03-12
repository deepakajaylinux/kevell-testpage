======================
System Detection
======================

Zusammenfassung
-----------------------

Dieses Modul zielt auf die Erkennung der Maschine des Benutzers und in der Hand stellt ihnen die notwendigen Informationen, um sie in Bezug auf die Benutzer-System. Es bietet auch eine Möglichkeit, die Benutzer ihre Anwendungen zu konfigurieren. Die wenigen Beispiele für Anwendungen, Einstellungen enthält meine SQL Admin-Benutzer, Architektur, Admin-Benutzer, Host, Version, linux-Typ, Distro. Es ist bequem mit Ubuntu und Cent-OS.

Hilfe Befehl
--------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den System-Detektionsmodule enthalten sind. Der Befehl help Listen aus der alternativen Parameter der Systemerkennung unter ptdeploy Modul. Es beschreibt auch die Syntax zum Nachweis von dem Computer des Benutzers. Der Befehl help zur Systemerkennung wird unten gezeigt.

.. code-block:: bash

	ptdeploy systemdetection help

Die Syntax für den Befehl help non-und Kleinschreibung, die einen Vorteil für das Modul erstellt. Der folgende Screenshot den Benutzer über den Befehl help unter Systemerkennung zu visualisieren.

.. code-block:: bash

 kevell@corp:/# ptdeploy systemdetection help
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

Erkennung verwendet werden, um die Systemeinstellungen zu erkennen. Durch die Verwendung eines einzigen Befehl kann der Benutzer alle Informationen, die über das System Anwendung zu erhalten.
Der Befehl für die Systemerkennung verwendet wird unten gegeben.

.. code-block:: bash

	ptconfigure systemdetection detect

Nach der Eingabe der oben genannten Befehl, den Prozess der Systemerkennung beginnt. Während des Systemerkennung die folgenden Informationen betreffend der entsprechenden Maschine gemeldet:

* Operating System
* Linux Type
* Distro
* Version
* Architecture
* Host Name
* IP Address 0.
* IP Address 1.

Endlich, nach Erkennung der Informationen zu den oben genannten Funktionen sind klar ausgewiesen. Der folgende Screenshot zeigt Ihnen über den Prozess der Systemerkennung.

.. code-block:: bash

 kevell@corp:/# ptconfigure system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: Kevells
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.18

 ------------------------------
 Detection Finished
 ******************************



Alternative Parameter
----------------------------------

Statt System erkennen können die folgenden Parameter verwendet werden:

* System Detection
* system-detection
* system detection

Vorteile
-------------

* Die Benutzer können die Anwendungseinstellungen mit diesem System Erkennungen konfigurieren.
* Die Hilfe Befehl deklarieren verwendeten Parameter werden Systemerkennung nicht beachtet, die einen zusätzlichen Vorteil, während im Vergleich  zu andere.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Nicht Groß- und Kleinschreibung.
* Schutz und Sicherheit möglich ist. Vermeiden von Schäden an der Anlage und zu Ressourcen, durch interne Prozesse oder böswillige Außenseiter.
  Authentifizierung, Eigentum und eingeschränktem Zugang sind offensichtlich Teile dieses Systems.
* Systemadministratoren in der Regel fest, welche Schnittstelle ein Benutzer mit, wenn sie zum ersten Mal eingeloggt beginnt.
* In der Regel in PHP geschrieben, obwohl einige sind in der Montage für eine optimale Leistung geschrieben.

Das System Erfassungsmodul bietet die Unterstützung:

* Identifizieren Sie eine Remote-Verfahren und / oder Host, mit denen zu kommunizieren.
* Stellen Sie die Verbindung zwischen den beiden Prozessen.
* Öffnen und schließen Sie die Verbindung je nach Bedarf.
* Übertragen Sie Nachrichten auf der Verbindung.

