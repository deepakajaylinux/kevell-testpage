=================
PTBuild
=================

Zusammenfassung
----------------------

Dieses Tool hilft dem Benutzer, unter ptconfigure in Pharao Tools zu installieren und zu aktualisieren ptbuild. Automatisierung des Build sollte auch die Automatisierung der Integration, die häufig Einsatz in einer produktionsähnlichen Umgebung. In vielen Fällen ist die Build-Skript nicht nur kompiliert Binärdateien, sondern erzeugt auch Dokumentation, Webseiten, Statistiken und Vertriebsmedien wie Red Hat. Es tröstet mit Ubuntu und Cent OS.

Hilfe Befehl
-----------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in den ptbuild Module enthalten sind. Der Befehl help Listen aus der alternativen Parameter ptbuild unter ptconfigure Modul. Es beschreibt auch die Syntax für die Installation updation des Benutzers. Der Befehl help für ptbuild ist nachfolgend dargestellt.

.. code-block:: bash

 		ptconfigure ptbuild help


Der folgende Screenshot zeigt den vollen Einsatz der ptbuild.

.. code-block:: bash

 kevell@corp:/# ptconfigure ptbuild help

 ******************************


  This command allows you to install or update ptbuild.

  ptbuild, ptbuild

        - install
        Installs the latest version of ptbuild
        example: ptconfigure ptbuild install

        - ensure
        Ensures ptbuild is installed
        example: ptconfigure ptbuild ensure

        - uninstall
        Uninstalls the latest version of ptbuild
        example: ptconfigure ptbuild uninstall
 ------------------------------
 End Help
 ******************************

Installation
--------------------

Dies ist ein Werkzeug, das unter ptconfigure sitzt und zieht saubere Kopien der Benutzercodebasis und hat volle baut, aus dem Nichts, die ganze Zeit. Dieser Befehl wird verwendet, um neueste Version von ptbuild installieren. Der Befehl für den Einbau verwendet wird, ist wie folgt.

.. code-block:: bash

	ptconfigure ptbuild install

Nach Den Befehl das System an ist

Install ptbuild?(Y/N)

Wenn der Benutzer gibt dann Y ptbuild installiert. Der folgende Screenshot zeigen es.

.. code-block:: bash


.. cssclass:: table-bordered

 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 | Parameters                | Verzeichnis (default)  | Optionen                  | Kommentare                                          |
 +===========================+========================+===========================+=====================================================+
 |Data directory (Default)   | Yes                    | “/opt/ptbuild”            | Es wird ptbuild unter ptconfigure installieren      |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Data directory             | No                     | End Schrägstrich          | Der Benutzer muss ein den Pfad                      |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Executor directory         | Yes                    | “/usr/bin”                | Es wird Testamentsvollstrecker Verzeichnis          | 
 |(Default)                  |                        |                           | installieren                                        |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Executor directory         | No                     | No Schrägstrich           | Der Nutzer ist damit Eingang als Verzeichnisname.|  |  
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+

Uninstall
--------------

Dieser Befehl wird verwendet, um die neueste Version von ptbuild Deinstallieren. Der Befehl für die Deinstallation verwendet wird, ist wie folgt.

.. code-block:: bash

		ptconfigure ptbuild Uninstall

Nach Den Befehl das System an ist

Uninstall ptbuild?(Y/N)

Wenn der Benutzer gibt dann Y ptbuild wird deinstalliert. Der folgende Screenshot zeigen es.

.. code-block:: bash


.. cssclass:: table-bordered

 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 | Parameters                | Verzeichnis (default)  | Optionen                  | Kommentare                                          |
 +===========================+========================+===========================+=====================================================+
 |Data directory (Default)   | Yes                    | “/opt/ptbuild”            | es wird uninstall ptbuild unter ptconfigure         |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Data directory             | No                     | End Schrägstrich          | Der Benutzer muss ein den Pfad                      |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Executor directory         | Yes                    | “/usr/bin”                | es wird uninstall Vollstrecker-Verzeichnis          | 
 |(Default)                  |                        |                           |                                                     |
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+
 |Executor directory         | No                     | No Schrägstrich           | Der Nutzer ist damit Eingang als Verzeichnisname.|  |  
 +---------------------------+------------------------+---------------------------+-----------------------------------------------------+


Dafür Sorgen
----------------

Stellen Sie sicher, Prozess verwendet, um die ptbuild im Benutzersystem oder nicht installiert zu überprüfen. Der folgende Befehl hilft dem Anwender, zu gewährleisten.

.. code-block:: bash

		ptconfigure ptbuild ensure

Der folgende Screenshot zeigt seine Funktionen.
Vorteile
----------------

* Wird möglich installieren ptbuilds.
* Geeignet, um mit Ubuntu und CentOS arbeiten.
* Nicht Groß- und Kleinschreibung.
* Automation in aktualisierte Version.
* Zuverlässigkeit, Verfügbarkeit, Wartungsfreundlichkeit mit anderen Verbindungen.


