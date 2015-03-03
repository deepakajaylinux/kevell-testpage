=================
Teamcity module
=================

Zusammenfassung
-------------------------

Teamcity ist ein Java-basiertes Build-Management und kontinuierliche Integration Server. Dieses Modul zielt darauf ab, die neueste Version von Teamcity-Server und seinen Abhängigkeiten zu installieren.

Hilfe Befehl
---------------

Der Befehl help führt den Anwender zur Verfügung zu stellen, was notwendig ist, um die Aufgabe zu erfüllen. Der Befehl zum Einsatz von dazu beitragen, dass im Rahmen der Terminal wird wie folgt angegeben,

.. code-block:: bash

	ptconfigure Teamcity help

Die nachfolgende Snapshots gibt Ihnen eine bildliche Darstellung der Befehl help, und es als Teamcity und Teamcity aufgeführten zwei Parameter. (Parameter ist die Groß- und Kleinschreibung)

.. code-block:: bash

	kevell@copy:/# ptconfigure teamcity help

	Dieser Befehl ermöglicht es Ihnen, Teamcity, die beliebte Build-Server installieren.
	Teamcity, teamcity

        - install
        Installs Teamcity from the Jetbrains distributed native package
        example: ptconfigure teamcity install

	------------------------------
	End Help
	******************************

Installation
-------------

Der Befehl zum Installieren Teamcity Modul verwendet wird unten gegeben,

.. code-block:: bash

	ptconfigure Teamcity install

Die folgende Abbildung erklärt, wie man Teamcity Module installiert.

.. code-block:: bash


	kevell@corp:/# ptconfigure Teamcity install
	Install Teamcity? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Teamcity !        *
	*******************************
	PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/Teamcity/Model/TeamcityUbuntu.php on line 42
	[Pharaoh Logging] Ensure module install is not checking versions
	[Pharaoh Logging] Module Java reports itself as Installed
	[Pharaoh Logging] Not installing as already installed
	Creating /tmp/ptconfigure-temp-script-82478215982.sh
	chmod 755 /tmp/ptconfigure-temp-script-82478215982.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-82478215982.sh Permissions
	Executing /tmp/ptconfigure-temp-script-82478215982.sh
	--2015-01-08 14:42:15--  http://download.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download.jetbrains.com (download.jetbrains.com)... 54.217.236.18
	Connecting to download.jetbrains.com (download.jetbrains.com)|54.217.236.18|:80... connected.
	HTTP request sent, awaiting response... 302 Moved Temporarily
	Location: http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz [following]
	--2015-01-08 14:42:16--  http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download-cf.jetbrains.com (download-cf.jetbrains.com)... 54.230.190.208, 54.230.190.220, 54.230.190.210, ...
	Connecting to download-cf.jetbrains.com (download-cf.jetbrains.com)|54.230.190.208|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 551078596 (526M) [application/x-tar]
	Saving to: ‘TeamCity-8.1.3.tar.gz’
		
	 99% [                                                                                                   >  ] 60,46,771   63.3KB/s 	

Options
---------

.. cssclass:: table-bordered

 +----------------------+----------------+-------------------------------------------------------------------------------------+
 | Parameters           | Erforderliche  | Kommentare                                                                          |
 +======================+================+=====================================================================================+
 |ptconfigure Teamcity  | Y(Yes)         | Dieser Befehl Teamcity Module installiert                                           |
 |install               |                |                                                                                     |
 +----------------------+----------------+-------------------------------------------------------------------------------------+
 |Install Teamcity?     | Y              | Wenn der Benutzer gibt Y, Das Modul untersucht für die Unterstützung                |
 |( Y/N)                |                | Voraussetzungen für Teamcity, wenn Ausfahrten wurde auf die neue Version            |
 |                      |                | aktualisiert oder er die neuen Paket mit unterstützenden Anforderungen installiert. |
 +----------------------+----------------+-------------------------------------------------------------------------------------+
 |Install Teamcity?     | N              | Wenn der Benutzer eingibt N wurde die Installation abgebrochen.                     |
 |( Y/N)|               |                |                                                                                     |
 +----------------------+----------------+-------------------------------------------------------------------------------------+



Vorteile für die Nutzer
----------------------------

* Installiert alle Unterstützung Anforderungen an Teamcity-Server in einer effizienten Weise ausgeführt
* Einfache Anwendung von Zugangs- und Installation
* Coding wird nicht beachtet.

