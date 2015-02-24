==============
ModuleManager
==============

Zusammenfassung
-----------------------

Der Hauptanwendungsbereich des Modulmanagers ist es, dem Benutzer erlauben, ihre Module verwalten. Seine Hauptfunktionen beinhaltet die Installation, aktivieren, deaktivieren, stellen Sie sicher, deinstallieren. wollen wir sehen, über diese wichtige Funktionen des Modul-Manager in einer aufwendigen Weise aus den anstehenden Themen.

Hilfe Befehl
----------------------

Der Befehl help dieser Modul-Manager ist eine kurze Bedienungsanleitung, die den Benutzer über den Zweck führt, der Modul-Manager, beschreibt die Benutzer über die wichtigsten Funktionen, wie zu installieren, aktivieren, deaktivieren, stellen Sie sicher, deinstallieren Sie zusammen mit der Syntax für die Deklaration ihnen. Außerdem werden outs die alternativen Parameter Modul-Manager. Der Befehl zur Feststellung der Hilfe-Option im Rahmen des Modul-Manager wie folgt dar:

.. code-block:: bash

		ptconfigure  ModuleManager help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Modul-Manager.

.. code-block:: bash


 kevell@corp:/# ptconfigure  ModuleManager help

 ******************************


  The Module Manager allows you to manage modules. Install, Ensure, Uninstall, Enable, Disable.

  ModuleManager, module-manager, modulemanager

        - install
        Installs the latest version of a module. If a module of the same name already exists in your Extensions directory,
        an error will be thrown.
        example: ptconfigure  module-manager install --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - ensure
        Ensures the existence of a module. The module will only be installed if it currently doesn't exist.
        example: ptconfigure  module-manager ensure --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - uninstall
        Uninstalls a Module. This will delete all of the files for this Module
        example: ptconfigure  module-manager enable --module-name="MyModule"

        - enable
        Enables a Module. All installed Modules are enabled by default.
        example: ptconfigure  module-manager enable --module-name="MyModule"

        - disable
        Disables a Module. The files for this module will still exist, but none will be automatically loaded during execution.
        example: ptconfigure  module-manager disable --module-name="MyModule"

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl für die Installation der Modulmanager in der Benutzer-Maschine verwendet wird, wie folgt dar:

.. code-block:: bash

		ptconfigure  module-manager install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+
 | Parameter               | Alternative Parameter                   | Optionen  | Kommentare                                     |
 +=========================+=========================================+===========+================================================+
 |Install ModuleManager?   | anstelle von module-manager, wir        | Y(Yes)    | Wenn der Benutzer wünschen, den                |
 |(Y/N)                    | verwenden können, modulemanager,        |           | Installationsprozess können sie Eingang        |
 |                         | ModuleManager also.                     |           | als Y. gehen                                   |
 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+
 |Install ModuleManager?   | anstelle von module-manager, wir        | N(No)     | Wenn der Benutzer wünschen, den                |
 |(Y/N)                    | verwenden können, modulemanager,        |           | Installationsprozess können sie Eingang        |
 |                         | ModuleManager also.                     |           | als N. beenden|                                |
 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+

Wenn der Benutzer geht der Installation, während des Prozesses der Montage wird der folgende Prozess durchgeführt, wie in der Form einer 
Tabelle:

.. cssclass:: table-bordered

 +----------------------------+----------------------+------------+-------------------------------------------------------------+
 | Parameters                 | Weg                  | Optionen   | Kommentare                                                  |
 +============================+======================+============+=============================================================+
 |Program executor directory  | “/usr/bin”           | Yes        | Wenn der Benutzer die Installation mit dem Standardprogramm |
 |(Default)                   |                      |            | Testamentsvollstrecker Verzeichnis gehen sie eingeben       |
 |                            |                      |            | kann als Ja                                                 |
 +----------------------------+----------------------+------------+-------------------------------------------------------------+
 |Program executor directory  | user specific        | No(End     | Wenn der Benutzer die Installation mit eigenen              |
 |(Default)                   |                      | slash)     | Programmausführungs Verzeichnis können sie Eingang als N    |
 |                            |                      |            | gehen, und in die Hand geben sie Ort besitzen|              |
 +----------------------------+----------------------+------------+-------------------------------------------------------------+


Schließlich Installation abgeschlossen wird, wie in der Abbildung unten dargestell

ermöglichen
-------------

Der Freigabeprozess zielt darauf ab, so dass das Modul. Alle installierten Module werden standardmäßig mit dem Befehl unten angegeben aktiviert:

.. code-block:: bash

	ptconfigure  module-manager enable --module-name="MyModule"

