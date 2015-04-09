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


 kevell@corp:/#ptconfigure PHPCI install
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 [Pharaoh Logging] Packages php5-mcrypt, curl from the Packager Apt are already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-45785693692.sh
 chmod 755 /tmp/ptconfigure-temp-script-45785693692.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45785693692.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45785693692.sh
 Temp File /tmp/ptconfigure-temp-script-45785693692.sh Removed
 Creating /tmp/ptconfigure-temp-script-47686609771.sh
 chmod 755 /tmp/ptconfigure-temp-script-47686609771.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47686609771.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47686609771.sh
 Module rewrite already enabled
 Temp File /tmp/ptconfigure-temp-script-47686609771.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Composer reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-71236381661.sh
 chmod 755 /tmp/ptconfigure-temp-script-71236381661.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71236381661.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71236381661.sh
 Installing block8/phpci (1.6.0)
   - Installing block8/phpci (1.6.0)
    Loading from cache

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
  - Installing symfony/yaml (v2.6.4)
    Loading from cache

  - Installing block8/b8framework (1.1.9)
    Loading from cache

  - Installing ircmaxell/password-compat (v1.0.4)
    Loading from cache

  - Installing psr/log (1.0.0)
    Loading from cache

  - Installing monolog/monolog (1.12.0)
    Loading from cache

  - Installing pimple/pimple (v1.1.1)
    Loading from cache

  - Installing symfony/console (v2.6.4)
    Loading from cache

  - Installing symfony/filesystem (v2.6.4)
    Loading from cache

  - Installing symfony/config (v2.6.4)
    Loading from cache

  - Installing robmorgan/phinx (v0.4.2.1)
    Loading from cache

  - Installing swiftmailer/swiftmailer (v5.3.1)
    Loading from cache

 Generating autoload files
 Temp File /tmp/ptconfigure-temp-script-42085224634.sh Removed
 Creating /tmp/ptconfigure-temp-script-47565859655.sh
 chmod 755 /tmp/ptconfigure-temp-script-47565859655.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47565859655.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47565859655.sh
 [Pharaoh Logging] Lets begin Configuration of a Web Server for PHPCI
 [Pharaoh Logging] Lets Add our Apache VHost
 [Pharaoh Logging] Now lets restart Apache so we are serving our new application 

 Logging Starting
 Logging Complete
 Logging Starting
 Logging Complete
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.phpci.local
	DocumentRoot /opt/phpci/phpci/public/
	<Directory /opt/phpci/phpci/public/>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Require all granted

        <IfModule mod_rewrite.c>
          RewriteEngine On
          RewriteBase /opt/phpci/phpci/public/
          RewriteCond %{REQUEST_FILENAME} !-f
          RewriteCond %{REQUEST_FILENAME} !-d
          RewriteRule . /index.php [L]
        </IfModule>

	</Directory>

 </VirtualHost>

 Assuming Okay due to yes parameter
 Site www.phpci.local already enabled
 a2ensite www.phpci.local done
 Logging Starting
 Logging Complete
 Temp File /tmp/ptconfigure-temp-script-47565859655.sh Removed
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

.. code-block:: bash

 kevell@corp:/#ptconfigure PHPCI config-default

 Install PHP CI Default Configuration? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPCI Defaults        *
 *******************************
 Set non-default value for db_read_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_write_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_name? Default is phpci (Y/N) 
 n
 Set non-default value for db_username? Default is phpci (Y/N) 
 n
 Set non-default value for db_pass? Default is phpci_pass (Y/N) 
 n
 Set non-default value for phpci_url? Default is http://www.phpci.local (Y/N) 
 n
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ****************************** 

.. code-block:: bash


 kevell@corp:/#ptconfigure phpci install-default-database
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 Database script executed
 ******************************  

 Seems Fine...Database Actions Finished
 ******************************

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ******************************



Vorteile
-----------

* PHPCI verwendet werden, um die Konfiguration und Datenbank-Datei zu installieren. Bei der Installation, ob es eine Datei vorhanden, 
  überschreibt den Inhalt.
* Die neue Version kann automatisch aktualisiert.
* Es können Benutzer Wunsch bei Installation Datenbank übernehmen.
* Continuous Integration ist möglich.
* Mehrere Umwelt
* Erstellen Sie PHP mit verschiedenen Varianten wie PDO, MySQL, SQLite, debuggen ... etc.
* Automatische Feature-Erkennung.

