=========
Logging
=========

Zusammenfassung
------------------------

Dieses Modul protokolliert eine Information an das Bedienfeld und optional php Protokoll.

Der Prozess der mit diesem Modul, um Daten über Sensoren zu sammeln, die Daten zu analysieren und speichern und Ausgabe der Ergebnisse der Erhebung und Analyse. Protokollierung impliziert auch die Controlpanel der das System installiert und analysiert die Daten. Nicht Groß- und Kleinschreibung ist eine Krone für dieses Modul. Das passt mit Ubuntu und Cent-OS arbeiten.

Hilfe Befehl
-----------------------

Dieser Befehl kann über die Ziele und Befehle in Logging unter Ptconfigure  Modul funktionieren. Es erklärt auch den Befehl, um die Protokollierung Module installiert. Vor der Installation kann der Benutzer lesen diese Hilfe Befehl erklärt seine Funktion.

.. code-block:: bash
        
	        ptconfigure  logging help

Die folgenden Screenshots können Sie den Befehl help visualisieren

.. code-block:: bash


 kevell@corp:/# ptconfigure  Logging help

 ******************************


  Use this to log a message to the Console, and optionally also the php error log.

  Logging, logging

        - log
        Logs a message to the console and optionally the php log
        example: ptconfigure  logging log --log-message="Here is something logging to the console and error log"
        example: ptconfigure  logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************

Installation
-----------------

Diese Installationsverfahren sind für die Steuerung php Protokoll. Dieser Abschnitt enthält Informationen über die Kompatibilität und Anforderungen, grundlegende Anweisungen zur Installation und Konfiguration von Kleopatra, um detailliertere Informationen. Dieser Befehl kann über die Ziele und Befehle unter Ptconfigure  Logging-Modul funktionieren. Es erklärt auch den Befehl, um die Protokollierung Module installiert. Vor der Installation kann der Benutzer lesen diese Hilfe Befehl erklärt seine Funktion.

.. code-block:: bash
        
                ptconfigure  logging  log

Die folgenden Screenshots können Sie den Befehl help visualisieren

.. code-block:: bash

 kevell@corp:/# ptconfigure  logging log 

 Install Logging? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Logging: Success
 ------------------------------
 Installer Finished
 ******************************

Optionen 
------------

.. cssclass:: table-bordered


 +-----------------------------+--------------------------------------+-------------+----------------------------------------------------+
 | Parameter                   |  Alternative Parameter               | Optionen    | Kommentare                                         |
 +=============================+======================================+=============+====================================================+
 |ptconfigure logging Install  | Wir verwenden Logging, logging       | Y           | System startet log process under ptconfigure       |
 +-----------------------------+--------------------------------------+-------------+----------------------------------------------------+
 |ptconfigure  logging Install | Wir verwenden Logging, logging       | N           | System-Haltestellen log process under ptconfigure| |
 +-----------------------------+--------------------------------------+-------------+----------------------------------------------------+



Vorteile
-------------

* Echtzeit-Daten-Visualisierung
* Nicht Groß- und Kleinschreibung
* Benutzerdefinierte Funktionen
* Terabyte Datenspeicher
* Network Connectivity
* Gut in Ubuntu und Cent-OS zu tun

