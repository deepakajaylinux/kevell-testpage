===============
ApacheModules
===============

Zusammenfassung
-------------------------
Dieses Modul erleichtert, um die Apache-Module installieren. Es gibt die Konfiguration Ihrer Umgebung. Die Überprüfung Verfügbarkeit der Module ist möglich. Es ist bequem in Ubuntu ebenso wie in Cent OS.

Hilfe Befehl
---------------------


Dieses Help-Befehl wird über den Zweck eines bestimmten Moduls erläutert. Die Syntax für die Installation wird unter dem Help-Befehl dargestellt. Es listet auch heraus die alternative Parameter, die für die Deklaration verwendet werden können. Der Befehl Help ist einfach zu bedienen durch den Endbenutzer. Der folgende Befehl führt den Benutzer über die Verwendung dieses Moduls.

.. code-block:: bash

	 ptconfigure apache modules help

Nachdem er den Befehl gab, listet der Befehl die Hilfeoptionen. Die folgenden Screenshots geben visuellen Effekt für die Nutzung dieses Moduls.

.. code-Block:: bash

 kevell@corp:/# ptconfigure ApacheModules help
 ******************************


  This command is part of Core and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  ApacheModules, apachemods, apache-modules, apachemodules

        - install
        Installs common apache Modules
        example: ptconfigure apache-modules install

 ------------------------------
 End Help
 ******************************


Installation
--------------

Installation ist kein schwieriger Prozess, dieses Modul unter ptconfigure zu installieren, nur mit dem Befehl unten gegeben,

.. code-block:: bash

	Install apache-modules install

After giving the command it will ask,

.. code-block:: bash

	Install Apache module? (Y/N)

	If you give an input as ‘Y’, the module will be installed successfully.
	If you give an input as ‘N’, then it will come out of the installation.

The following screen shots will give visual effect for the installation of this module.

.. code-block:: bash


 kevell@corp:/# ptconfigure apache-modules install

 Install Apache Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Mods!        *
 *******************************
 [Pharaoh Logging] Package libxml2-dev from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-35249017336.sh
 chmod 755 /tmp/ptconfigure-temp-script-35249017336.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-35249017336.sh Permissions
 Executing /tmp/ptconfigure-temp-script-35249017336.sh
 /tmp/ptconfigure-temp-script-35249017336.sh: 1: /tmp/ptconfigure-temp-script-35249017336.sh: a2enmod: not found
 Temp File /tmp/ptconfigure-temp-script-35249017336.sh Removed
 Creating /tmp/ptconfigure-temp-script-68493187412.sh
 chmod 755 /tmp/ptconfigure-temp-script-68493187412.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-68493187412.sh Permissions
 Executing /tmp/ptconfigure-temp-script-68493187412.sh
 /tmp/ptconfigure-temp-script-68493187412.sh: 1: /tmp/ptconfigure-temp-script-68493187412.sh: a2enmod: not found
 Temp File /tmp/ptconfigure-temp-script-68493187412.sh Removed
 Creating /tmp/ptconfigure-temp-script-47826905041.sh
 chmod 755 /tmp/ptconfigure-temp-script-47826905041.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47826905041.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47826905041.sh
 /tmp/ptconfigure-temp-script-47826905041.sh: 1: /tmp/ptconfigure-temp-script-47826905041.sh: a2enmod: not found
 Temp File /tmp/ptconfigure-temp-script-47826905041.sh Removed
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 
 Creating config file /etc/php5/apache2/php.ini with new version
 php5_invoke: Enable module opcache for apache2 SAPI
 php5_invoke: Enable module readline for apache2 SAPI
 php5_invoke: Enable module pdo for apache2 SAPI
 php5_invoke: Enable module mcrypt for apache2 SAPI
 php5_invoke: Enable module json for apache2 SAPI
 apache2_switch_mpm Switch to prefork
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 apache2_invoke: Enable module php5
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   apache2
 Suggested packages:
   apache2-doc apache2-suexec-pristine apache2-suexec-custom apache2-utils
   php-pear
 The following NEW packages will be installed:
  apache2 libapache2-mod-php5
 0 upgraded, 2 newly installed, 0 to remove and 70 not upgraded.
 Need to get 0 B/2,295 kB of archives.
 After this operation, 10.4 MB of additional disk space will be used.
 Selecting previously unselected package apache2.
 (Reading database ... 193229 files and directories currently installed.)
 Preparing to unpack .../apache2_2.4.7-1ubuntu4.4_amd64.deb ...
 Unpacking apache2 (2.4.7-1ubuntu4.4) ...
 Selecting previously unselected package libapache2-mod-php5.
 Preparing to unpack .../libapache2-mod-php5_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.7) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up apache2 (2.4.7-1ubuntu4.4) ...
 * Restarting web server apache2
   ...done.
 Setting up libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.7) ...
 Module mpm_event disabled.
 Enabling module mpm_prefork.
 * Restarting web server apache2
   ...done.
 * Restarting web server apache2
   ...done.
 [Pharaoh Logging] Adding Package libapache2-mod-php5 from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-70188204368.sh
 chmod 755 /tmp/ptconfigure-temp-script-70188204368.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-70188204368.sh Permissions
 Executing /tmp/ptconfigure-temp-script-70188204368.sh
 Module php5 already enabled
 Temp File /tmp/ptconfigure-temp-script-70188204368.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheModules: Success
 ------------------------------
 Installer Finished
 ******************************





Option
-----------

.. cssclass:: table-bordered

 +-------------------------+-----------------------+---------------------------------------------------------------+
 | Parameter               | Erforderlich          | Kommentare 					           |
 +=========================+=======================+===============================================================+
 |Install Apache           | Yes		   | Wenn der Benutzer gibt Eingabe als Ja, wird das Modul zu      |
 |Module? (Y/N)            |                       | installieren                                                  |
 +-------------------------+-----------------------+---------------------------------------------------------------+
 |Install Apache           | No                    | Wenn der Benutzer gibt Eingang als nicht, wird sie beendet    |
 |Module? (Y/N)            |                       | werden.|                                                      |
 +-------------------------+-----------------------+---------------------------------------------------------------+

Vorteile 
--------

* Das Modul ist eine Hilfe für Link mit ptconfigure.
* Während der Installation des Apache-Module, werden es die Konfigurationsdateien hinnehmen.
* Wenn die Konfigurationsdateien nicht im System vorhanden sind werden Sie dieses Modul automatisch installiert.





 

