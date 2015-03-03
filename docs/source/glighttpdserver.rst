========================
LigHTTPDServer 
========================

Zusammenfassung
-----------------------

  Lighttpd ist ein Webserver optimiert für Geschwindigkeit kritischen Umgebungen während verbleibenden standardkonforme, sichere und flexible. Es ist eine Alternative für Apache Webserver.

Lighttpd unterstützt die FastCGI, SCGI und CGI-Schnittstellen zu externen Programmen, Auth, Output-Compression, URL-Rewriting und ermöglicht Web-Anwendungen in jeder beliebigen Programmiersprache geschrieben, mit dem Server verwendet werden. Lighttpd sind die besten bekannten asynchronen Server. Der Hauptvorteil des asynchronen Ansatz ist die Skalierbarkeit.

Dieses Modul zielt darauf ab, die neueste Version von Lighttpd-Server und seinen Abhängigkeiten zu installieren.


Hilfe Befehl
--------------

Der Befehl help führt den Anwender zur Verfügung zu stellen, was notwendig ist, um die Aufgabe zu erfüllen. Der Befehl zum Einsatz von dazu beitragen, dass im Rahmen der Terminal wird wie folgt angegeben,

.. code-block:: bash

	ptconfigure lighttpdserver help

Die nachfolgende Snapshots gibt Ihnen eine bildliche Darstellung der Befehl help, und es aufgeführt drei Parameter als LigHTTPDServer, lighttpd-Server, lighttpdserver. (Parameter ist die Groß- und Kleinschreibung)

.. code-block:: bash

	 Kevell@corp:/# ptconfigure LigHTTPDServer help

	 ******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

  	LigHTTPDServer, lighttpd-server, lighttpdserver

        - install
        Installs LigHTTPD HTTP Server
        example: ptconfigure lighttpd-server install

	------------------------------
	End Help
	******************************

Installation
------------------

Der Befehl für die Installation von Lighttpd Modul ist unten angegeben,

.. code-block:: bash

	ptconfigure lighttpd-server  install


.. code-block:: bash

	Kevell@corp:/# ptconfigure lighttpd-server install

	Install LigHTTPD Server? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         LigHTTPD Server!        *
	*******************************
	update-alternatives: warning: not replacing /usr/share/man/man1/spawn-fcgi.1.gz with a link
	2015-01-09 14:45:09: (network.c.405) can't bind to port:  80 Address already in use 
	invoke-rc.d: initscript lighttpd, action "start" failed.
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        gamin libgamin0 libterm-readkey-perl libterm-readline-perl-perl spawn-fcgi
	Suggested packages:
	rrdtool apache2-utils
	The following NEW packages will be installed:
        gamin libgamin0 libterm-readkey-perl libterm-readline-perl-perl lighttpd
        spawn-fcgi
	0 upgraded, 6 newly installed, 0 to remove and 280 not upgraded.
	Need to get 378 kB of archives.
	After this operation, 1,622 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgamin0 amd64 0.1.10-4.1ubuntu1 [16.4 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe gamin amd64 0.1.10-4.1ubuntu1 [41.1 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main libterm-readkey-perl amd64 2.31-1 [27.4 kB]
	Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libterm-readline-perl-perl all 1.0303-1 [51.9 kB]
	Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe lighttpd amd64 1.4.33-1+nmu2ubuntu2 [227 kB]
	Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/universe spawn-fcgi amd64 1.6.3-1 [14.0 kB]
	Fetched 378 kB in 24s (15.2 kB/s)
	Selecting previously unselected package libgamin0.
	(Reading database ... 171800 files and directories currently installed.)
	Preparing to unpack .../libgamin0_0.1.10-4.1ubuntu1_amd64.deb ...
	Unpacking libgamin0 (0.1.10-4.1ubuntu1) ...
	Selecting previously unselected package gamin.
	Preparing to unpack .../gamin_0.1.10-4.1ubuntu1_amd64.deb ...
	Unpacking gamin (0.1.10-4.1ubuntu1) ...
	Selecting previously unselected package libterm-readkey-perl.
	Preparing to unpack .../libterm-readkey-perl_2.31-1_amd64.deb ...
	Unpacking libterm-readkey-perl (2.31-1) ...
	Selecting previously unselected package libterm-readline-perl-perl.
	Preparing to unpack .../libterm-readline-perl-perl_1.0303-1_all.deb ...
	Unpacking libterm-readline-perl-perl (1.0303-1) ...
	Selecting previously unselected package lighttpd.
	Preparing to unpack .../lighttpd_1.4.33-1+nmu2ubuntu2_amd64.deb ...
	Unpacking lighttpd (1.4.33-1+nmu2ubuntu2) ...
	Selecting previously unselected package spawn-fcgi.
	Preparing to unpack .../spawn-fcgi_1.6.3-1_amd64.deb ...
	Unpacking spawn-fcgi (1.6.3-1) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libterm-readkey-perl (2.31-1) ...
	Setting up libterm-readline-perl-perl (1.0303-1) ...
	Setting up spawn-fcgi (1.6.3-1) ...
	update-alternatives: using /usr/bin/spawn-fcgi.standalone to provide /usr/bin/spawn-fcgi (spawn-fcgi) in auto mode
	Setting up gamin (0.1.10-4.1ubuntu1) ...
	Setting up libgamin0 (0.1.10-4.1ubuntu1) ...
	Setting up lighttpd (1.4.33-1+nmu2ubuntu2) ...
	 * Starting web server lighttpd
	   ...fail!
	Processing triggers for libc-bin (2.19-0ubuntu6) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	[Pharaoh Logging] Adding Package lighttpd from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	LigHTTPDServer: Success
	------------------------------
	Installer Finished
	******************************


options
-----------

.. cssclass:: table-bordered

 +-----------------------+-----------------------------------+----------------+------------------------------------------------------+
 | Paramaeters           | Alternative Parameter             | Erforderliche  | Kommentare                                           |
 +=======================+===================================+================+======================================================+
 |ptconfigure            | LigHTTPDServer, lighttpd-server,  | Yes            | Dieser Befehl installiert die LigHTTPD module        |
 |lighttpd-server        | lighttpdserver                    |                |                                                      |
 |install                |                                   |                |                                                      |
 +-----------------------+-----------------------------------+----------------+------------------------------------------------------+
 |Install                | LigHTTPDServer, lighttpd-server,  | Y              | Wenn der Benutzer gibt Y, dieses Modul prüft zuvor   |
 |lighttpd-server(Y/N)   | lighttpdserver                    |                | installierte Version, wenn Ausfahrten wurde auf die  |
 |                       |                                   |                | neueste Version aktualisiert oder er die frische     |
 |                       |                                   |                | Paket installiert.                                   |
 +-----------------------+-----------------------------------+----------------+------------------------------------------------------+
 |Install                | LigHTTPDServer, lighttpd-server,  | N              | Wenn der Benutzer eingibt N wurde die                |
 |lighttpd-server(Y/N)   | lighttpdserver                    |                | Installation abgebrochen.|                           |
 +-----------------------+-----------------------------------+----------------+------------------------------------------------------+



Vorteile für die Nutzer
-----------------------

* Installieren LigHTTPDServer in einer einzigen Umgebung ohne Browser.
* Einfache Anwendung von Zugangs- und Installation
* Coding wird nicht beachtet.
* Nicht Groß- und Kleinschreibung
* Well-to-do in Ubuntu und CentOS.

