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

	 cleopatra apache modules help

Nachdem er den Befehl gab, listet der Befehl die Hilfeoptionen. Die folgenden Screenshots geben visuellen Effekt für die Nutzung dieses Moduls.

.. code-Block:: bash

 kevell@corp:/# cleopatra ApacheModules help
 ******************************


  This command is part of Core and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  ApacheModules, apachemods, apache-modules, apachemodules

        - install
        Installs common apache Modules
        example: cleopatra apache-modules install

 ------------------------------
 End Help
 ******************************


Installation
--------------

Installation ist kein schwieriger Prozess, dieses Modul unter Cleopatra zu installieren, nur mit dem Befehl unten gegeben,

.. code-block:: bash

	Install apache-modules install

After giving the command it will ask,

.. code-block:: bash

	Install Apache module? (Y/N)

	If you give an input as ‘Y’, the module will be installed successfully.
	If you give an input as ‘N’, then it will come out of the installation.

The following screen shots will give visual effect for the installation of this module.

.. code-block:: bash

 kevell@corp:/#  cleopatra apache-modules install
 Install Apache Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Mods!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libxml2-dev
 0 upgraded, 1 newly installed, 0 to remove and 229 not upgraded.
 Need to get 630 kB of archives.
 After this operation, 2,928 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libxml2-dev amd64 2.9.1+dfsg1-3ubuntu4.4 [630 kB]
 Fetched 630 kB in 2min 38s (3,990 B/s)
 Selecting previously unselected package libxml2-dev:amd64.
 (Reading database ... 181481 files and directories currently installed.)
 Preparing to unpack .../libxml2-dev_2.9.1+dfsg1-3ubuntu4.4_amd64.deb ...
 Unpacking libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 [Pharaoh Logging] Adding Package libxml2-dev from the Packager Apt executed correctly
 Creating /tmp/cleopatra-temp-script-11435369770.sh
 chmod 755 /tmp/cleopatra-temp-script-11435369770.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-11435369770.sh Permissions
 Executing /tmp/cleopatra-temp-script-11435369770.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-11435369770.sh Removed
 Creating /tmp/cleopatra-temp-script-95277456152.sh
 chmod 755 /tmp/cleopatra-temp-script-95277456152.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-95277456152.sh Permissions
 Executing /tmp/cleopatra-temp-script-95277456152.sh
 Considering dependency filter for deflate:
 Module filter already enabled
 Module deflate already enabled
 Temp File /tmp/cleopatra-temp-script-95277456152.sh Removed
 Creating /tmp/cleopatra-temp-script-1351048337.sh
 chmod 755 /tmp/cleopatra-temp-script-1351048337.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-1351048337.sh Permissions
 Executing /tmp/cleopatra-temp-script-1351048337.sh
 Considering dependency setenvif for ssl:
 Module setenvif already enabled
 Considering dependency mime for ssl:
 Module mime already enabled
 Considering dependency socache_shmcb for ssl:
 Enabling module socache_shmcb.
 Enabling module ssl.
 See /usr/share/doc/apache2/README.Debian.gz on how to configure SSL and create self-signed certificates.
 To activate the new configuration, you need to run:
   service apache2 restart
 Temp File /tmp/cleopatra-temp-script-1351048337.sh Removed
 [Pharaoh Logging] Package libapache2-mod-php5 from the Packager Apt is already installed, so not installing
 Creating /tmp/cleopatra-temp-script-89813944614.sh
 chmod 755 /tmp/cleopatra-temp-script-89813944614.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-89813944614.sh Permissions
 Executing /tmp/cleopatra-temp-script-89813944614.sh
 Module php5 already enabled
 Temp File /tmp/cleopatra-temp-script-89813944614.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 Output of config test was:
 apache2: Syntax error on line 214 of /etc/apache2/apache2.conf: Could not open configuration file /etc/apache2/httpd.conf: No such file or 
 directory 
 Action 'configtest' failed.
 The Apache error log may have more information.
 * Restarting web server apache2
   ...fail!
 * The apache2 configtest failed.
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

* Das Modul ist eine Hilfe für Link mit Kleopatra.
* Während der Installation des Apache-Module, werden es die Konfigurationsdateien hinnehmen.
* Wenn die Konfigurationsdateien nicht im System vorhanden sind werden Sie dieses Modul automatisch installiert.





 

