==============
PostgresServer
==============

Zusammenfassung
----------------------

PostgresServer ist ein universelles und objektrelationalen Datenbankmanagementsystem. Verwenden Sie den Datenbank installieren. PostgresServer entworfen, um auf LINUX-ähnlichen Plattformen. Allerdings ist PostgresServer tragbar, so dass es auf verschiedenen Plattformen wie Mac OS X, Solaris und Windows.

Es ermöglicht Ihnen, benutzerdefinierte Funktionen entwickelt, mit verschiedenen Programmiersprachen wie C / C ++, Java, etc. zu addieren

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von PostgresServer Modul bestimmen. Benutzer werden kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl wird dem Endbenutzer zu wissen, wann und wie der Befehl verwendet werden führen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
          
      ptconfigure PostgresServer help


.. code-block:: bash

	kevell@corp:/# ptconfigure PostgresServer  help
	******************************


        This command allows you to install the Postgres Server. Currently only
	Postgres Workbench, the Database management GUI provided by Oracle for
  	Postgres.

  	PostgresServer, postgres-server, postgresserver

        - install
        Install some Postgres Server Tools through apt-get.
        example: ptconfigure postgres-server install

  	Notes, during postgres install a root password will be set. First, it'll look
  	for the parameter --postgres-root-pass, if this is not set, it'll look in the
  	ptconfigure config for a postgres-default-root-pass setting, and failing both of
  	those it will just set the password for root to ptconfigure.

	------------------------------
	End Help
	******************************


Installation
----------------

Wenn der Benutzer braucht, um das Modul in Maschinen installieren. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
              
      ptconfigure PostgresServer install


Nach der Eingabe des Befehls vor, den Prozess der Ausführung beinhaltet, wie in der in Tabellenform dargestellt,

.. cssclass:: table-bordered

 +------------------------+------------------------------------------------+------------+-----------------------------------------------+
 | Parameters             | Alternative Parameter                          | Options    | Kommentar                                     |
 +========================+================================================+============+===============================================+
 |Install Postgres        | PostgresServer, postgresserver,                | Y          | Wenn der Benutzer wünschen, die Installation  |
 |Server? (Y/N)           | postgres-server. Der Benutzer kann irgendeine  |            | können sie als Eingangs Y. fortzufahren       |
 |                        | der oben genannten Bestimmungen.               |            |                                               |
 +------------------------+------------------------------------------------+------------+-----------------------------------------------+
 |Install Postgres        | PostgresServer, postgresserver,                | N          | Wenn der Benutzer wünschen, um die            |
 |Server? (Y/N)           | postgres-server. Der Benutzer kann irgendeine  |            | Installation zu beenden sie eingeben kann     |
 |                        | der oben genannten Bestimmungen.               |            | als N.|                                       |
 +------------------------+------------------------------------------------+------------+-----------------------------------------------+

Wenn der Benutzer Erlös Installation während des Prozesses der Installation die folgenden Schritte beteiligt sind,

* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die zusätzlichen Pakete, die automatisch installiert werden.
* Liste outs die vorgeschlagenen Pakete, installieren.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure PostgresServer install
 Install Postgres Server? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Postgres Server!        *
 *******************************                                                                                                                                        Adding user postgres to group ssl-cert

 Creating config file /etc/logrotate.d/postgresql-common with new version
 Building PostgreSQL dictionaries from installed myspell/hunspell packages...
  en_us
 Removing obsolete dictionary files:
 * No PostgreSQL clusters exist; see "man pg_createcluster"
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libpq5 postgresql-9.3 postgresql-client-9.3 postgresql-client-common
  postgresql-common
 Suggested packages:
  oidentd ident-server locales-all postgresql-doc-9.3
 The following NEW packages will be installed:
  libpq5 postgresql postgresql-9.3 postgresql-client-9.3
  postgresql-client-common postgresql-common
 0 upgraded, 6 newly installed, 0 to remove and 301 not upgraded.
 Need to get 3,666 kB of archives.
 After this operation, 15.4 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libpq5 amd64 9.3.5-0ubuntu0.14.04.1 [80.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main postgresql-client-common all 154 [25.4 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main postgresql-client-9.3 amd64 9.3.5-0ubuntu0.14.04.1 [782 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/main postgresql-common all 154 [103 kB]
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main postgresql-9.3 amd64 9.3.5-0ubuntu0.14.04.1 [2,670 kB]
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/main postgresql all 9.3+154 [5,088 B]
 Preconfiguring packages ...
 Fetched 3,666 kB in 8min 13s (7,435 B/s)
 Selecting previously unselected package libpq5.
 (Reading database ... 181615 files and directories currently installed.)
 Preparing to unpack .../libpq5_9.3.5-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking libpq5 (9.3.5-0ubuntu0.14.04.1) ...
 Selecting previously unselected package postgresql-client-common.
 Preparing to unpack .../postgresql-client-common_154_all.deb ...
 Unpacking postgresql-client-common (154) ...
 Selecting previously unselected package postgresql-client-9.3.
 Preparing to unpack .../postgresql-client-9.3_9.3.5-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking postgresql-client-9.3 (9.3.5-0ubuntu0.14.04.1) ...
 Selecting previously unselected package postgresql-common.
 Preparing to unpack .../postgresql-common_154_all.deb ...
 Adding 'diversion of /usr/bin/pg_config to /usr/bin/pg_config.libpq-dev by postgresql-common'
 Unpacking postgresql-common (154) ...
 Selecting previously unselected package postgresql-9.3.
 Preparing to unpack .../postgresql-9.3_9.3.5-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking postgresql-9.3 (9.3.5-0ubuntu0.14.04.1) ...
 Selecting previously unselected package postgresql.
 Preparing to unpack .../postgresql_9.3+154_all.deb ...
 Unpacking postgresql (9.3+154) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up libpq5 (9.3.5-0ubuntu0.14.04.1) ...
 Setting up postgresql-client-common (154) ...
 Setting up postgresql-client-9.3 (9.3.5-0ubuntu0.14.04.1) ...
 update-alternatives: using /usr/share/postgresql/9.3/man/man1/psql.1.gz to provide /usr/share/man/man1/psql.1.gz (psql.1.gz) in auto mode
 Setting up postgresql-common (154) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up postgresql-9.3 (9.3.5-0ubuntu0.14.04.1) ...
 Creating new cluster 9.3/main ...
  config /etc/postgresql/9.3/main
  data   /var/lib/postgresql/9.3/main
  locale en_IN
  port   5432
 update-alternatives: using /usr/share/postgresql/9.3/man/man1/postmaster.1.gz to provide /usr/share/man/man1/postmaster.1.gz (postmaster.1.gz) in auto mode
 * Starting PostgreSQL 9.3 database server
   ...done.
 Setting up postgresql (9.3+154) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package postgresql from the Packager Apt executed correctly
 E: Failed to fetch http://in.archive.ubuntu.com/ubuntu/pool/main/p/postgresql-common/postgresql-contrib_9.3+154_all.deb  Connection failed [IP: 91.189.88.149 80]

 E: Unable to fetch some archives, maybe run apt-get update or try with --fix-missing?
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libossp-uuid16 postgresql-contrib-9.3
 Suggested packages:
  uuid libdbd-pg-perl
 The following NEW packages will be installed:
  libossp-uuid16 postgresql-contrib postgresql-contrib-9.3
 0 upgraded, 3 newly installed, 0 to remove and 301 not upgraded.
 Need to get 435 kB of archives.
 After this operation, 2,038 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libossp-uuid16 amd64 1.6.2-1.3ubuntu1 [29.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main postgresql-contrib-9.3 amd64 9.3.5-0ubuntu0.14.04.1 [400 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main postgresql-contrib all 9.3+154 [5,106 B]
 Err http://in.archive.ubuntu.com/ubuntu/ trusty/main postgresql-contrib all 9.3+154
  Connection failed [IP: 91.189.88.149 80]
 Fetched 430 kB in 6min 25s (1,114 B/s)
 [Pharaoh Logging] Adding Package postgresql-contrib from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PostgresServer: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-------------

* Benutzerdefinierte Typen
* Tisch Erbe
* Sophisticated Verriegelung
* Ansichten, Regeln, Unterauswahl
* Verschachtelte Transaktionen (Speicherpunkte)
* Punkt-in-Time-Recovery

