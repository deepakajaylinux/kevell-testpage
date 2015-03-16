===========
Dapperfy
===========

Zusammenfassung
----------------------

Dapperfy ist ein schönes Teil der Standard-Core-Modul, die bei der Schaffung eines Standard-Set von Autopiloten-Dateien für ihre Projekte hilft und unterstützt die Anwender. Die Benutzer können Standard-Anwendungen konfigurieren. Zum Beispiel: mysql Admin-Benutzer, Host, weiterzugeben.

Lassen Sie uns sehen, wie man dapper Standard und adrett Liste Aufgaben im Rahmen dieses Moduls aus den anstehenden Themen zu verwenden.

Hilfe Befehl
--------------------

Der Befehl help umhüllt alle notwendigen Informationen über dapperfy wie auch vorrangig, die Liste der alternativen Parameter, die in der Erklärung verwendet werden kann, was sind primäre Funktion dapperfy (Ex: Standard, Liste), und auch die Syntax für die Deklaration verwendet diese interessante Funktionen. Der folgende Befehl ist für Hilfe-Option unter dapperfy erklärt verwendet,

.. code-block:: bash


	ptdeploy Dapperfy help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# ptdeploy Dapperfy help
 ******************************
.. code-block:: bash

  This command is part of a default Module Core and provides you with a method by which you can
  create a standard set of Autopilot files for your project from the command line.
  You can configure default application settings, ie: mysql admin user, host, pass


  Dapperfy, dapperfy

        - list
        List all of the autopilot files in your build/config/ptdeploy/autopilots
        example: ptdeploy dapperfy list

        - standard
        Create a standard set of autopilots to manage
        example: ptdeploy dapperfy standard

        The start of the command will be ptdeploy autopilot execute *filename*

 --------------
  Drupal Module:

  The Drupal module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Drupal site. This module adds the 'drupal' action to dapperfy.

  - drupal
  create drupal tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy drupal --yes --guess

 --------------
  Joomla Module:

  The Joomla module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Joomla site. This module adds the 'joomla' action to dapperfy.

  - joomla, joomla30
  create joomla tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy joomla --yes --guess

  - joomla-phlagrant, joomla30-phlagrant
  create joomla tailored automated deployment ptdeploy autopilots for your Phlagrant Virtual Machines
  example: ptdeploy dapperfy joomla-phlagrant --yes --guess
 --------------
  Wordpress Module:

  The Wordpress module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Wordpress site. This module adds the 'wordpress' action to dapperfy.

  - wordpress
  create wordpress tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy wordpress --yes --guess
 ------------------------------
 End Help
 ******************************



Wie Dapper Norm verwenden
---------------------------------------

Der Befehl zum dapperfy Standard verwendet wird unten gezeigt,

.. code-block:: bash

	ptdeploy dapperfy standard

Nach der Eingabe des Befehls oben angegeben wurde, wird der folgende Prozess, wie in der Tabelle unten beschrieben in einem Schritt-für-Schritt-Basis.

.. cssclass:: table-bordered


 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 | Parameters                  | Alternative Parameters    | Options     | Kommentare                                                  |
 +=============================+===========================+=============+=============================================================+
 |Dapperfy This? (Y/N)         | Statt dapperfy können wir | Y(Yes)      | Wenn der Benutzer wünschen, dapperfying Prozess, den        |
 |                             | Dapperfy auch.            |             | sie eingeben können, wie Y. gehen                           |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 |Dapperfy This? (Y/N)         | Statt dapperfy können wir | N(No)       | Wenn der Benutzer wünschen, die dapperfying Prozess,        |
 |                             | Dapperfy auch.            |             | den sie eingeben können, wie N. beenden                     |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 |Use existing environment     |                           | Y(Yes)      | Wenn der Benutzer wünschen, mit den vorhandenen             |
 |settings? (Y/N)              |                           |             | Umgebungseinstellungen können sie Eingang als Y. gehen      |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 |Use existing environment     |                           | N(No)       | Wenn der Benutzer Wunsch, mit den neuen                     |
 |settings? (Y/N)              |                           |             | Umgebungseinstellungen gehen sie eingeben kann als N.       |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 |Do you want to add another   |                           | Y(Yes)      | Wenn der Benutzer wünschen, eine andere Umgebung für        |
 |environment?                 |                           |             | dapperfying sie Eingang kann als Y. hinzufügen              |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+
 |Do you want to add another   |                           | N(No)       | Wenn der Benutzer nicht in der Notwendigkeit, ein           |
 |environment?                 |                           |             | weiteres Umfeld für dapperfying sie Eingang kann als N.|    |
 +-----------------------------+---------------------------+-------------+-------------------------------------------------------------+

Die zwei verschiedenen Arten von Bildschirm kann nützlich für die Benutzer, die eine bildliche Darstellung dapperfying Prozess sein. Der zweite Screenshot zeigt Methode zur Angabe Bereitschaft in einem der vorhandenen Umgebungseinstellungen.


.. code-block:: bash


 kevell@corp:/# ptdeploy dapperfy standard
 Dapperfy This? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 ******************************


 Success
 In Dapperfy
 ******************************


Wie Dapperfy Liste verwenden
---------------------------------

Das primäre Ziel der Liste Aufgabe es ist, alle Autopilot-Dateien der Benutzer Projekte, die an einem bestimmten Ort verfügbar sind, aus. Die Syntax für die Liste unter dapperfy ist unten dargestellt,

.. code-block:: bash

        ptdeploy dapperfy list

Der unten abgebildete Screenshot zeigt die Funktionsweise der Liste Option unter dapperfy.




Vorteile
-----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Der Benutzer kann die Liste der Dateien, die Autopiloten für ihre Projekte zur Verfügung stehen zu sehen.
* Während dapperfying, kann der Benutzer die Umgebungseinstellungen sie erfordert angeben.
* Viele Umgebungen hinzugefügt werden, um dapperfy werden.
