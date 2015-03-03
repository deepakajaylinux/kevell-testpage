===========
VNC
===========

Zusammenfassung
-----------------------

Dieses Modul bietet Unterstützung für die Installation vnc4server via apt get. Es ermöglicht Konnektivität für virtuelle Maschine. Es erleichtert die Gewährleistung vor der Installation.

Hilfe Befehl
--------------

Der Befehl help liefert ein Bewusstsein für die VNC-Modul. Es beschreibt auch über die Optionen, die im Rahmen dieser VNC-Modul durchgeführt werden können.

Die Hilfe-Befehl für diesen VNC-Modul ist unten angegeben,

.. code-block:: bash

	ptconfigure vnc help

Der Screenshot unten angegebenen zeigt Ihnen eine bildliche Darstellung über die Nutzung der Hilfebefehl unter VNC-Modul.

.. code-block:: bash

 Kevell@corp:/# ptconfigure vnc help
 ******************************


        This command allows you to install VNC, the popular Virtual Machine Solution.

	 VNC, vnc

        - install
        Installs VNC through apt-get
        example: ptconfigure vnc install

	------------------------------
	End Help
	******************************


Installation
-------------
.. code-block:: bash
	
		ptconfigure vnc install

Der Screenshot unten angegebenen zeigt Ihnen eine bildliche Darstellung über die Nutzung der Hilfebefehl unter VNC-Modul.

.. cssclass:: table-bordered

 +-------------------------+----------------------------+------------------+------------------------------------------------------+
 | Parameters              | Alternative parameters     | Erforderliche    | Kommentar                                            |
 +=========================+============================+==================+======================================================+
 |Install VNC? (Y/N)       | VNC, vnc                   | Y(Yes)           | Wenn der Benutzer Wunsch, mit Installation           |
 |                         |                            |                  | fortzusetzen, können sie Eingang als Y.              |
 +-------------------------+----------------------------+------------------+------------------------------------------------------+
 |Install VNC? (Y/N)       | VNC, vnc                   | N(NO)            | Wenn der Benutzer wünschen, um die Installation zu   |
 |                         |                            |                  | beenden, sie einfach mit N. beenden kann|            |
 +-------------------------+----------------------------+------------------+------------------------------------------------------+

Bei der Installation des VNC-Server es die folgenden Operationen wie unten angegeben:

* Liest die Paketlisten, Statusinformationen,
* Erstellt die Abhängigkeitsstruktur.
* Installiert die xbase-Kunden als zusätzlichen Pakete, VNC-Java-Pakete, wie vorgeschlagen.
* Installiert vnc4server xbase-Kunden als neue Pakete.
* Es zeigt auch die Anzahl der Dateien aktualisiert, neu installiert, entfernt wird, nicht aktualisiert.

Der Screenshot wie unten angegeben, werden die Nutzer grafisch über den Prozess der Installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  xbase-clients
 Suggested packages:
  vnc-java
 The following NEW packages will be installed:
  vnc4server xbase-clients
 0 upgraded, 2 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,579 kB of archives.
 After this operation, 5,418 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe xbase-clients all 1:7.7+1ubuntu8 [2,752 B]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vnc4server amd64 4.1.1+xorg4.3.0-37ubuntu5.0.1 [1,577 kB]
 Fetched 1,579 kB in 33s (46.6 kB/s)
 Selecting previously unselected package xbase-clients.
 (Reading database ... 211210 files and directories currently installed.)
 Preparing to unpack .../xbase-clients_1%3a7.7+1ubuntu8_all.deb ...
 Unpacking xbase-clients (1:7.7+1ubuntu8) ...
 Selecting previously unselected package vnc4server.
 Preparing to unpack .../vnc4server_4.1.1+xorg4.3.0-37ubuntu5.0.1_amd64.deb ...
 Unpacking vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xbase-clients (1:7.7+1ubuntu8) ...
 Setting up vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 update-alternatives: using /usr/bin/vnc4server to provide /usr/bin/vncserver (vncserver) in auto mode
 update-alternatives: using /usr/bin/Xvnc4 to provide /usr/bin/Xvnc (Xvnc) in auto mode
 update-alternatives: using /usr/bin/x0vnc4server to provide /usr/bin/x0vncserver (x0vncserver) in auto mode
 update-alternatives: using /usr/bin/vnc4passwd to provide /usr/bin/vncpasswd (vncpasswd) in auto mode
 update-alternatives: using /usr/bin/vnc4config to provide /usr/bin/vncconfig (vncconfig) in auto mode
 [Pharaoh Logging] Adding Package vnc4server from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************

Wenn der VNC-Server in der Benutzer-Maschine bereits vorhanden ist, wird es eine Ausnahme auslöst Nachricht wie der VNC-Server installiert ist. Die folgende Abbildung gibt eine bildliche Darstellung in Bezug auf die Ausnahmemeldung.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 [Pharaoh Logging] Package vnc4server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************


Vorteile
---------------

* Es ermöglicht, den Prozess der Sicherung vor dem Einbau.
* Es erleichtert die Installation via apt get.
* Es ermöglicht die virtuelle Maschine Konnektivität.
* Bei VNC-Server ist bereits vorhanden sind, außergewöhnliche Nachricht wirft ihn während des Prozesses zu gewährleisten.

