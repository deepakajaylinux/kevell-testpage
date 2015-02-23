================
MysqlTools
================

Zusammenfassung
-------------------------

Dieses Modul soll die Installation einige Tools, die den MySQL-Server unterstützt. Es erleichtert auch bei der Installation der MySQL Workbench GUI und sowie mytop Command Line Tool.

Hilfe Befehl
----------------

Der Befehl help weist die Benutzer im Umgang mit diesem Modul. Darüber hinaus wird es auch bestimmt die alternative Parameter. Der Befehl für die Hilfe-Option verwendet, ist wie folgt:

.. code-block:: bash

	ptconfigure MysqlTools help

Der Befehl help gibt auch den Befehl für die Installation dieses mysqltools Modul. Schauen Sie sich die Screenshots unten angegeben.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools help

 ******************************


  This command allows you to install some tools to help with MySQL Server. Installs the MySQL
  Workbench GUI and also the mytop Command Line Tool.

  MysqlTools, mysql-tools, mysqltools

        - install
        Installs Mysql Tools through apt-get.
        example: ptconfigure mysql-tools install

 ------------------------------
 End Help
 ******************************

Installation
-------------

Dieses Modul installiert die MySQL-Tools, die den MySQL-Server mit Hilfe von apt-get unterstützt. Der Befehl für die Installation mysqltools Ihr Gerät verwendet wird, wie folgt dar:

.. code-block:: bash

	ptconfigure MysqlTools install


.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------------------+------------+-------------------------------------------+
 | Parameter                | Alternative Parameter                               | Option     | Kommentare                                |
 +==========================+=====================================================+============+===========================================+
 |Install MySQL Tools?      | An der Stelle Mysql Werkzeuge diese alternative     | Y(Yes)     | Wenn der Benutzer wünschen, den           |
 |(Y/N)                     | Namen können verwendet werden: MysqlTools,          |            | Installationsprozess können sie Eingang   |
 |                          | , mysql-tools, mysqltools.                          |            | als Y. gehen                              |
 +--------------------------+-----------------------------------------------------+------------+-------------------------------------------+
 |Install MySQL Tools?      | An der Stelle Mysql Werkzeuge diese alternative     | N(No)      | Wenn der Benutzer wünschen, den           |
 |(Y/N)                     | Namen können verwendet werden: MysqlTools,          |            | Installationsprozess können sie Eingang   |
 |                          | , mysql-tools, mysqltools.                          |            | als N. gehen|                             |
 +--------------------------+-----------------------------------------------------+------------+-------------------------------------------+

.. rubric:: Wenn der Benutzer gehen Installation der MySQL-Tools werden die folgenden Operationen durchgeführt, während der Installation

* Es liest die Paketlisten.
* Erstellt die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Installiert die zusätzlichen Pakete, die erforderlich sind.
* Installiert die vorgeschlagenen Pakete.
* Installiert die neue Pakete.
* Zeigt die Anzahl der Dateien, die aktualisiert wurden, neu installiert, entfernt und nicht aktualisiert.

Der Screenshot siehe unten gibt Ihnen eine grafische Darstellung über die Schritte, wie oben erklärt.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools install

 Install MySQL Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Tools!        *
 *******************************
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
 mysql-workbench : Depends: libmysqlcppconn7 (>= 1.1.3) but it is not installabl                                                                                        e
                   Recommends: ttf-bitstream-vera but it is not going to be inst                                                                                        alled
                   Recommends: mysql-utilities but it is not going to be install                                                                                        ed
 [Pharaoh Logging] Adding Package mysql-workbench from the Packager Apt did not e                                                                                        xecute correctly
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libconfig-inifiles-perl
 The following NEW packages will be installed:
  libconfig-inifiles-perl mytop
 0 upgraded, 2 newly installed, 0 to remove and 13 not upgraded.
 Need to get 73.8 kB of archives.
 After this operation, 288 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main libconfig-inifiles-perl                                                                                         all 2.68-1 [39.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mytop all 1.9.1-1 [34                                                                                        .1 kB]
 Fetched 73.8 kB in 7s (10.5 kB/s)
 Selecting previously unselected package libconfig-inifiles-perl.
 (Reading database ... 254866 files and directories currently installed.)
 Preparing to unpack .../libconfig-inifiles-perl_2.68-1_all.deb ...
 Unpacking libconfig-inifiles-perl (2.68-1) ...
 Selecting previously unselected package mytop.
 Preparing to unpack .../archives/mytop_1.9.1-1_all.deb ...
 Unpacking mytop (1.9.1-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libconfig-inifiles-perl (2.68-1) ...
 Setting up mytop (1.9.1-1) ...
 [Pharaoh Logging] Adding Package mytop from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlTools: Success
 ------------------------------
 Installer Finished
 ******************************

Es wird auch gibt den Namen der Werkzeuge, die installiert sind, beispielsweise

.. code-block:: bash


.. rubric::  mysql-server-core-5.5:amd64, mysql-server-5.5: amd64, libaio1:amd64, mysql-server:amd64.

Vorteile
----------

* Der Benutzer kann die benötigten Werkzeuge zu installieren, dass MySQL Server unterstützt.
* Es erleichtert auch bei der Installation der MySQL Workbench GUI und sowie mytop Command Line Tool.
* Nach der Installation, wird es zeigt die Werkzeuge Listen, die neu installiert werden.
