=========
Citadel
=========


Zusammenfassung
-------------------------

Citadel ist eine komplette und funktionsreiche Open-Source-Groupware-Plattform. Die Zitadelle System ist äußerst vielseitig. Es verfügt über zahlreiche Frontends für die Nutzer, wie eine textbasierte Oberfläche, einer AJAX-Stil Web-Interface und viele gängige PIM-Clients, die SMTP / POP / IMAP zu präsentieren. Alle diese können gleichzeitig verwendet werden.

Es ist auch extrem skalierbar. Sie können nicht nur eine gut ausgestattete Citadel-Server-Unterstützung eine große Anzahl von gleichzeitigen Benutzern, aber Sie können auch bauen ein verteiltes Netzwerk von Citadel-Knoten, die ein Zimmer teilen und deren Inhalte.

Hilfe Befehl
-------------

Dieser Befehl hilft, um die Verwendung von Citadel-Modul zu bestimmen. Der Benutzer wird kommen, über die verschiedenen Möglichkeiten/Format wissen, dieses Modul ausgeführt. Der alternative-Parameter, die in der Deklaration verwendet werden ist klar unter der Hilfe-Option definiert. Dieser Befehl führt den Endbenutzer zu wissen, den Befehl für die Installation. Im folgenden sind der Befehl.

.. code-block:: bash

                cleopatra citadel Help


Die bildliche Darstellung des Screenshots ist nachfolgend aufgeführt,

.. code-block:: bash

 kevell@corp:/# cleopatra Citadel help
 ******************************


 This module installs Citadel Server and provides configuration

 Citadel, citadel-server, citadel

       - install
       Installs Citadel Server
       example: cleopatra citadel install

       - configure
       Configure E-Mail with Citadel Server
       example: cleopatra citadel configure

 ------------------------------
 End Help

Installation
---------------

