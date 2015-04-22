========
Drupal
========

Zusammenfassung
-----------------------

Drupal-Modul ist Teil der Standard-Module. Es bietet Autopiloten für Drupal, die von builderfy und dapperfy Autopiloten zugeschnitten ist. Neben dem builderfy und dapperfy bietet es drupal Bankkonfiguration für die DB configure Moduls.

Drupal ist ein freies Open-Source Content-Management-Framework in PHP geschrieben und unter der GNU General Public License. Es wird als Back-End-Rahmen für die mindestens 2,1% aller Websites weltweit von persönlichen Blogs der Unternehmens, politischen und Regierungs-Websites einschließlich WhiteHouse.gov und data.gov.uk. hin verwendet Es ist auch für das Wissensmanagement und Business Collaboration verwendet.

Drupal läuft auf allen Computer-Plattform, die sowohl eine Web-Server in der Lage, mit PHP (einschließlich Apache, Litespeed, IIS, Lighttpd, Hiawatha, Cherokee oder Nginx) und eine Datenbank (zB MySQL, MongoDB, MariaDB, PostgreSQL, SQLite oder Microsoft unterstützt SQL Server), um Inhalte und Einstellungen zu speichern.

Lassen Sie uns sehen, wie man das Drupal unter diesen Modulen in verschiedenen Aspekten dapperfy.

Hilfe Befehl
--------------------

Der Befehl help ist eine kurze und sowie interessante Zusammenfassung für den Benutzer. Sie bietet Informationen über seine wichtige Rolle, Angaben zum abweichenden Parameter, die in Erklärungen verwendet werden können, Seine drei Hauptfunktionen (builderfy, dapperfy, ausführen), und auch die Syntax für die Verwendung und zu erklären, diese drei interessante Funktionen. Die Hilfe-Option erklärte Syntax, ist unten angegeben.


.. code-block:: bash

	ptdeploy Drupal help



Nach der Eingabe des Befehls oben angegeben, kann der Benutzer die Anzeige aufgrund der Hilfe-Optionen zusammen mit den oben beschriebenen Details anzuzeigen, können Sie visuell diese Ergebnisse der Hilfe-Option erhalten, wie aus der folgenden Bildschirm dargestellt ist.

.. code-block:: bash

 kevell@corp:/# ptdeploy Drupal help
 ******************************


  This module is a Default Modules and provides autopilots for drupal tailored Builderfy and Dapperfy Autopilots.
  Also provides Drupal Database Configuration for the DBConfigure Module.

  Drupal, drupal

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Drupal.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy drupal --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

Wie Drupal Dapperfy
--------------------------------
 
Wir wollen sehen, über die verschiedenen Aspekte dieses Moduls in dapperfying die Drupal. Der Befehl für diesen Zweck verwendet wird, ist für alle Aspekte, wie unten dargestellt,

.. code-block:: bash

 	ptdeploy dapperfy drupal


Nach der Eingabe des Befehls oben angegeben, werden die folgenden Informationen während der Ausführung erkundigte sich aus der Tabelle dargestellt,

.. cssclass:: table-bordered


 +--------------------------+-------------------------------------+----------+--------------------------------------------------+
 | Parameters               | Alternative Parameters              | Options  | Kommentare                                       |
 +==========================+=====================================+==========+==================================================+
 |Dapperfy This for         | Anstelle von Drupal, können         | Y(Yes)   | Wenn der Benutzer die drupal sie eingeben        |
 |Drupal? (Y/N)             | wir drupal auch.                    |          | können, wie Y. dapperfy muss                     |
 +--------------------------+-------------------------------------+----------+--------------------------------------------------+
 |Dapperfy This for         | Anstelle von Drupal, können         | N(No)    | Wenn der Benutzer nicht in der Notwendigkeit,    |
 |Drupal? (Y/N)             | wir drupal auch.                    |          | die Drupal sie eingeben können, wie N. dapperfy| |
 +--------------------------+-------------------------------------+----------+--------------------------------------------------+


Wenn der Benutzer Erlös dapperfying die Drupal durch Eingabe als Y, werden die folgenden Schritte während der Ausführung beteiligt,

