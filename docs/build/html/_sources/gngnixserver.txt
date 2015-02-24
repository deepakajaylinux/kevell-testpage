=============
NginxServer
=============

Zusammenfassung
-------------------------
Nginx, ausgesprochen "Engine X", ist ein High-Performance-Web-Server. Die Nginx Web-Server ist eine leichte und vielseitige Server, der für die verschiedenen Aufgaben, die viele moderne Webseiten Bedarf konfiguriert werden können. Ngnix Server fungiert als Vermittler für die Benutzer bei der Konfiguration von Anwendungseinstellungen. Einige Beispiele für Anwendungen, Einstellungen enthält MySQL Admin-Benutzer, Host weiter. Nginx macht Schlagzeilen als der neue Web-Server der Wahl für viele Webmaster. Die oberste Grund für seine Popularität ist seine Geschwindigkeit. Nginx ist schneller als Apache in nicht-Testumgebungen, da seine Architektur ist ereignisgesteuert, während der Apache-Prozess ist angesteuert. Die ptconfigure Module dient als Weg durch für die Installation dieses Nginx Server.

Hilfe Befehl
------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der Ngnix Servermodul enthalten sind. Der Befehl help listet einige der alternativen Parameter Ngnix Server. Es beschreibt auch die Syntax für die Installation Ngnix Server. Der Befehl help für Ngnix Server ist unten angegeben.

.. code-block:: bash

	ptconfigure nginx-server

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Nginx Server.

.. code-block:: bash


	kevell@corp:/# ptconfigure NginxServer help
	******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

	NginxServer, nginx-server, nginxserver

        - install
        Installs Nginx HTTP Server
        example: ptconfigure nginx-server install

	------------------------------
	End Help
	******************************


Installation
---------------

Installieren des Nginx Server ist einfacher, indem Sie den folgenden Befehl ein, wie gezeigt:
.. code-block:: bash

	ptconfigure nginx-server install

Nach der Eingabe des Befehls über die folgenden Vorgänge, wie gezeigt in der Tabellenform auf.

.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------------+-------------+------------------------------------------+
 | Parameter                | Alternative Parameter                         | Option      | Kommentare                               |
 +==========================+===============================================+=============+==========================================+
 |ptconfigure nginx-server  | Trotz Nginx Server, die folgende alternatives | Y(Yes)      | Wenn der Benutzer wünschen, den          |
 |install? (Y/N)            | auch verwendet werden: NginxServer,           |             | Installationsprozess können sie Eingang  |
 |                          | nginx-Server, nginxserver.                    |             | als Y. gehen                             |
 +--------------------------+-----------------------------------------------+-------------+------------------------------------------+
 |ptconfigure nginx-server  | Trotz Nginx Server, die folgende alternatives | N(No)       | Wenn der Benutzer wünschen, den          |
 |install? (Y/N)            | auch verwendet werden: NginxServer,           |             | Installationsprozess können sie Eingang  |
 |                          | nginx-Server, nginxserver.                    |             | als N. Beenden|                          |
 +--------------------------+-----------------------------------------------+-------------+------------------------------------------+

Wenn der Benutzer den Installationsprozess läuft, wird die Nginx HTTP Server installiert werden. Wenn das Paket von Nginx ist bereits in der Benutzer-Maschine vorhanden ist, wird eine Meldung angezeigt, um den Benutzer anweisen, wie Nginx ist vorhanden in dieser Maschine bereits. Schließlich Berichte werden mit klaren Ergebnissen und Status erzeugt. Der folgende Screenshot erklärt die oben genannten Verfahren bildlich.

.. code-block:: bash
	

	Kevell@corp:/# ptconfigure nginx-server install
	
	Install Nginx Server? (Y/N) 
	y	
	*******************************
	*        Pharaoh Tools        *
	*         Nginx Server!       *
	*******************************
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	nginx-common nginx-core
	Suggested packages:
	fcgiwrap nginx-doc
	The following NEW packages will be installed:
	nginx nginx-common nginx-core
	0 upgraded, 3 newly installed, 0 to remove and 278 not upgraded.
	Need to get 347 kB of archives.
	After this operation, 1,295 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-common all 1.4.6-1ubuntu3.1 [17.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-core amd64 1.4.6-1ubuntu3.1 [324 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx all 1.4.6-1ubuntu3.1 [5,218 B]
	Fetched 347 kB in 3s (104 kB/s)
	Selecting previously unselected package nginx-common.
	(Reading database ... 168194 files and directories currently installed.)
	Preparing to unpack .../nginx-common_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx-common (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx-core.
	Preparing to unpack .../nginx-core_1.4.6-1ubuntu3.1_amd64.deb ...
	Unpacking nginx-core (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx.
	Preparing to unpack .../nginx_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	ureadahead will be reprofiled on next reboot
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Setting up nginx-common (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Setting up nginx-core (1.4.6-1ubuntu3.1) ...
	Setting up nginx (1.4.6-1ubuntu3.1) ...
	[Pharaoh Logging] Adding Package nginx from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	NginxServer: Success
	------------------------------
	Installer Finished
	******************************

Vorteile
----------

* Durch die Nutzung dieser Nginx Server kann der Benutzer die Anwendung zu konfigurieren.
* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Nginx ist schnell, weil sie nicht brauchen, um einen neuen Prozess für jede neue Anfrage erstellen.
* Nginx verbraucht sehr wenig Speicher, vor allem für statische Webseiten.
* Nginx kann mit einer Vielzahl von Systemen eingesetzt werden.
* Nginx ist hoch skalierbar, und die Leistung ist unabhängig von Hardware.
* Nginx ist einfach zu installieren und zu konfigurieren.
* Wie Apache, Nginx hat alle Funktionen, die Sie von einem führenden Web-Server erwarten würden:
* Statische Datei dient.
* SSL / TLS-Unterstützung.
* Virtuelle Hosts.
* Rück Proxy.
* Der Lastausgleich.
* Compression.
* Zugangskontrollen.
* URL-Rewriting.
* Custom Logging.
* Server-Side Includes.
* WebDAV.
* FLV-Streaming.
* FastCGI.

