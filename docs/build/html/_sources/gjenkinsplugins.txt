================
JenkinsPlugins
================

Zusammenfassung
-----------------------

Jenkins ist sehr beliebt, um Server zu bauen. Jenins ist eine Quelle kontinuierliche Integration-Tool in Java geschrieben. Jenkins bietet kontinuierliche Integrationsleistungen für die Softwareentwicklung.

Plugins für Jenkins, die seine Verwendung, um Projekte in anderen Sprachen als Java geschrieben verlängern veröffentlicht. Plugins sind für die Integration von Jenkins mit den meisten Versionskontrollsysteme und große Datenbanken. Viele Build-Tools werden über ihre jeweiligen Plug-ins unterstützt. Plugins können auch die Art und Weise Jenkins sieht ändern oder neue Funktionen hinzufügen. Builds können Prüfberichte in verschiedenen Formaten von Plugins unterstützt generieren (JUnit-Unterstützung ist derzeit gebündelt) und Jenkins können die Berichte anzeigen und erstellen Trends und machen sie in der GUI.

Hilfe Befehl
-----------------

Diese Funktion dient, um die Verwendung von JenkinsPlugins Modul bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
             
	ptconfigure JenkinsPlugins help

 kevell@corp:/# ptconfigure JenkinsPlugins help
 ******************************


  This command allows you to install a bunch of plugins that we recommend for
  PHP builds in Jenkins.

  JenkinsPlugins, jenkinsplugins, jenkins-plugins, jenkins-plugs

        - install
        Installs the latest version of Jenkins Plugins for PHP recommended by Golden Contact
        example: ptconfigure jenkins-plugins install

 ------------------------------
 End Help
 ******************************

Installation
----------------

  Dieser Befehl ermöglicht es Ihnen, eine Reihe von Plugins, die wir für PHP baut in Jenkins installieren. Wenn der Benutzer Jenkins Modul in Maschinen installieren muss, wird die unten gegebenen Befehl das Verfahren der Ausführung der Installation.

.. code-block:: bash
        
		ptconfigure JenkinsPlugins install

Der Screenshot der obigen Befehl aufgelistet unten,

.. code-block:: bash

 


 kevell@corp:/# ptconfigure jenkins-plugins install
 Install Jenkins Plugins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jenkns Plgs!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-71115535759.sh
 chmod 755 /tmp/ptconfigure-temp-script-71115535759.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71115535759.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71115535759.sh
 Cloning into 'jplugins'...
 remote: Counting objects: 39, done.
 remote: Total 39 (delta 0), reused 0 (delta 0), pack-reused 39
 Unpacking objects: 100% (39/39), done.
 Checking connectivity... done.
 * Restarting Jenkins Continuous Integration Server jenkins
   ...done.
 Temp File /tmp/ptconfigure-temp-script-71115535759.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsPlugins: Success
 ------------------------------
 Installer Finished
 ******************************


Options
-----------     

.. cssclass:: table-bordered

 +----------------------+-------------------------------------------------------------+-------------+---------------------------------------+
 | Parameters           | Alternative Parameter                                       | Option      | Kommentare                            |
 +======================+=============================================================+=============+=======================================+
 |ptconfigure           | Entweder der vier alternative Parameter kann das Kommando   | Y           | Sobald der Benutzer bietet die        |
 |JenkinsPlugins        | verwendet werden - JenkinsPlugins, jenkinsplugins,          |             | Möglichkeit, startet                  |
 |Install               | jenkins-plugins, jenkins-plugs                              |             | System-Installation                   |
 |                      | eg: ptconfigure jenkins-plugins Install                     |             |                                       |
 +----------------------+-------------------------------------------------------------+-------------+---------------------------------------+
 |ptconfigure           | Entweder der vier alternative Parameter kann das Kommando   | N           | Sobald der Benutzer bietet die        |
 |JenkinsPlugins        | verwendet werden - JenkinsPlugins, jenkinsplugins,          |             | Möglichkeit, Anschläge                |
 |Install               | jenkins-plugins, jenkins-plugs                              |             | System-Installation                   |
 |                      | eg: ptconfigure jenkins-plugins Install|                    |             |                                       |
 +----------------------+-------------------------------------------------------------+-------------+---------------------------------------+


Vorteile
--------------

* Das Plugin wird Ihnen einen Bericht darüber, wie viel jedes Plugin wird in alle Ihre Aufgaben verwendet werden. Daher wird es die verwendeten   Verlängerungs analysieren Punkte der einzelnen Jobs.
* Dieses Plugin gibt Ihnen die Möglichkeit, die Nutzung Ihrer installierten Plugins analysieren.
* Nicht Groß- und Kleinschreibung
* Well-to-do in Ubuntu und CentOS.