Schritt 1:

Haben Sie eine andere Umgebung hinzufügen? (Y / N)

Der Benutzer die Eingabe Y oder N aufweisen kann, je nach Bedarf für das Hinzufügen eines weiteren Umgebung.

Der folgende Screenshot zeigt visuell diesen Prozess der dapperfying die Drupal.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************


Die zweite Form der Deklaration der dapperfying von Drupal wird nachstehend erläutert, und der Befehl für das verwendet wird, ist die gleiche wie
.. code-block:: bash

	ptdeploy dapperfy drupal

Nach der Eingabe des Befehls oben angegeben, werden die folgenden Informationen während der Ausführung erkundigte sich aus der Tabelle dargestellt,

.. cssclass:: table-bordered

 +---------------------------+-------------------------------+-------------+---------------------------------------------------------------+
 | Parameters                | Alternative Parameters        | Options     | Kommentare                                                    |
 +===========================+===============================+=============+===============================================================+
 |Dapperfy This for          | Anstelle von Drupal, können   | Y(Yes)      | Wenn der Benutzer die drupal sie eingeben können, wie Y.      |
 |Drupal? (Y/N)              | wir drupal auch.              |             | dapperfy muss                                                 |
 +---------------------------+-------------------------------+-------------+---------------------------------------------------------------+
 |Dapperfy This for          | Anstelle von Drupal, können   | N(No)       | Wenn der Benutzer nicht in der Notwendigkeit, die Drupal      |
 |Drupal? (Y/N)              | wir drupal auch.              |             | sie eingeben können, wie N. dapperfy                          |
 +---------------------------+-------------------------------+-------------+---------------------------------------------------------------+
 |Use existing environment   |                               | Y(Yes)      | Wenn der Benutzer wünschen, mit den vorhandenen               |
 |settings? (Y/N)            |                               |             | Umgebungseinstellungen können sie Eingang als Y. gehen        |
 +---------------------------+-------------------------------+-------------+---------------------------------------------------------------+
 |Use existing environment   |                               | N(No)       | Wenn der Benutzer Wunsch, mit den neuen                       |
 |settings? (Y/N)            |                               |             | Umgebungseinstellungen gehen sie eingeben kann als N.|        |
 +---------------------------+-------------------------------+-------------+---------------------------------------------------------------+


Nach Abschluß der Untersuchungen oben angegeben, werden die folgenden Schritte, wie beschrieben, auszuführen,

Schritt 1:

Möchten Sie Einträge auf jede App in Umgebung ändern möchten default-lokale (J / N)

Der Benutzer die Eingabe Y oder N sind

Schritt 2:

Umwelt 1 Standard-local:

In diesem Schritt wird Wert für Umwelt und temp dir erkundigt werden und der Benutzer zur Eingabe von ihnen haben.

Schritt 3:

Enter-Servers ist ein Array von Einträgen

Ziel eingeben?

Geben Nutzer?

Nach Abschluß der Untersuchungen oben angegeben, werden die folgenden Schritte, wie beschrieben, auszuführen,

Schritt 1:

Möchten Sie Einträge auf jede App in Umgebung ändern möchten default-lokale (J / N)

Der Benutzer die Eingabe Y oder N sind

Schritt 2:

Umwelt 1 Standard-local:

In diesem Schritt wird Wert für Umwelt und temp dir erkundigt werden und der Benutzer zur Eingabe von ihnen haben.

Schritt 3:

Enter-Servers ist ein Array von Einträgen

Ziel eingeben?

Geben Nutzer?

Enter Password?

Der Benutzer hat die Eingabe diejenigen Daten erfragt.

Schritt 4:

In einem anderen Server? (Y / N)

Der Benutzer muss die Eingabe Y oder N je nach ihrem Wunsch.

Schritt 5:

Möchten Sie Einträge auf jede App in Umgebung ändern möchten default-lokalen -0.000 (J / N)

Der Benutzer die Eingabe Y oder N sind

Schritt 6:

