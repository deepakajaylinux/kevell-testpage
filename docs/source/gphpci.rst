===============
Phpci
===============

Zusammenfassung
-------------------------

   PHPCI ist ein Open Source kontinuierliche Integration-Tool speziell für ptconfigure konzipiert. Der Anwender haben es mit Einfachheit an erster Stelle, so dass, während sie nicht alles Jenkins tun kann, ist es ein Kinderspiel zu installieren und zu verwenden. Dies ist die Leichtigkeit, mit Ubuntu und Cent-OS.

Hilfe Befehl
-----------------------

 Dieser Befehl help führen den Anwender auf bestimmte Operation zu Phpci Zustand durch. Dies eignet sich für alle Arten von Unternehmenskunden.

.. code-block:: bash
   
                ptconfigure PHPCI help


The help command shows a short list of the commands built into the Phpci module. The following screen shot visualize it.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCI help
 ******************************


  This command allows you to install PHPCI, the popular Build Server.

  PHPCI, phpci

        - install
        Installs PHPCI through git, with its dependencies
        example: ptconfigure phpci install

        - config-default, default-config
        Installs a default config.yml file for PHPCI
        example: ptconfigure phpci config-default --yes --guess

        - install-default-database
        Installs a default database and user for PHPCI
        example: ptconfigure phpci install-default-database --yes --guess
            --mysql-admin-user="root" # guess will provide root
            --mysql-admin-pass="some-pass" # guess will provide ptconfigure

  You can install a complete local version of PHPCI with the following:

  sudo ptconfigure phpci install --yes --guess
  sudo ptconfigure phpci install-default-database --yes --guess
  sudo ptconfigure phpci config-default --yes --guess

 ------------------------------
 End Help
 ******************************

Installation
-----------------

 Dieses Modul hilft, phpci installieren. Der erste Schritt dieses Modul müssen Komponisten zu überprüfen, ist im System verfügbar ist oder nicht. Wenn es im System nicht verfügbar ist automatisch, wird er es zu installieren.

.. code-block:: bash

                   ptconfigure Phpci install


Nach der Eingabe des Befehls oben, sind die folgenden Verfahren während des Prozesses der Installation beteiligt, wie in der Tabellenform dargestellt,

.. cssclass:: table-bordered

 +-------------------------+-----------------------------------------+-------------+-------------------------------------------+
 | Parameters              | Alternative Parameter                   | Optionen    | Kommentare                                |
 +=========================+=========================================+=============+===========================================+
 |Install PHPCI? (Y/N)     | anstelle von PHPCI, , wir verwenden     | Y(Yes)      | Wenn der Benutzer wünschen, den           |
 |                         | können, phpci also.                     |             | Installationsprozess können sie Eingang   |
 |                         |                                         |             | als Y. gehen                              |
 +-------------------------+-----------------------------------------+-------------+-------------------------------------------+
 |Install PHPCI? (Y/N)     | anstelle von PHPCI, , wir verwenden     | N(No)       | Wenn der Benutzer wünschen, den           |
 |                         | können, phpci also.                     |             | Installationsprozess können sie Eingang   |
 |                         |                                         |             | als N. beenden|                           |
 +-------------------------+-----------------------------------------+-------------+-------------------------------------------+

Wenn der Benutzer Erlös Installation während des Prozesses der Installation die folgenden Schritte beteiligt sind,

* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die zusätzlichen Pakete, die automatisch installiert werden.
* Liste outs die vorgeschlagenen Pakete, installieren.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Und dann wird sie fragt Eingabe von den Benutzern, wie in tabellarischer Form dargestellt

