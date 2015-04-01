======
Go
======

Synopsis
----------


Go ist eine erweiterte Continuous Integration und Release-Management -System. Es dauert ein innovatives Konzept zur Verwaltung der Aufbau , Test und Freigabeprozess . Go ist ein Open -Source-Produkt .


Hilfe Befehl
---------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten , die in der Go -Modul enthalten sind. Es listet einige der alternativen Parameter der Go -Modul. Es beschreibt auch die Syntax für die Installation des Go. Der Befehl help zur Go -Modul wird wie unten dargestellt.

.. code-block:: bash

	ptconfigure ThoughtWorksGo help

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,



.. code-block:: bash

 kevell@corp:/# ptconfigure ThoughtWorksGo help

 ******************************


  This command allows you to install the ThoughtWorks Go.

  ThoughtWorksGo, thoughtworks-go, thoughtworksgo

        - install server
        Install the the Thoughtworks Go Server
        example: ptconfigure thoughtworksgo install --yes --guess --install-server
       
        - install Agent
        Install the the Thoughtworks Go Agent
        example: ptconfigure thoughtworksgo install --yes --guess --install-agent


 ------------------------------
 End Help
 ******************************


Installation
----------------

Der Befehl für die Installation des Moduls Go auf dem Terminal verwendet wird, aufgeführt unten ,

.. code-block:: bash


	ptconfigure thoughtworksgo install --yes --guess --install-server

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure thoughtworksgo install --yes --guess --install-server

 *******************************
 *        Pharaoh Tools        *
 *         ThoughtWorks Go!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-15356059969.sh
 chmod 755 /tmp/ptconfigure-temp-script-15356059969.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-15356059969.sh Permissions
 Executing /tmp/ptconfigure-temp-script-15356059969.sh
 --2015-03-31 11:03:48--  http://download01.thoughtworks.com/go/14.1.0/ga/go-server-14.1.0-18882.deb
 Resolving download01.thoughtworks.com (download01.thoughtworks.com)... 205.251.73.100
 Connecting to download01.thoughtworks.com (download01.thoughtworks.com)|205.251.73.100|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 134577812 (128M) [application/x-deb]
 Saving to: â€˜go-server-14.1.0-18882.debâ€™

 100%[===========================================================================================>] 13,45,77,812 22.6KB/s   in 78m 24s

 2015-03-31 12:22:14 (27.9 KB/s) - â€˜go-server-14.1.0-18882.debâ€™ saved [134577812/134577812]

 dpkg: no packages found matching cruise-server
 chown: cannot access â€˜/var/lib/go-server/**â€™: No such file or directory
 nohup: redirecting stderr to stdout
 Selecting previously unselected package go-server.
 (Reading database ... 233409 files and directories currently installed.)
 Preparing to unpack .../tmp/go-server-14.1.0-18882.deb ...
 Adding system user `go' (UID 134) ...
 Adding new group `go' (GID 146) ...
 Adding new user `go' (UID 134) with group `go' ...
 Creating home directory `/var/go' ...
 Unpacking go-server (14.1.0-18882) ...
 Setting up go-server (14.1.0-18882) ...
 Found Java /usr/lib/jvm/java-7-openjdk-amd64/jre in PATH, using it.
 Installation of Go Server completed.
 using default settings from /etc/default/go-server
 Started Go Server on http://murali:8153/go
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Temp File /tmp/ptconfigure-temp-script-15356059969.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ThoughtWorksGo: Success
 ------------------------------
 Installer Finished
 ******************************


Alternative Parameter
------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden kann ,

ThoughtWorksGo, thoughtworks-go, thoughtworksgo


Vorteile
---------

* Einheitliche Gestaltung von Entwicklungsmaschinen
* Einfach Onboarding
