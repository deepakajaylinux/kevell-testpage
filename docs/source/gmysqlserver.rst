===============
Mysqlserver
===============

Zusammenfassung
----------------------

Dieses Modul fungiert als Vermittler, um MySQL-Server mit der aktualisierten Version über apt-get install. Wenn der MySQL-Server in Ihrer Maschine bereits vorhanden ist, wird es überprüft die Verfügbarkeit der neu aktualisierte Modul.

Der Befehl help
--------------------

Der Befehl help führt den Anwender in Bezug auf die Methodik in der Nutzung sowie über die Maßnahmen, die im Rahmen dieser Module durchgeführt werden können. Es beschreibt auch die alternative Namen für die mysql-server. Der Befehl für die Verwendung von Hilfe-Option ist unten angegeben

.. code-block:: bash

	ptconfigure  mysql-server help

Dieser Befehl erlaubt den Benutzern, sich seiner Aufgabe und auch über den Befehl für die Installation der MySQL-Server verwendet wird.

Der Screenshot unten angegeben eine bildliche Darstellung über den Befehl Hilfe.

.. code-block:: bash


 kevell@corp:/# ptconfigure  MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure  mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure  config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure .

 ------------------------------
 End Help
 ******************************

Installation
--------------

Der Befehl für die Installation der MySQL-Server verwendet, wird unten gegeben.

.. code-block:: bash

	ptconfigure  mysql-server install

Während der Installation wird der folgende Prozess
---------------------------------------------------------

* Dieses Modul hilft, einige Werkzeuge für MySQL-Server via installieren apt-get.
* Zunächst wird ein Root-Passwort gesetzt.
* Bei der Installation, wird es für einen Parameter --mysql-root Pass suchen.
* Wenn die --mysql-root Pass nicht verfügbar ist, wird sie die Kleopatra Config für die Einstellungen der mysql-default-root Pass suchen.
* Bei den beiden oben genannten Schritte wird versagt, wird es, indem Sie root-Passwort zu Kleopatra gehen.

Zusätzliche Optionen
------------------------

Lassen Sie uns über, die zusätzliche Optionen bei der Installation der MySQL-Server beteiligt sehen.

.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------------+------------+------------------------------------------+
 | Parameters               | Verzeichnis (Standard)                          | Optionen   | Kommentare                               |
 +==========================+=================================================+============+==========================================+
 |Install MySQL Server?     | An der Stelle MySQL Server diese alternative    | Y(Yes)     | Wenn der Benutzer wünschen, den          |
 |(Y/N)                     | Namen können verwendet werden: MysqlServer,     |            | Installationsprozess können sie Eingang  |
 |                          | mysql-server, mysqlserver.                      |            | als Y. gehen                             |
 +--------------------------+-------------------------------------------------+------------+------------------------------------------+
 |Install MySQL Server?     | An der Stelle MySQL Server diese alternative    | N(No)      | Wenn der Benutzer wünschen, den          |
 |(Y/N)                     | Namen können verwendet werden: MysqlServer,     |            | Installationsprozess können sie Eingang  |
 |                          | mysql-server, mysqlserver.                      |            | als N beenden|                           |
 +--------------------------+-------------------------------------------------+------------+------------------------------------------+


Der folgende Screenshot gibt Ihnen eine grafische Darstellung über den Installationsprozess.


