===========
PHPModules
===========

Zusammenfassung
-----------------------

Diese Module zielt auf die Installation und Kuvertierung einige der häufigsten und hilfsbereit, die Unterstützung von PHP-Modulen. Einige Beispiele sind: php5-gd das Bild libs, php5-imagick das Bild libs, php5-curl dem entfernten Datei-Handling-Bibliotheken, php5-mysql die Bibliotheken für den Umgang mit MySQL-Verbindungen. Wir wollen sehen, wie dieses Modul, den Prozess der Installation im kommenden Themen verwenden.

Hilfe Befehl
----------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der PHP-Modul enthalten sind. Es listet einige der alternativen Parameter der PHP-Modul. Es beschreibt auch die Syntax für die Installation des PHP-Moduls. Der Befehl help for Php-Modul wird wie unten dargestellt.

.. code-block:: bash
	
		ptconfigure PHPModules help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP-Modul.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************

Installation
--------------

Der Befehl für die Installation der PHP-Module in der Benutzer-Maschine verwendet wird, wie folgt dar:

.. code-block:: bash

		ptconfigure phpmods install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 | Parameters                  | Alternative Parameter                             | Optionen  | Kommentare                              |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 |Install PHP Modules? (Y/N)   | anstelle von phpmods,Die wir verwenden können     | Y(Yes)    | Wenn der Benutzer wünschen, den         |
 |                             | PHPModules, php-mods, php-modules, phpmodules     |           | Installationsprozess können sie Eingang |
 |                             | also.                                             |           | als Y. gehen                            |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 |Install PHP Modules? (Y/N)   | anstelle von phpmods,Die wir verwenden können     | N(No)     | Wenn der Benutzer wünschen, den         |
 |                             | PHPModules, php-mods, php-modules, phpmodules     |           | Installationsprozess können sie Eingang |
 |                             | also.                                             |           | als N. beenden|                         |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+

Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:


* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die Pakete, die automatisch installiert werden.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install

 Install PHP Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 /packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists 
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 php5_invoke: Enable module apcu for cgi SAPI
 php5_invoke: Enable module apcu for cli SAPI
 rmdir: failed to remove â€˜/usr/share/doc/php-apcâ€™: Directory not empty
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  php5-apcu
 Suggested packages:
  php5-gd
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 0 to remove and 252 not upgraded.
 Need to get 75.9 kB of archives.
 After this operation, 344 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-apcu amd64 4.0.2-2build1 [73.2 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe php-apc all 4.0.2-2build1 [2,762 B]
 Fetched 75.9 kB in 42s (1,783 B/s)
 Selecting previously unselected package php5-apcu.
 (Reading database ... 233423 files and directories currently installed.)
 Preparing to unpack .../php5-apcu_4.0.2-2build1_amd64.deb ...
 Unpacking php5-apcu (4.0.2-2build1) ...
 Selecting previously unselected package php-apc.
 Preparing to unpack .../php-apc_4.0.2-2build1_all.deb ...
 Unpacking php-apc (4.0.2-2build1) ...
 Setting up php5-apcu (4.0.2-2build1) ...
 Setting up php-apc (4.0.2-2build1) ...
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt executed correctly
 php5_invoke: Enable module gd for cgi SAPI
 php5_invoke: Enable module gd for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
   php5-gd
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/28.0 kB of archives.
 After this operation, 163 kB of additional disk space will be used.
 Selecting previously unselected package php5-gd.
 (Reading database ... 233448 files and directories currently installed.)
 Preparing to unpack .../php5-gd_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt executed correctly
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
  php5-imagick : Depends: libmagickcore3 (>= 8:6.6.0.4) but it is not installable
                Depends: libmagickwand3 (>= 8:6.6.0.4) but it is not installable
                Depends: libtiff4 but it is not installable
                Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 php5_invoke: Enable module curl for cgi SAPI
 php5_invoke: Enable module curl for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-curl
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/27.4 kB of archives.
 After this operation, 142 kB of additional disk space will be used.
 Selecting previously unselected package php5-curl.
 (Reading database ... 233455 files and directories currently installed.)
 Preparing to unpack .../php5-curl_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 php5-mysql is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 252 not upgraded.
 [Pharaoh Logging] Package php5-mysql from the Packager Apt is already installed, so not installing.
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
 php5-memcache : Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php5-memcached
 0 upgraded, 0 newly installed, 0 to remove and 251 not upgraded.
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 php5_invoke: Enable module mongo for cgi SAPI
 php5_invoke: Enable module mongo for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-mongo
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 94.5 kB of archives.
 After this operation, 334 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-mongo amd64 1.4.5-1build1 [94.5 kB]
 Fetched 94.5 kB in 45s (2,096 B/s)
 Selecting previously unselected package php5-mongo.
 (Reading database ... 233462 files and directories currently installed.)
 Preparing to unpack .../php5-mongo_1.4.5-1build1_amd64.deb ...
 Unpacking php5-mongo (1.4.5-1build1) ...
 Setting up php5-mongo (1.4.5-1build1) ...
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Alle die häufig verwendete PHP-Module der Installation wird in einer einzigen Prozess gehüllt.