.. cssclass:: table-bordered

 +--------------------------+------------------------------+------------------+----------------------------------------------------+
 | Parameter                | Weg                          | Optionen         | Kommentare                                         |
 +==========================+==============================+==================+====================================================+
 |Program data              | “/opt/phpunit(entsprechend   | Yes              | Wenn der Benutzer die Installation mit dem         |
 |directory (Default)       |  Modul)”                     |                  | Standard-Programm-Daten-Verzeichnis gehen sie      |
 |                          |                              |                  | eingeben kann als Ja                               |
 +--------------------------+------------------------------+------------------+----------------------------------------------------+
 |Program data directory    | User Specific                | No(End Slash)    | Wenn der Benutzer mit ihren eigenen                |
 |                          |                              |                  | Programmdatenverzeichnis fortfahren möchten,       |
 |                          |                              |                  | können sie Eingang als N, und in die Hand geben    |
 |                          |                              |                  | sie Ort besitzen.                                  |
 +--------------------------+------------------------------+------------------+----------------------------------------------------+
 |Program executor          | “/usr/bin”                   | Yes              | Wenn der Benutzer die Installation mit dem         |
 |directory (Dafault)       |                              |                  | Standardprogramm Testamentsvollstrecker            |
 |                          |                              |                  | Verzeichnis gehen sie eingeben kann als Ja.        |
 +--------------------------+------------------------------+------------------+----------------------------------------------------+
 |Program executor          | User specific                | No(End Slash)    | Wenn der Benutzer mit ihren eigenen                |
 |directory                 |                              |                  | Programmausführungs Verzeichnis fortfahren möchten |
 |                          |                              |                  | , können sie Eingang als N, und in die Hand geben  |
 |                          |                              |                  | sie Ort besitzen.|                                 |
 +--------------------------+------------------------------+------------------+----------------------------------------------------+



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash

 kevell@corp:/#  ptconfigure phpci install
 Install PHPCI? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libmcrypt4
 Suggested packages:
  libmcrypt-dev mcrypt
 The following NEW packages will be installed:
  libmcrypt4 php5-mcrypt
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 77.3 kB of archives.
 After this operation, 324 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmcrypt4 amd64 2.5.8-3.1ubuntu1 [61.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php5-mcrypt amd64 5.4.6-0ubuntu5 [15.4 kB]
 Fetched 77.3 kB in 4s (19.1 kB/s)
 Selecting previously unselected package libmcrypt4.
 (Reading database ... 182037 files and directories currently installed.)
 Preparing to unpack .../libmcrypt4_2.5.8-3.1ubuntu1_amd64.deb ...
 Unpacking libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Selecting previously unselected package php5-mcrypt.
 Preparing to unpack .../php5-mcrypt_5.4.6-0ubuntu5_amd64.deb ...
 Unpacking php5-mcrypt (5.4.6-0ubuntu5) ...
 Setting up libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Setting up php5-mcrypt (5.4.6-0ubuntu5) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package php5-mcrypt from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-82480901916.sh
 chmod 755 /tmp/ptconfigure-temp-script-82480901916.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-82480901916.sh Permissions
 Executing /tmp/ptconfigure-temp-script-82480901916.sh
 Temp File /tmp/ptconfigure-temp-script-82480901916.sh Removed
 Creating /tmp/ptconfigure-temp-script-43828918328.sh
 chmod 755 /tmp/ptconfigure-temp-script-43828918328.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-43828918328.sh Permissions
 Executing /tmp/ptconfigure-temp-script-43828918328.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-43828918328.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: composer: not found
 [Pharaoh Logging] Module Composer reports itself as Not Installed
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...


 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 Creating /tmp/ptconfigure-temp-script-34508236330.sh
 chmod 755 /tmp/ptconfigure-temp-script-34508236330.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-34508236330.sh Permissions
 Executing /tmp/ptconfigure-temp-script-34508236330.sh
 #!/usr/bin/env php
 Installing block8/phpci (1.5.2)
  - Installing block8/phpci (1.5.2)
    Downloading: 100%

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
 Warning: The lock file is not up to date with the latest changes in composer.json. You may be getting outdated dependencies. Run update to update them.
 Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - The requested PHP extension ext-pdo_mysql * is missing from your system.

 Temp File /tmp/ptconfigure-temp-script-34508236330.sh Removed
 Creating /tmp/ptconfigure-temp-script-28990655696.sh
 chmod 755 /tmp/ptconfigure-temp-script-28990655696.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-28990655696.sh Permissions
 Executing /tmp/ptconfigure-temp-script-28990655696.sh
 sudo: dapperstrano: command not found
 Temp File /tmp/ptconfigure-temp-script-28990655696.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCI: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
--------

* PHPCI verwendet werden, um die Konfiguration und Datenbank-Datei zu installieren. Bei der Installation, ob es eine Datei vorhanden, 
  überschreibt den Inhalt.
* Die neue Version kann automatisch aktualisiert.
* Es können Benutzer Wunsch bei Installation Datenbank übernehmen.
* Continuous Integration ist möglich.
* Mehrere Umwelt
* Erstellen Sie PHP mit verschiedenen Varianten wie PDO, MySQL, SQLite, debuggen ... etc.
* Automatische Feature-Erkennung.