.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-46222435876.sh
 chmod 755 /tmp/ptconfigure-temp-script-46222435876.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-46222435876.sh Permissions
 Executing /tmp/ptconfigure-temp-script-46222435876.sh
 Temp File /tmp/ptconfigure-temp-script-46222435876.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libdbd-mysql-perl libdbi-perl libterm-readkey-perl mysql-client-5.5
  mysql-client-core-5.5
 Suggested packages:
  libclone-perl libmldbm-perl libnet-daemon-perl libplrpc-perl
  libsql-statement-perl
 The following NEW packages will be installed:
  libdbd-mysql-perl libdbi-perl libterm-readkey-perl mysql-client
  mysql-client-5.5 mysql-client-core-5.5
 0 upgraded, 6 newly installed, 0 to remove and 172 not upgraded.
 Need to get 2,315 kB/3,321 kB of archives.
 After this operation, 40.1 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client-core-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [710 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [1,592 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client all 5.5.41-0ubuntu0.14.04.1 [12.3 kB]
 Fetched 2,315 kB in 44s (51.7 kB/s)
 Selecting previously unselected package libdbi-perl.
 (Reading database ... 232987 files and directories currently installed.)
 Preparing to unpack .../libdbi-perl_1.630-1_amd64.deb ...
 Unpacking libdbi-perl (1.630-1) ...
 Selecting previously unselected package libdbd-mysql-perl.
 Preparing to unpack .../libdbd-mysql-perl_4.025-1_amd64.deb ...
 Unpacking libdbd-mysql-perl (4.025-1) ...
 Selecting previously unselected package libterm-readkey-perl.
 Preparing to unpack .../libterm-readkey-perl_2.31-1_amd64.deb ...
 Unpacking libterm-readkey-perl (2.31-1) ...
 Selecting previously unselected package mysql-client-core-5.5.
 Preparing to unpack .../mysql-client-core-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-client-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-client-5.5.
 Preparing to unpack .../mysql-client-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-client-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-client.
 Preparing to unpack .../mysql-client_5.5.41-0ubuntu0.14.04.1_all.deb ...
 Unpacking mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libdbi-perl (1.630-1) ...
 Setting up libdbd-mysql-perl (4.025-1) ...
 Setting up libterm-readkey-perl (2.31-1) ...
 Setting up mysql-client-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Setting up mysql-client-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Setting up mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 [Pharaoh Logging] Adding Package mysql-client from the Packager Apt executed correctly
 Aborting downgrade from (at least) 5.6 to 5.5.
 If are sure you want to downgrade to 5.5, remove the file
 /var/lib/mysql/debian-*.flag and try installing again.
 dpkg: error processing archive /var/cache/apt/archives/mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb (--unpack):
  subprocess new pre-installation script returned error exit status 1
 Errors were encountered while processing:
  /var/cache/apt/archives/mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb
 E: Sub-process /usr/bin/dpkg returned an error code (1)
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   libaio1 libhtml-template-perl mysql-server-5.5 mysql-server-core-5.5
 Suggested packages:
   libipc-sharedcache-perl tinyca mailx
 The following NEW packages will be installed:
  libaio1 libhtml-template-perl mysql-server mysql-server-5.5
  mysql-server-core-5.5
 0 upgraded, 5 newly installed, 0 to remove and 172 not upgraded.
 Need to get 4,964 kB/5,036 kB of archives.
 After this operation, 53.0 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server-core-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [3,207 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [1,744 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server all 5.5.41-0ubuntu0.14.04.1 [12.4 kB]
 Preconfiguring packages ...
 Fetched 4,964 kB in 1min 5s (75.8 kB/s)
 Selecting previously unselected package libaio1:amd64.
 (Reading database ... 233242 files and directories currently installed.)
 Preparing to unpack .../libaio1_0.3.109-4_amd64.deb ...
 Unpacking libaio1:amd64 (0.3.109-4) ...
 Selecting previously unselected package mysql-server-core-5.5.
 Preparing to unpack .../mysql-server-core-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-server-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-server-5.5.
 Preparing to unpack .../mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Selecting previously unselected package libhtml-template-perl.
 Preparing to unpack .../libhtml-template-perl_2.95-1_all.deb ...
 Unpacking libhtml-template-perl (2.95-1) ...
 Selecting previously unselected package mysql-server.
 Preparing to unpack .../mysql-server_5.5.41-0ubuntu0.14.04.1_all.deb ...
 Unpacking mysql-server (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package mysql-server from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************




Wenn der MySQL-Server gibt es in Ihrem Computer bereits, dann wird es eine Meldung an den Benutzer zu werfen, wie es bereits installiert ist. Der folgende Screenshot stellt den Prozess der Sicherstellung:


.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-23889189196.sh
 chmod 755 /tmp/ptconfigure-temp-script-23889189196.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23889189196.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23889189196.sh
 Temp File /tmp/ptconfigure-temp-script-23889189196.sh Removed
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************



Vorteile
----------

* Bei der Installation der MySQL-Server, installiert es mit der aktualisierten Version.
* Es sorgt dafür, vor der Installation, und überprüfen Sie die Verfügbarkeit von Modulen.
* Im Falle von neuen Modulen in der aktualisierten Version enthalten ist, wird das fehlende Modul einzeln installiert werden.
* Es prüft die Verfügbarkeit der Bibliotheksfunktionen in der MySQL-Server.