Die Einstellungen für die Umwelt kann manuell, wenn die Eingabe nicht-Standardwerte erforderlich definiert werden.

Die Daten während der Ausführung der Anwendung Einstellungen erkundigt wie unten definiert sind,

Preis Git Repo-URL

Preis Optional privaten SSH-Schlüssel für Git Repo.

Preis Git Individuelle Niederlassung

Preis Apache VHost URL

Preis Apache VHost Hostname / IP

Preis, wie viele Revisionen zu halten

Preis-Leistungs-DB-IP-Adresse

Preis DB App Benutzername

Preis DB App User Pass

Schritt 7:

Haben Sie eine andere Umgebung hinzufügen? (Y / N)

Der Benutzer muss die Eingabe Y oder N, je nach ihren Bedürfnissen.

Das folgende Bild wird eine bildliche Darstellung zu geben für die oben genannten Schritte erläutert.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal

 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to modify entries applicable to any app in environment default-local (Y/N) 
 Y
 Environment 1 default-local : 
 Default Settings for Any App not setup for environment default-local enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /root/gg
 Enter user ?
 root
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 Do you want to modify entries applicable to any app in environment default-local-8080 (Y/N) 
 n
 Settings for dapper not setup for environment default-local-8080 enter them manually.
 Environment 2 default-local-8080 : 
 Value for: Project Container directory, (inc slash)
 /root/vv
 Value for: Git Repo URL
 
 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch
 
 Value for: Apache VHost URL (Don't Include http://)
 
 Value for: Apache VHost Hostname/IP
 
 Value for: How many revisions to keep
 
 Value for: DB IP Address
 
 Value for: DB App User Name (Will be created if not existing)
 
 Value for: DB App User Pass
 
 Value for: DB Name (Will be created if not existing)
 
 Value for: DB Admin User Name
 
 Value for: DB Admin User Pass
 
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 
 

Die dritte Form der Ausführung wird von den kommenden Schritten erklärt. Der Befehl ist identisch mit

.. code-block:: bash

	ptdeploy dapperfy drupal


Nach der Eingabe des Befehls oben angegeben, werden die folgenden Informationen während der Ausführung erkundigte sich aus der Tabelle dargestellt,


.. cssclass:: table-bordered

 +----------------------------+------------------------------------+------------+---------------------------------------------------------+
 | Parameters                 | Alternative Parameters             | Options    | Kommentare                                              |
 +============================+====================================+============+=========================================================+
 |Dapperfy This for Drupal?   | Anstelle von Drupal, können wir    | Y(Yes)     | Wenn der Benutzer die drupal sie eingeben können,       | 
 |(Y/N)                       | drupal auch.                       |            | wie Y. dapperfy muss                                    |
 +----------------------------+------------------------------------+------------+---------------------------------------------------------+
 |Dapperfy This for Drupal?   | Anstelle von Drupal, können wir    | N(No)      | Wenn der Benutzer nicht in der Notwendigkeit, die       |
 |(Y/N)                       | drupal auch.                       |            | Drupal sie eingeben können, wie N. dapperfy             |
 +----------------------------+------------------------------------+------------+---------------------------------------------------------+
 |Use existing environment    |                                    | Y(Yes)     | Wenn der Benutzer wünschen, mit den vorhandenen         |
 |settings? (Y/N)             |                                    |            | Umgebungseinstellungen können sie Eingang als Y. gehen  |
 +----------------------------+------------------------------------+------------+---------------------------------------------------------+
 |Use existing environment    |                                    | N(No)      | Wenn der Benutzer Wunsch, mit den neuen                 |
 |settings? (Y/N)             |                                    |            | Umgebungseinstellungen gehen sie eingeben kann als N.|  |
 +----------------------------+------------------------------------+------------+---------------------------------------------------------+


After completion of the enquiries given above, the following steps as described will execute,

Step 1:

Do you want to add another environment settings? (Y/N)

The user have to input Y or N.

Step 2:

Environment 3 default-local:

In this step, value for environment and temp dir are enquired and the user have to input them.

The settings for environment can be defined manually if needed to input non-default values.

The data's inquired during the execution of applying settings are defined as below,

Value for Project Container Directory.

Value for Git repo URL

Value for Optional Private SSH Key for Git Repo.

Value for Git Custom Branch

Value for Apache VHost URL

Value for Apache VHost Hostname/IP

Value for how many revisions to keep

Value for DB IP Address

Value for DB App User Name

Value for DB App User Pass

The following screenshot will give an pictorial representation for the steps explained above.



.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Value for: Project Container directory, (inc slash)

 Value for: Git Repo URL

 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch

 Value for: Apache VHost URL (Don't Include http://)

 Value for: Apache VHost Hostname/IP

 Value for: How many revisions to keep

 Value for: DB IP Address

 Value for: DB App User Name (Will be created if not existing)

 Value for: DB App User Pass

 Value for: DB Name (Will be created if not existing)

 Value for: DB Admin User Name

 Value for: DB Admin User Pass

 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************


Die vierte Art von dapperfying die Drupal wird nachstehend erläutert, und der Befehl verwendet wird, ist dieselbe wie

.. code-block:: bash

	ptdeploy dapperfy drupal

Nach der Eingabe des Befehls oben angegeben, werden die folgenden Informationen während der Ausführung erkundigte sich aus der Tabelle dargestellt,

.. cssclass:: table-bordered


 +-----------------------------+-------------------------------------+-----------+----------------------------------------------------------+
 | Parameters                  | Alternative Parameters              | Options   | Kommentare                                               |
 +=============================+=====================================+===========+==========================================================+
 |Dapperfy This for            | Anstelle von Drupal, können wir     | Y(Yes)    | Wenn der Benutzer die drupal sie eingeben können, wie    |
 |Drupal? (Y/N)                | drupal auch.                        |           | Y. dapperfy muss                                         |
 +-----------------------------+-------------------------------------+-----------+----------------------------------------------------------+
 |Dapperfy This for            | Anstelle von Drupal, können wir     | N(No)     | Wenn der Benutzer nicht in der Notwendigkeit, die        |
 |Drupal? (Y/N)                | drupal auch.                        |           | Drupal sie eingeben können, wie N. dapperfy              |
 +-----------------------------+-------------------------------------+-----------+----------------------------------------------------------+
 |Use existing environment     |                                     | Y(Yes)    | Wenn der Benutzer wünschen, mit den vorhandenen          |
 |settings? (Y/N)              |                                     |           | Umgebungseinstellungen können sie Eingang als Y. gehen   |
 +-----------------------------+-------------------------------------+-----------+----------------------------------------------------------+
 |Use existing environment     |                                     | N(No)     | Wenn der Benutzer Wunsch, mit den neuen                  |
 |settings? (Y/N)              |                                     |           | Umgebungseinstellungen gehen sie eingeben kann als N.|   |
 +-----------------------------+-------------------------------------+-----------+----------------------------------------------------------+


Wenn der Benutzer Erlös dapperfying die Drupal durch Eingabe als Y, werden die folgenden Schritte während der Ausführung beteiligt,

Schritt 1:

Haben Sie eine andere Umgebung hinzufügen? (Y / N)

Der Benutzer die Eingabe Y oder N aufweisen kann, je nach Bedarf für das Hinzufügen eines weiteren Umgebung.

Der folgende Screenshot zeigt visuell diesen Prozess der dapperfying die Drupal.


.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

Builderfy
--------------

Es schafft Drupal Templates Build installieren. Der Anwender kann weitere Vorlagen hinzufügen. Wenn wir Änderungen an der Benutzer-Repository , Sie eine neue Version für den Anwender Ziel Produktion . Der Befehl zum builderfy verwendet ist wie folgt,

.. code-block:: bash

        ptdeploy builderfy continuous-drupal

.. code-block:: bash



 kevell@corp:/# ptdeploy builderfy continuous-drupal
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



Vorteile
-----------

* Es ist gut-to-do sowohl ubuntu und als auch in Cent OS.
* Die in der Erklärung verwendeten Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Die Einstellungen für die Umwelt können während der Ausführung des dapperfying definiert werden.

