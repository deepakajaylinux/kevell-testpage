==============
PTDeploy
==============

Zusammenfassung
-------------------------

Die ptdeploy umhüllt die Anwendungen der Nutzer mit automatisierte Bereitstellung, Aufbau und Release-Funktionen, Web-App Versionierung und Infrastruktur-Code in PHP.

Es erleichtern die Benutzer und bietet automatisierte Deployment Templates und installiert eine vollständig kontinuierliche Build für Ihr Projekt.

Hilfe Befehl
---------------------

Wenn Sie den Zweck eines bestimmten Moduls wissen möchten, geben Sie einfach den Befehl wie folgt:

.. code-block:: bash
	
	ptdeploy ModuleName help

Dieser Befehl liefert die Verwendung dieser speziellen Modul und auch die verfügbaren Optionen in Aktionen, die Sie ausführen können. Die unter gezeigt Screenshot erläutert die Verwendung des Moduls Apache Steuer unter ptdeploy mit dem Befehl help.

Der Befehl help listet auch die alternativen Parameter, die in der Erklärung verwendet werden kann.

Warum diese ptdeploy bauen
------------------------------------------

Um gut Einsatz zu bauen, werden viele Dateien benötigt, um von FTP- oder anderen Ad-hoc-Lösungen kopiert werden. Und auch viele Unternehmen Automation Werkzeuge fehlten. Um diese Engpässe ptdeploy unter dem Pharao Werkzeug überwunden waren aufzubauen.
PHP hat ptdeploy wie Rubin fiils die Lücke in Capistrano.

Dieses Tool ist für die Bereitstellung Anwendungen und baut auf Ihre Boxen. Der Benutzer kann mit einem oder zwei PHP-Dateien Oder schnell Setup Cloud freundliche Bereitstellungsmustern einzurichten sogar einfache oder komplexe Anwendungsbereitstellungsmuster für ihr System.

ptdeploy ist modular aufgebaut. objektorientiert und erweiterbar. Also, wenn der Benutzer keine zusätzlichen Module erfordert sie erstellen und die neuen Module auf der Basis ihrer Anforderungen.

Diese ptdeploy fungiert als Wrapper, wo alle Schritte der Nutzer Implementierung wird in einer einzigen Datei bedeckt. Auf diese Weise können mit einem einzigen Befehl zu feuern eine Instanz Ihrer Anwendungen.

Installation
---------------

Installieren des ptdeploy können auf zwei Arten in Abhängigkeit von der Verfügbarkeit und Anforderungen der Anwender durchgeführt werden. Diese beiden Möglichkeiten des Einrichtens ptdeploy sind:

* Installieren ptdeploy über ptconfigure
* Installation des ptdeploy ohne Abhängigkeit von ptconfigure.



Installieren ptdeploy über ptconfigure
-------------------------------------------------

Wenn der Benutzer die ptconfigure in ihrer Maschine, dann ist es die einfacheren Weg, um ptdeploy mit dem folgenden Befehl installiert werden:

.. code-block:: bash

	sudo ptconfigure ptdeploy install --yes --guess

Installieren des ptdeploy ohne Abhängigkeit von ptconfigure
-------------------------------------------------------------------------------

Wenn der Benutzer wünschen, die ptdeploy ohne abhängig und mit dem ptconfigure sie mit dem folgenden Befehl installieren:

.. code-block:: bash
		
	sudo apt-get install php5 git

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install-silent

or 

Die folgende Befehl ist vorhersehbar für die Benutzer, um die Position während der Installation angeben möchten.

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install

Erweiterte Funktionen
-------------------------

Bearbeiten der Host-Dateien, virtuellen Host-Dateien, Konfigurationsdateien, Datenbankupdates und alle mit dieser automatisiert werden.

Durch die Verwendung der Fähigkeit der Remote-Server-Management, können die Benutzer-Bereitstellungen in Infrastruktur jeder Größe zu automatisieren.

Die Art und Weise, wie die ptdeploy fördert das Projekt mit dapperfy
-------------------------------------------------------------------------------------------

Das Wort ist eine dapperfy ptdeploy Befehl, einige Autopiloten für Ihr Projekt erstellt.

