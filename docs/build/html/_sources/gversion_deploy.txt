=========
Version
=========

Zusammenfassung
-----------------------

Dieses Modul verwendet werden, um aktualisierte Version unter ptdeploy installieren. Versionskontrolle am häufigsten als Stand-alone-Anwendungen ausgeführt werden, aber die Revisionskontrolle ist auch in verschiedenen Arten von Betriebssystem wie Ubuntu und Cent OS eingebettet. Die meisten Version können mehrere Entwickler auf dieselbe Datei gleichzeitig bearbeiten. Der erste Entwickler, "check in" Änderungen an der zentralen Repository immer gelingt. Das System können Einrichtungen zur Verfügung, um weitere Änderungen in den zentralen Repository zusammenzuführen, und die Erhaltung der von dem ersten Entwickler, wenn andere Entwickler überprüfen in.It unterstützt Ubuntu und CentOS.

Hilfe Befehl
-----------------------

Der Befehl help führt die Benutzer über die Version des ptdeploy. Die Optionen, die in der Version-Module enthalten sind. Der Befehl help listet einige der alternativen Parameter Version unter ptdeploy Modul. Es beschreibt auch die Syntax für die Ausführung. Der Befehl help zur Version wird unten gezeigt.

.. code-block:: bash

	ptdeploy  version help

Der folgende Screenshot zeigt den vollen Einsatz der ptdeploy.

.. code-block:: bash


 kevell@corp:/# ptdeploy Version help
 ******************************


  This command is part of Default Modules and handles Application Versioning, allowing for rollbacks and the like.

  Version, version, vrs

          - specific
          Will change back the *current* symlink to whichever available version you pick
          example: ptdeploy version specific --limit=4 --container=/var/www/applications/the-app --version=2

          - latest
          Will change back the *current* symlink to the latest created version
          example: ptdeploy version latest
          example: ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

          - rollback
          Will change back the *current* symlink to the latest created version but one
          example: ptdeploy version rollback
          example: ptdeploy version rollback --limit=3 --container=/var/www/applications/the-app


      You can also apply a limit to the number of Versions to keep by using the --limit parameter
          example: ptdeploy version latest --limit=3

 ------------------------------
 End Help
 ******************************


Alternative Parameter
-----------------------


Der folgende Screenshot zeigt den vollen Einsatz der ptdeploy. 

Version, version, vrs



Specific
-----------

Das Besondere Option ermöglicht es dem Benutzer, zu ändern zurück die aktuelle Version Verzeichnis bestimmte Version zu machen. Der Befehl für die bestimmte Option ist unten dargestellt ,

.. code-block:: bash

        ptdeploy version specific

or

.. code-block:: bash

        ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

.. code-block:: bash


 kevell@corp:/# ptdeploy version specific

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 Please Choose Version to make current (Showing newest first, Enter none for newest):
 --- All Versions: ---
 (0) karuna 

 0
 How many Versions to limit to? Enter 0 to ignore version limits
 2
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************
 
.. code-block:: bash

 kevell@corp:/# ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

Latest
----------

Die neueste Option erlaubt die Benutzer, die verfügbaren Link auf die neueste Version zu ändern zurück . Der Befehl für die neuesten Ausführungsprozess wird unten gezeigt ,

.. code-block:: bash 

        ptdeploy version latest

or

.. code-block:: bash

        ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

.. code-block:: bash


 kevell@corp:/# ptdeploy version latest

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 5
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version latest --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************

Rollback
----------

Die Option Rollback ermöglicht die Benutzer Änderungen an der bestehenden Version zu machen. Die Rollback- Ausführungsprozess wird unten gezeigt ,

.. code-block:: bash

        ptdeploy version rollback

or

.. code-block:: bash

        ptdeploy version rollback --limit=3 --container=/opt/versiontest/

.. code-block:: bash


 kevell@corp:/# ptdeploy version rollback

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 4
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version rollback --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************


Option
------------

.. cssclass:: table-bordered

 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+
 | Parameters                   | Alternative parameter                      | Option    | Kommentare                                   |
 +==============================+============================================+===========+==============================================+
 |Install version?(Y/N)         | Anstelle der Verwendung von Version        | Yes       | Unter ptdeploy Modul erfolgreich             |
 |                              | kann der Anwender nutzen Version,          |           | installiert                                  |
 |                              | version,vrs                                |           |                                              |
 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+
 |Install version?(Y/N)         | Anstelle der Verwendung von Version kann   | No        | Verlassen Sie das Bild                       |
 |                              | der Anwender nutzen Version,               |           |                                              |
 |                              | version, vrs|                              |           |                                              |
 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+


Vorteile
---------------

* Neue Version aktualisiert werden kann.
* Es eignet sich mit Ubuntu und CentOS.
* Nicht Groß- und Kleinschreibung
* Automation möglich
* Einfach zu der Eingabe der Befehle
