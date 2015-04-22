==========
Joomla
==========

Zusammenfassung
----------------

Joomla bietet Integrations Website. Viele Web-Hosting-Services bieten eine Ein-Klick-Installation immer den Benutzer neuen Standort und in nur ein paar Minuten laufen.

Einschließlich seiner einfachen Bedienbarkeit und Erweiterbarkeit, haben Joomla die beliebteste Website-Software. Best of all, Autopilot, builderfy und dapperfy sind in ptdeploy und macht eine beste Lösung. Das ist komfortabel mit Ubuntu und Cent OS.

Hilfe Befehl
------------------------

Dieser Befehl help führt den Anwender zur Integration für Joomla bieten. Es hat personalisiert Autopilot, builderfy und dapperfy sind in ptdeploy .Auch bietet Datenbankkonfiguration für die db configure-Modul.

Der Befehl help for Oracle ist nachfolgend dargestellt.

.. code-block:: bash

	ptdeploy joomla help

Nach Eingang der obige Befehl, beginnt es funktioniert, um Joomla Website zu integrieren. Es Katechese die Funktionen joomla in den Screenshots.

.. code-block:: bash

 kevell@corp:/# ptdeploy Joomla help
 ******************************


  This module is a Default one, and provides integration for Joomla websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Joomla Database Configuration for the DBConfigure Module.

  Joomla, joomla

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Joomla.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy joomla --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************


Dapperfy
---------------

Diese dapperfy verwendeten die Benutzer Auto Deploy-Dateien. Dapperfy kann für eine Reihe von Projekten, ohne komplexe Konfigurationen mit ein paar Minuten im Wert von Einrichtung zu arbeiten. Mit Dapperfy ist sehr schnell und ist wahrscheinlich der beste Ausgangspunkt, auch bei komplexen Konfigurationen der Benutzer immer nur die Dateien zu ändern danach mit eigenen Anpassungen. Der folgende Befehl verwendet für dapperfy.

.. code-block:: bash

	ptdeploy dapperfy joomla

Nach der Eingabe wie die oben genannten Befehl dazu aufgefordert, dapperfy Ausführung zeigt der Screenshot.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy joomla
 Dapperfy This for Joomla? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************

Builderfy
--------------

Es schafft Vorlagen build installieren. Der Anwender kann weitere Vorlagen hinzufügen. Wenn wir Änderungen an der Benutzer-Repository, Sie eine neue Version für den Anwender Ziel Produktion. Der Befehl zum builderfy verwendet ist wie folgt,

.. code-block:: bash

	ptdeploy builderfy continuous-joomla


Der folgende Screenshot erklärt seine Funktion.

.. code-block:: bash


 kevell@corp:/# ptdeploy builderfy continuous-joomla
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Success
 In Builderfy
 ******************************


ausführen
------------

Dieser Vorgang auszuführen Autopilot build Schöpfer. Schnellzugriffe möglich sind. Der Befehl für die Ausführung wie folgt,

.. code-block:: bash

	ptdeploy autopilot execute

Der folgende Screenshot erklären seine Funktionen.

.. code-block:: bash



Option
------------

.. cssclass:: table-bordered

 +----------------------------------------+-----------+------------------------------------------------------------+
 | Parameters                             | Options   | Kommentare                                                 |
 +========================================+===========+============================================================+
 |Dapperfy this for joomla? (Y/N)         | Y         | Es wird joomla unter ptdeploy in Pharaoh Tools dapperfy    |
 +----------------------------------------+-----------+------------------------------------------------------------+
 |Dapperfy this for joomla? (Y/N)         | N         | Das System der Ausfahrt dapperfy                           |
 +----------------------------------------+-----------+------------------------------------------------------------+
 |Do you want to add another              | Y         | Es ermöglicht dem Benutzer die nächste Umgebung auswählen  |
 |environment?(Y/N)                       |           |                                                            |
 +----------------------------------------+-----------+------------------------------------------------------------+
 |Do you want to add another              | N         | Es ermöglicht dem Benutzer, den Prozess zu stoppen         |
 |environment?(Y/N)|                      |           |                                                            |
 +----------------------------------------+-----------+------------------------------------------------------------+


Vorteile
------------

* Gut Unterstützung für IT-Profis
* Mehrsprachige Prozess
* Einfaches Upgrade
* Speedy Systemfunktion
* Nicht Groß- und Kleinschreibung
* Geeignet für Ubuntu und Cent OS.


Das Joomla selbst eröffnet eine ganz neue Welt des Ausdrucks, weil es Ihnen die Freiheit zu bedienen, dass der Benutzer Design Traum wahr werden lässt!