Wenn der Benutzer Zitadelle Server Maschine installieren muss, können Sie die folgenden Befehle, um die Zitadelle-Suite installieren eingeben. Das System wird der Prozess der Installation ausführen. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

                Install citadel Cleopatra

 kevell@corp:/# cleopatra Citadel install
 Install Citadel Server? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Citadel Server!     *
 *******************************
 Creating /tmp/cleopatra-temp-script-11993825383.sh
 chmod 755 /tmp/cleopatra-temp-script-11993825383.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-11993825383.sh Permissions
 Executing /tmp/cleopatra-temp-script-11993825383.sh
 Temp File /tmp/cleopatra-temp-script-11993825383.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  debconf-utils
 0 upgraded, 1 newly installed, 0 to remove and 228 not upgraded.
 Need to get 57.4 kB of archives.
 After this operation, 157 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main debconf-utils all 1.5.51ubuntu2 [57.4 kB]
 Fetched 57.4 kB in 2s (24.6 kB/s)
 Selecting previously unselected package debconf-utils.
 (Reading database ... 180308 files and directories currently installed.)
 Preparing to unpack .../debconf-utils_1.5.51ubuntu2_all.deb ...
 Unpacking debconf-utils (1.5.51ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up debconf-utils (1.5.51ubuntu2) ...
 [Pharaoh Logging] Adding Package debconf-utils from the Packager Apt executed correctly
 [Pharaoh Logging] Stopping apache2 service
 * Stopping web server apache2
 *
 Creating /tmp/cleopatra-temp-script-74031405363.sh
 chmod 755 /tmp/cleopatra-temp-script-74031405363.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-74031405363.sh Permissions
 Executing /tmp/cleopatra-temp-script-74031405363.sh
 Temp File /tmp/cleopatra-temp-script-74031405363.sh Removed
 apache2_invoke: Enable configuration javascript-common
 invoke-rc.d: initscript apache2, action "reload" failed.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  citadel-client citadel-mta citadel-server citadel-webcit javascript-common
 libc-ares2 libcitadel4 libev4 libjs-prototype libjs-scriptaculous
 libsieve2-1 tinymce
 Suggested packages:
 localepurge
 Recommended packages:
 db4.6-util
 The following NEW packages will be installed:
 citadel-client citadel-mta citadel-server citadel-suite citadel-webcit
 javascript-common libc-ares2 libcitadel4 libev4 libjs-prototype
 libjs-scriptaculous libsieve2-1 tinymce
 0 upgraded, 13 newly installed, 0 to remove and 228 not upgraded.
 Need to get 1,993 kB of archives.
 After this operation, 8,897 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libc-ares2 amd64 1.10.0-2 [38.5 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main javascript-common all 11 [6,066 B]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-prototype all 1.7.1-3 [44.2 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-scriptaculous all 1.9.0-2 [107 kB]
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libsieve2-1 amd64 2.2.6-1.2 [73.1 kB]
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/universe tinymce all 3.4.8+dfsg0-1 [488 kB]
 Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libcitadel4 amd64 8.24-1 [60.5 kB]
 Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-client amd64 8.24-1 [78.5 kB]
 Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libev4 amd64 1:4.15-3 [29.6 kB]
 Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-server amd64 8.24-1 [348 kB]
 Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-mta amd64 8.24-1 [4,520 B]
 Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-webcit amd64 8.24-dfsg-1 [712 kB]
 Get:13 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-suite all 8.24-dfsg-1 [3,542 B]
 Preconfiguring packages ...
 Fetched 1,993 kB in 16s (122 kB/s)
 Selecting previously unselected package libc-ares2:amd64.
 (Reading database ... 180340 files and directories currently installed.)
 Preparing to unpack .../libc-ares2_1.10.0-2_amd64.deb ...
 Unpacking libc-ares2:amd64 (1.10.0-2) ...
 Selecting previously unselected package javascript-common.
 Preparing to unpack .../javascript-common_11_all.deb ...
 Unpacking javascript-common (11) ...
 Selecting previously unselected package libjs-prototype.
 Preparing to unpack .../libjs-prototype_1.7.1-3_all.deb ...
 Unpacking libjs-prototype (1.7.1-3) ...
 Selecting previously unselected package libjs-scriptaculous.
 Preparing to unpack .../libjs-scriptaculous_1.9.0-2_all.deb ...
 Unpacking libjs-scriptaculous (1.9.0-2) ...
 Selecting previously unselected package libsieve2-1.
 Preparing to unpack .../libsieve2-1_2.2.6-1.2_amd64.deb ...
 Unpacking libsieve2-1 (2.2.6-1.2) ...
 Selecting previously unselected package tinymce.
 Preparing to unpack .../tinymce_3.4.8+dfsg0-1_all.deb ...
 Unpacking tinymce (3.4.8+dfsg0-1) ...
 Selecting previously unselected package libcitadel4.
 Preparing to unpack .../libcitadel4_8.24-1_amd64.deb ...
 Unpacking libcitadel4 (8.24-1) ...
 Selecting previously unselected package citadel-client.
 Preparing to unpack .../citadel-client_8.24-1_amd64.deb ...
 Unpacking citadel-client (8.24-1) ...
 Selecting previously unselected package libev4.
 Preparing to unpack .../libev4_1%3a4.15-3_amd64.deb ...
 Unpacking libev4 (1:4.15-3) ...
 Selecting previously unselected package citadel-server.
 Preparing to unpack .../citadel-server_8.24-1_amd64.deb ...
 Unpacking citadel-server (8.24-1) ...
 Selecting previously unselected package citadel-mta.
 Preparing to unpack .../citadel-mta_8.24-1_amd64.deb ...
 Unpacking citadel-mta (8.24-1) ...
 Selecting previously unselected package citadel-webcit.
 Preparing to unpack .../citadel-webcit_8.24-dfsg-1_amd64.deb ...
 Unpacking citadel-webcit (8.24-dfsg-1) ...
 Selecting previously unselected package citadel-suite.
 Preparing to unpack .../citadel-suite_8.24-dfsg-1_all.deb ...
 Unpacking citadel-suite (8.24-dfsg-1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up libc-ares2:amd64 (1.10.0-2) ...
 Setting up javascript-common (11) ...
 * Reloading web server apache2
 *
 * Apache2 is not running
 Setting up libjs-prototype (1.7.1-3) ...
 Setting up libjs-scriptaculous (1.9.0-2) ...
 Setting up libsieve2-1 (2.2.6-1.2) ...
 Setting up tinymce (3.4.8+dfsg0-1) ...
 Setting up libcitadel4 (8.24-1) ...
 Setting up citadel-client (8.24-1) ...
 Adding group `citadel' (GID 126) ...
 Done.
 Adding system user `citadel' (UID 118) ...
 Adding new user `citadel' (UID 118) with group `citadel' ...
 Not creating home directory `/var/lib/citadel'.
 Setting up libev4 (1:4.15-3) ...
 Setting up citadel-server (8.24-1) ...
 Setting up citadel-webcit (8.24-dfsg-1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up citadel-mta (8.24-1) ...
 Setting up citadel-suite (8.24-dfsg-1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package citadel-suite from the Packager Apt executed correctly
 [Pharaoh Logging] Restarting citadel service
 sendcommand: started (pid=4943) connecting to Citadel server at /var/run/citadel/citadel-admin.socket
 200 udayakumar Citadel server ADMIN CONNECTION ready.
 DOWN
 231 Shutting down server.  Goodbye.
 sendcommand: processing ended.
 ....................... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Citadel: Success
 ------------------------------
 Installer Finished
 ******************************



Option
------------

.. cssclass:: table-bordered


 +---------------------------------+-----------------------------------------------+---------------+-----------------------------------------+
 | Parameter			   | Alternative Parameter			   | Optionen	   | Kommentare				     |
 +=================================+===============================================+===============+=========================================+
 |cleopatra Citadel Install?       | Entweder der drei alternativen Parameter      | Y             | Sobald der Benutzer diese Option bietet |
 |(Y/N)                            | können in Befehls verwendet werden -          |               | ,  startet System Installation          |
 |                                 | Citadel, Citadel server, citadel              |               |                                         |
 |                                 | eg: Cleopatra  citadel-server Install         |               |                                         |
 +---------------------------------+-----------------------------------------------+---------------+-----------------------------------------+
 |Cleopatra citadel to install?    | Entweder der drei alternativen Parameter      | N             | Sobald der Benutzer diese Option bietet |
 |(Y / N)                          | können in Befehls verwendet werden -          |               | Das System stoppt den                   | 
 |                                 | Citadel, Citadel server, citadel              |               | Installationsprozess                    |
 |                                 | eg: Cleopatra  citadel-server Install|        |               |                                         |
 +---------------------------------+-----------------------------------------------+---------------+-----------------------------------------+



Konfiguration
-------------------

Dieser Befehl hilft bei der Konfiguration des Servers Zitadelle. Einmal die unten mit dem Befehl wird ausgeführt, das System liefert Ihnen mit dem Standardwert für jeden Abschnitt, wenn es irgendwelche Änderungen erfolgen, der Benutzer kann die Daten bereitstellen. Nachfolgend finden Sie der Befehl für die Konfiguration verwendet.

.. code-block:: bash


                Configure Cleopatra Citadel


Vorteile
-------------

* E-Mail, Kalender/Planung, Adressbücher
* Schwarze Bretter, Mailing-Listen-Server, instant-messaging
* Unterstützung für mehrere Domänen
* Eine intuitive, attraktive AJAX-basierte Web-Oberfläche
 