Mit dem dapperfy ist sehr schnell und ist wahrscheinlich der beste Ausgangspunkt.

Capify Vs Dapperfy
-------------------------

Beim Vergleich der capify mit dapperfy ist es offensichtlich, zu sagen, dass die dapperfy ist die beste, wie es ist in PHP geschrieben.

Die Stärke ist, dass die dapperfy ptdeploy Befehl stellt die Standard-Set von Autopiloten für die Benutzer Projekte. wo die capify bietet ähnliche Funktion wie der Ruby-Projekt.

So verwenden und Verfügbare Module
-----------------------------------------------

Lassen Sie uns sehen, wie man die ptdeploy Tool, zuerst, geben Sie einfach als

.. code-block:: bash

	ptdeploy

dieser Befehl die Namen der Module, die unter ptdeploy sind, aus.

* ApacheControl - Apache Server Control
* ApacheVHostEditor - Apache Virtual Host Functions
* AppSettings - PTDeploy Application Settings
* Autopilot - PTConfigure Autopilot - User Defined Installations
* Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
* CukeConf - Cucumber Configuration
* DBConfigure - Database Connection Configuration Functions
* DBInstall - Database Installation Management Functions
* Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
* Drupal - Drupal - Integration and Templates for Drupal
* EnvironmentConfig - Environment Configuration - Configure Environments for a project
* GitClone - GitClone Source Control Clone Functions
* HostEditor - Host File Management Functions
* Invoke - SSH Invocation Functions
* Joomla - Joomla - Integration and Templates for Joomla
* LighttpdControl - Lighttpd Server Control
* Logging - Logging - Output errors to the logging
* NginxControl - Nginx Server Control
* NginxSBEditor - Nginx Server Block Functions
* ParallelSshChild - Command Execution Functions
* Project - PTDeploy Project Management Functions
* RunCommand - Execute a Command
* SFTP - SFTP Functionality
* SVN - SVN Source Control Project Checkout/Download Functions
* SystemDetection - System Detection - Detect the Running Operating System
* Templating - Templating
* Version - Versioning Functions
* Wordpress - Wordpress - Integration and Templates for Wordpress


Hier bezeichnet der Bildschirm die Anzeige aller Module unter ptconfigure.


.. code-block:: bash

 Available Commands:
 ---------------------------------------

 ApacheControl - Apache Server Control
 ApacheVHostEditor - Apache Virtual Host Functions
 AppSettings - PTDeploy Application Settings
 Autopilot - PTConfigure Autopilot - User Defined Installations
 Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
 CukeConf - Cucumber Configuration
 DBConfigure - Database Connection Configuration Functions
 DBInstall - Database Installation Management Functions
 Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
 Drupal - Drupal - Integration and Templates for Drupal
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 GitClone - GitClone Source Control Clone Functions
 HostEditor - Host File Management Functions
 Invoke - SSH Invocation Functions
 Joomla - Joomla - Integration and Templates for Joomla
 LighttpdControl - Lighttpd Server Control
 Logging - Logging - Output errors to the logging
 NginxControl - Nginx Server Control
 NginxSBEditor - Nginx Server Block Functions
 ParallelSshChild - Command Execution Functions
 Project - PTDeploy Project Management Functions
 RunCommand - Execute a Command
 SFTP - SFTP Functionality
 SVN - SVN Source Control Project Checkout/Download Functions
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Version - Versioning Functions
 Wordpress - Wordpress - Integration and Templates for Wordpress

******************************



.. toctree::
   :maxdepth: 6
   

 gapachecontrol_deploy
 gapachevhosteditor_deploy
 gautopilot_deploy
 gdapperfy_deploy
 gdbconfigure_deploy
 gdbinstall_deploy
 gdrupal_deploy
 genvironmentconfig_deploy
 ggitclone_deploy
 ggrafana_deploy
 ghosteditor_deploy
 ginvoke_deploy
 gjoomla_deploy
 glighttpdcontrol_deploy
 glogging_deploy
 gnginxcontrol_deploy
 gnginxsbeditor_deploy
 gproject_deploy
 gruncommand_deploy
 gsftp_deploy
 gsvn_deploy
 gsystemdetection_deploy
 gtemplating_deploy
 gversion_deploy
 gwordpress_deploy