Nach Eingabe dieses Befehls, das Modul, die angegeben wird, wird aktiviert.

Deaktivieren
----------------

Die Sperrprozess zielt darauf ab, das Deaktivieren des Moduls. Die Dateien der Module deaktiviert bleibt vorhanden, aber sie werden nicht zum Zeitpunkt der Ausführung geladen werden. Dies kann durch den folgenden Befehl erreicht werden

.. code-block:: bash

	ptconfigure  module-manager disable --module-name="MyModule"

Type text or a website address or translate a document.

Nach Eingabe dieses Befehls, das Modul, die angegeben wird, wird gesperrt.

Dafür Sorgen
---------------

Die Rolle sicherzustellen Prozesses ist es, die Verfügbarkeit von Modulen zu überprüfen. Nachdem der Prozess der Sicherstellung abgeschlossen wird die Module installiert werden, wenn die Module melden sich als nicht installiert. Der Prozess der sicherstellen kann, indem Sie den Befehl unten angegeben durchgeführt werden:

.. code-block:: bash

		ptconfigure  module-manager ensure

Während des Prozesses der Sicherung werden die Versionen der Module nicht überprüft. Der folgende Screenshot bildlich darstellen, den Prozess der zu gewährleisten.

.. code-block:: bash

 kevell@corp:/# ptconfigure  module-manager ensure

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ModuleManager reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ModuleManager: Success
 ------------------------------
 Installer Finished
 ******************************

Uninstall
-------------

Der Deinstallationsvorgang wird verwendet, um alle Dateien für die Module löschen. Der Befehl für die Deinstallation der Modul-Manager verwendet wird, wie folgt dar:

.. code-block:: bash

		ptconfigure  module-manager uninstall

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered


 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+
 | Parameter               | Alternative Parameter                   | Optionen  | Kommentare                                     |
 +=========================+=========================================+===========+================================================+
 |UnInstall ModuleManager? | anstelle von module-manager, wir        | Y(Yes)    | Wenn der Benutzer wünschen, die                |
 |(Y/N)                    | verwenden können, modulemanager,        |           | un Installation können sie Eingang             |
 |                         | ModuleManager also.                     |           | als Y. gehen                                   |
 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+
 |UnInstall ModuleManager? | anstelle von module-manager, wir        | N(No)     | Wenn der Benutzer wünschen, die                |
 |(Y/N)                    | verwenden können, modulemanager,        |           | un Installation können sie Eingang             |
 |                         | ModuleManager also.                     |           | als N. beenden|                                |
 +-------------------------+-----------------------------------------+-----------+------------------------------------------------+


Wenn der Benutzer geht die un-Installation, während des Prozesses der un-Installation wird der folgende Prozess durchgeführt, wie in der Tabellenform dargestellt:



.. cssclass:: table-bordered


 +----------------------------+----------------------+------------+----------------------------------------------------------------+
 | Parameters                 | Weg                  | Optionen   | Kommentare                                                     |
 +============================+======================+============+================================================================+
 |Program executor directory  | “/usr/bin”           | Yes        | Wenn der Benutzer die un Installation mit dem Standardprogramm |
 |(Default)                   |                      |            | Testamentsvollstrecker Verzeichnis gehen sie eingeben          |
 |                            |                      |            | kann als Ja                                                    |
 +----------------------------+----------------------+------------+----------------------------------------------------------------+
 |Program executor directory  | user specific        | No(End     | Wenn der Benutzer die un Installation mit eigenen              |
 |(Default)                   |                      | slash)     | Programmausführungs Verzeichnis können sie Eingang als N       |
 |                            |                      |            | gehen, und in die Hand geben sie Ort besitzen|                 |
 +----------------------------+----------------------+------------+----------------------------------------------------------------+



Schließlich un-Installation abgeschlossen wird, wie in der Abbildung unten dargestellt

.. code-block:: bash

Vorteile
-------------

* Die in Hilfe und Installation, Deinstallation verwendet wird, aktivieren, deaktivieren gewährleisten muss nicht beachtet werden, welche ein 
  zu sätzlicher Vorteil ist, während Parameter im Vergleich zu anderen.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Die sicherzustellen Verfahren erleichtert die Kontrolle Verfügbarkeit der Module vor der Installation.
* Wenn der Benutzer wünschen, ein bestimmtes Modul deaktivieren, können sie sie zu löschen, ohne ihre entsprechenden Dateien zu deaktivieren.
* Während der Installation, dem Benutzer zu deinstallieren können den Speicherort für die Programmausführungs Verzeichnis angeben.

