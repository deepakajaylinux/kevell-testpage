======================
System Detection
======================

Zusammenfassung
-----------------

Dieses Modul zielt auf dem Computer des Benutzers zu erkennen und in der hand bietet ihnen die nötigen Informationen für sie das Benutzer-System. Darüber hinaus eine Anlage an die Benutzer ihre Anwendungseinstellungen konfigurieren. Einige Beispiele für Anwendungseinstellungen enthält mein Sql Admin User, Architektur, Admin-Benutzer, Host, Version, Typ Linux Distribution. Es ist komfortabel mit Ubuntu und Cent OS.


Hilfe Befehl
-----------------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in den System-Erkennung-Modulen enthalten sind. Der Hilfebefehl listet die alternative Ausgabeparameter der Entdeckung unter Jrush Modul. Es beschreibt auch die Syntax für die Erkennung von dem Computer des Benutzers. Der Help-Befehl für Entdeckung ist unten dargestellt.


.. code-block:: bash

	jrush systemdetection help


Die Syntax für den Befehl Help nicht Groß-/Kleinschreibung beachtet, der einen Vorteil für dieses Modul hinzufügt. Der folgende Screenshot visualisieren den Benutzer über den Befehl Help unter Entdeckung.



.. code-block:: bash

 kevell@corp:/# jrush systemdetection help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This is a default Module and provides you with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

 ------------------------------
 End Help
 ****************************************

Detect
----------- 

Erkennen verwendet, um die Systemeinstellungen zu erkennen. Mithilfe eines einzelnen Befehls kann der Benutzer alle Informationen über die Systemanwendung erhalten.  Der Befehl zur Entdeckung ist unten angegeben.


.. code-block:: bash

	jrush systemdetection detect

Nach Eingabe des oben genannte Befehls, beginnt der Prozess der Entdeckung. Bei der Entdeckung sind der folgenden Informationen zu der entsprechenden Maschine berichtet:



* Operating System
* Linux Type
* Distro
* Version
* Architecture
* Host Name
* IP Address 0.
* IP Address 1.

Schließlich erwähnte nach ihrer Entdeckung die Informationen zu den oben genannten Funktionen deutlich gemeldet werden. Der folgende Screenshot zeigt Ihnen über den Prozess der Entdeckung.


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
 Host Name: udayakumar
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.24

 ------------------------------
 Detection Finished
 ******************************


Alternative Parameter
----------------------------------

Statt Entdeckung können die folgenden Parameter verwendet werden:


* System Detection
* system-detection
* system detection

Vorteile
-------------

* Die Benutzer können die Anwendungseinstellungen verwenden dieses System-Erkennungen konfigurieren. 
* Die Parameter für das Deklarieren von Help-Befehl, Entdeckung Groß-‘ /Kleinschreibung kein zusätzlichen Vorteil, während im Vergleich zu 
  anderen ist. 
* Es ist wohlhabenden in beiden Cent OS und so gut wie Ubuntu. 
* Schutz und Sicherheit ist möglich. Verhindert Schaden auf das System und Mittel, durch interne Prozesse oder böswillige Außenseiter.  
  Authentifizierung, Besitz und Zugangsbeschränkungen sind offensichtlich Teile dieses Systems. 
* System-Administratoren im Allgemeinen bestimmen, welche Schnittstelle ein Benutzer beginnt mit beim ersten Zoll Anmeldung 
* im Allgemeinen in PHP geschrieben, obwohl einige in Assembly für eine optimale Leistung geschrieben sind.



Das System-Detection-Modul unterstützt:


* Identifizieren Sie einen Remoteprozess bzw. Host mit denen zu kommunizieren. 
* Stellen Sie eine Verbindung zwischen zwei Prozessen. 
* Öffnen Sie und schließen Sie die Verbindung nach Bedarf. 
* Überträgt Nachrichten entlang der Verbindung.


  


