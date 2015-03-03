===========
PTTest 
===========

Zusammenfassung
----------------------

pttest Modul ist für den Umgang mit Test-Suite-Konfiguration und Ausführung mit einem gemeinsamen Satz von Regeln für eine Reihe von Tools und Technologien. Es kann benutzt werden, um Start Test-Suiten für Ihre Anwendungen zu erzeugen, und die automatisierte Testdurchführung Skripte innerhalb weniger Minuten.

Dieses Modul soll die Installation der neuesten Version von pttest Werkzeug.

Hilfe Befehl
---------------

Der Befehl help führt den Anwender zur Verfügung zu stellen, was notwendig ist, um die Aufgabe zu erfüllen. Der Befehl zum Einsatz von dazu beitragen, dass im Rahmen der Terminal wird wie folgt angegeben,

.. code-block:: bash

	ptconfigure pttest help

Die nachfolgende Snapshots gibt Ihnen eine bildliche Darstellung der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest help
 ******************************


  This command allows you to update pttest.

  pttest, cleo, pttest

        - install
        Installs the latest version of pttest
        example: pttest pttest install

 ------------------------------
 End Help
 ******************************

Installation
-------------

Der bevorzugte Weg, um eine der Pharao Apps installieren, ist durch ptconfigure. Wenn Sie bereits installiert ptconfigure dann können Sie pttest mit dem folgenden Befehl installiert werden,

.. code-block:: bash

	ptconfigure pttest install

Die nachfolgende Snapshots gibt Ihnen eine bildliche Darstellung der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest install
 Install pttest - Update to latest version ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          pttest!         *
 *******************************
 What is the program data directory? Found "/opt/pttest" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/pttest.git'  /tmp/pttest/pttestCloning into '/tmp/pttest/pttest'...
 remote: Counting objects: 909, done.
 remote: Total 909 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (909/909), 361.15 KiB | 87.00 KiB/s, done.
 Resolving deltas: 100% (412/412), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 pttest: Success
 ------------------------------
 Installer Finished
 ******************************

Options
------------

.. cssclass:: table-bordered

 +---------------------+--------------------+----------------------------------------------------------------------+
 | Paramaters          | Erforderliche      | Kommentare                                                           |
 +=====================+====================+======================================================================+
 |ptconfigure pttest   | Yes                | Dieser Befehl wird die pttest Module installiert                     |
 |install              |                    |                                                                      |
 +---------------------+--------------------+----------------------------------------------------------------------+
 |Install pttest?      | Y                  | Wenn der Benutzer gibt Y, dieses Modul prüft zuvor installierte      |
 |( Y/N)               |                    | Version, wenn Ausfahrten wurde auf die neueste Version aktualisiert  |
 |                     |                    | oder er die frische Paket installiert. Um die Programmdateien auf    |
 |                     |                    | den bestimmten Pfad Benutzer zu speichern müssen Schlüsseltaste "/"  |
 |                     |                    | eingeben oder es den Standardpfad wie in der Abbildung verwendet.    |
 +---------------------+--------------------+----------------------------------------------------------------------+
 |Install pttest?      | N                  | Wenn der Benutzer eingibt N wurde die Installation abgebrochen.      |
 |( Y/N)|              |                    |                                                                      |
 +---------------------+--------------------+----------------------------------------------------------------------+



Vorteile für die Nutzer
----------------------------

* Einfache Anwendung von Zugangs- und Installation
* Coding wird nicht beachtet
* Full Quelle verfügbar ist und es gibt keine Lizenzkosten.

