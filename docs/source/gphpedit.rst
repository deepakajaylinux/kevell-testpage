=========
PHPEdit  
=========

Zusammenfassung
-----------------------

PHPEdit-Modul ist eine komplette integrierte Entwicklungsumgebung für PHP. Viel mehr als ein einfaches PHP zu bearbeiten, zu dem Benutzer hilft es für die Durchführung ihrer Projekte in einem freundlichen und effizienten Art und Weise, mit einem einzigen Werkzeug die Integration aller Funktionen wird der Benutzer von der Gestaltung ihrer Projekte, deren Dokumentation benötigen, um ihren Einsatz. Es eignen mit Ubuntu und CentOS.

Hilfe Befehl
-----------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der PHPEdit Modul enthalten sind. Es listet einige der alternativen Parameter PHPEdit-Modul. Es beschreibt auch die Syntax für die Installation des phpedit Moduls. Der Befehl help für PHPEdit Modul wird wie unten dargestellt.

.. code-block:: bash

		ptconfigure Phpedit help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHPEdit.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPEdit help

 ******************************


  This command allows you to update PHPEdit.

  PHP-Edit, phpedit, PHPEdit

        - install
        Installs the latest version of PHPEdit
        example: ptconfigure phpedit install

 ------------------------------
 End Help
 ******************************

Installation
----------------

PHPEdit kommt mit einer Menge von Erweiterungen, Frameworks, Hilfedateien und Tools, so dass es in einem Installationsprogramm, die Anzüge angepasst werden kann der Benutzer needs.However ausgeliefert wird, da PHPEdit entwickelt sich ständig weiter, mit neuen Funktionen und Wartungskorrekturen , ein Auto-Update System ist ebenfalls verfügbar, um Schritt zu halten mit den neuesten Versionen PHPEdit mühelos. der Befehl für die Installation des Moduls wie folgt verwendet,

.. code-block:: bash

		ptconfigure Phpedit install

The screen shot makes clear about this module.


.. code-block:: bash

 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************


Deinstallation
----------------

Der Befehl für die Deinstallation des Moduls verwendet wird, aufgeführt unten ,


.. code-block:: bash

 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************



Option
-----------

.. cssclass:: table-bordered

 +--------------------------+------------------------------------------------+-------------+-------------------------------------------+
 | Parameters               | Alternative Parameters                         | Optionen    | Kommentare                                |
 +==========================+================================================+=============+===========================================+
 |Install phpedit? (Y/N)    | anstelle von PHP-Edit, folgende Alternativen   | Y           | Die Benutzer wünschen, den                | 
 |                          | können ebenfalls verwendet werden: phpedit,    |             | Installationsprozess zu fortzufahren.     |
 |                          | PHPEdit                                        |             |                                           |
 +--------------------------+------------------------------------------------+-------------+-------------------------------------------+
 |Install phpedit? (Y/N)    | anstelle von PHP-Edit, folgende Alternativen   | N           | Der Benutzer wünschen, um die             |
 |                          | können ebenfalls verwendet werden: phpedit,    |             | Installation zu beenden.                  |
 |                          | PHPEdit|                                       |             |                                           |
 +--------------------------+------------------------------------------------+-------------+-------------------------------------------+


Vorteile
---------------

* Schreiben Sie den Benutzer-Code schneller und mit allen zur Verfügung stehenden Code Assistenten und Code-Generatoren.
* Verbessern Sie die Qualität Ihrer Projekte mit dem integrierten Debugger, und die Unit-Tests Modul
* Stellen Sie leicht mit einem einzigen Klick die Benutzerprojekte und arbeiten transparent auf entfernte Dateien
* Erhöhen Sie die Produktivität der Anwender mit ihren Lieblings-Frameworks
* Code Intelligenz ist möglich.
* Debugger und Profiler ebenfalls zur Verfügung.
* Nicht Groß- und Kleinschreibung wirkt eine wichtige Rolle in diesem Modul

