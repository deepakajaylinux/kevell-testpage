============
Wordpress
============

Zusammenfassung
-----------------

Dieses Modul ist ein schönes Teil der Rückstellung eine, die die Nutzer bei der Integration der Word Press Websites erleichtert. Zu seinen Aufgaben gehören dapperfy, builderfy und bietet auch Word Press Datenbankkonfiguration für die DBConfigure Modul.

Word Press ist eine freie und Open-Source-Blogging-Tool und ein Content Management System (CMS) auf Basis von PHP und MySQL. Zur Ausstattung gehören eine Plugin-Architektur und ein Template-System. Word Press wurde von mehr als 23,3% der 10 Millionen Websites im Januar 2015. Word Press den beliebtesten Blogging-System im Einsatz auf dem Web verwendet wird, bei mehr als 60 Millionen Websites.

Hilfe Befehl
-------------------

Der Befehl Hilfe erläutert die Nutzer in Bezug auf die Hauptfunktion des Moduls, seine alternative Parameter, die in Erklärungen verwendet werden können, die drei Hauptfunktionen (zB: dapperfy, builderfy, ausführen), und auch über die Syntax für die Deklaration seiner drei Hauptfunktionen. Der Befehl zur Feststellung der Hilfe-Option verwendet, ist unten dargestellt,

.. code-block:: bash

	ptdeploy Wordpress help


Der folgende Screenshot zeigt visuell in Bezug auf die Hilfe-Befehl unter diesem Modul. Die in der Erklärung Syntax ist nicht case-sensitive. 

.. code-block:: bash

 kevell@corp:/# ptdeploy Wordpress help
 ******************************


  This module is a Default one, and provides integration for Wordpress websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Wordpress Database Configuration for the DBConfigure Module.

  Wordpress, wordpress

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Wordpress.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy wordpress --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************




Wie dapperfy Wordpress verwenden
--------------------------------------

Der Befehl zum dapperfy die Wordpress ist unten angegeben verwendet wird,


.. code-block:: bash

	ptdeploy dapperfy wordpress


Nach der Eingabe des Befehls oben angegebenen, beginnt der Prozess der dapperfying wie in der Tabelle unten dargestellt,

.. cssclass:: table-bordered


 +--------------------------+-----------------------------------------+-------------+-----------------------------------------------------+
 | Parameters               | Alternative Parameters                  | Options     | Kommentare                                          |
 +==========================+=========================================+=============+=====================================================+
 |Dapperfy This for         | Anstelle von Wordpress, Wordpress       | Y(Yes)      | Wenn der Benutzer, um die Wordpress können sie      | 
 |Wordpress? (Y/N)          | kann man auch verwenden.                |             | Eingang als Y. dapperfy muss                        |
 +--------------------------+-----------------------------------------+-------------+-----------------------------------------------------+
 |Dapperfy This for         | Anstelle von Wordpress, Wordpress       | N(No)       | Wenn der Benutzer nicht in der Notwendigkeit, die   |
 |Wordpress? (Y/N)          | kann man auch verwenden.                |             | Wordpress können sie Eingang als N. dapperfy|       |
 +--------------------------+-----------------------------------------+-------------+-----------------------------------------------------+


Wenn der Benutzer den Prozess der dapperfying die Wordpress, die während der Ausführung dapperfying die folgenden Schritte erfolgt verläuft,

Schritt 1:

Verwenden vorhandener Umgebungseinstellungen? (Y / N)

Der Benutzer muss J oder N angeben, je nach ihrem Wunsch nach der vorhandenen Umgebungseinstellungen.

Schritt 2:

Haben Sie eine andere Umgebung hinzufügen? (Y / N)

Der Benutzer muss J oder N angeben, je nach ihrem Wunsch für das Hinzufügen eines weiteren Umgebung.

Nach Abschluss dieser Schritte, den Prozess der dapperfying die Wordpress wird abgeschlossen. Es ist optisch von dem Screenshot unten angegeben dargestellt,

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress
 Dapperfy This for Wordpress? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
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
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
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
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 
Arbeiten von Wordpress Auto Deploy-Dateien
------------------------------------------------

Zur Erzeugung der automatischen Bereitstellung von Dateien in Wordpress, wird der Benutzer zur Eingabe müssen Sie den Befehl unten angegeben,

.. code-block:: bash

	ptdeploy dapperfy wordpress --yes --guess


Nach der Eingabe des Befehls oben angegeben, die automatische Bereitstellung von Dateien erzeugt werden, wie bildhaft aus der Abbildung unten dargestellt,

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress --yes --guess
 Standard Dapperfies:
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
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
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
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************


Vorteile
----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Auch Word Press verfügt über integrierte Linkmanagement; eine Suchmaschine, freundlich, sauber Permalink-Struktur
* Es hat die Fähigkeit, mehrere Kategorien Artikel zuweisen; und Unterstützung für die Kennzeichnung der Beiträge und Artikel.
* In Wordpress Automatikfilter sind ebenfalls enthalten und bietet eine standardisierte Formatierung und Formatierung von Text in Artikeln
