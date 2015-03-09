==============
Jenkins
==============

Zusammenfassung
-------------------------

Jenkins ist sehr beliebt, um Server zu bauen. Jenkins ist ein Open Source kontinuierliche Integration-Tool in Java geschrieben. Jenkins bietet kontinuierliche Integrationsleistungen für die Softwareentwicklung. Es ist ein Server-basiertes System läuft in einem Servlet-Container wie Apache Tomcat.

Kernfunktionalität und Flexibilität Jenkins 'lassen Sie ihn in einer Vielzahl von Umgebungen geeignet und kann helfen, den Entwicklungsprozess für alle Beteiligten

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von Jenkins Modul bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen.

.. code-block:: bash
             
		ptconfigure jenkins help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash



 
 kevell@corp:/# ptconfigure jenkins help
 ******************************


 This command allows you to install Jenkins, the popular Build Server.

 Jenkins, jenkins

 - install
 Installs Jenkins through apt-get
 example: ptconfigure jenkins install

 ------------------------------
 End Help
 ******************************
 Installation
 ----------------

Wenn der Benutzer Jenkins Modul in Maschinen installieren muss, wird die unten gegebenen Befehl das Verfahren der Ausführung der Installation.

.. code-block:: bash
              
	        ptconfigure jenkins install

Der Screenshot der obigen Befehl aufgelistet unten,

.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins install
 Install Jenkins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Jenkins !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-14615194352.sh
 chmod 755 /tmp/ptconfigure-temp-script-14615194352.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-14615194352.sh Permissions
 Executing /tmp/ptconfigure-temp-script-14615194352.sh
 E: Could not get lock /var/lib/apt/lists/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/lib/apt/lists/
 OK
 Temp File /tmp/ptconfigure-temp-script-14615194352.sh Removed
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 jenkins : Depends: daemon but it is not installable
           Depends: default-jre-headless but it is not installable or
                    java-runtime-headless
 [Pharaoh Logging] Adding Package jenkins from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jenkins: Success
 ------------------------------
 Installer Finished
 ******************************

Optionen
-----------

.. cssclass:: table-bordered

 +---------------------------+---------------------------------------------+----------------+--------------------------------------------+
 | Parameters                | Alternative Parameter                       | Optionen       | Kommentare                                 |
 +===========================+=============================================+================+============================================+
 |ptconfigure Jenkins        | Anstelle der Verwendung von Jenkins,        | Y              | Sobald der Benutzer bietet die             |
 |Install                    | kann der Benutzer Jenkins                   |                | Möglichkeit , startet System-              |
 |                           |                                             |                | Installation                               |
 +---------------------------+---------------------------------------------+----------------+--------------------------------------------+
 |ptconfigure Jenkins        | Anstelle der Verwendung von Jenkins,        | N              | Sobald der Benutzer bietet die             |
 |Install                    | kann der Benutzer Jenkins                   |                | Möglichkeit , stoppt System-               |
 |                           |                                             |                | Installation|                              |
 +---------------------------+---------------------------------------------+----------------+--------------------------------------------+




Vorteile
--------------

* Sofortige Fehlererkennung
* Keine Integration Schritt im Lebenszyklus
* Entfaltbarer System zu einem bestimmten Zeitpunkt
* Aufnahme der Entwicklung des Projekts

