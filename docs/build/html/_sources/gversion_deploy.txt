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


Der folgende Screenshot zeigt den vollen Einsatz der ptdeploy.Version, version, VERSION

Installation
----------------

Die Installation umfasst die Installation von Version erforderlich, um die Installation in einer aktualisierten Version zu machen. Es ist eine offensichtliche Prozess auf Version Modul unter ptdeploy installieren. Version mit nur mit dem Befehl unten angegeben,

.. code-block:: bash

	ptdeploy version Install

Nach beleben den Befehl geben Sie den Wert katechisieren.

Wenn die Benutzereingaben wie ja es wird automatisch Version mit der Überprüfung aus dem System zu installieren. Wenn nicht beenden Sie die Installation. Der folgende Screenshot zeigen, Version und seine Funktionen.


Option
------------

.. cssclass:: table-bordered

 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+
 | Parameters                   | Alternative parameter                      | Option    | Kommentare                                   |
 +==============================+============================================+===========+==============================================+
 |Install version?(Y/N)         | Anstelle der Verwendung von Version        | Yes       | Unter ptdeploy Modul erfolgreich             |
 |                              | kann der Anwender nutzen Version,VERSION   |           | installiert                                  |
 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+
 |Install version?(Y/N)         | Anstelle der Verwendung von Version kann   | No        | Verlassen Sie das Bild                       |
 |                              | der Anwender nutzen Version, VERSION.|     |           |                                              |
 +------------------------------+--------------------------------------------+-----------+----------------------------------------------+


Vorteile
---------------

* Neue Version aktualisiert werden kann.
* Es eignet sich mit Ubuntu und CentOS.
* Nicht Groß- und Kleinschreibung
* Automation möglich
* Einfach zu der Eingabe der Befehle
