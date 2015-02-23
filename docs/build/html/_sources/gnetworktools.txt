=============
NetworkTools
=============


Zusammenfassung
-------------------------

Die Netzwerk-Tools sind Software-Dienstprogramme entwickelt, um zu analysieren und konfigurieren verschiedene Aspekte der Computer-Netzwerk. Die häufigsten Netzwerk-Tools auf den meisten Betriebssystem zu finden sind Traceroute, Netstat und Ping. Jeder Netzwerk-Tools über eine eigene Funktion.

Zum Beispiel:

Es wird verwendet, um die Verbindung zu überprüfen

Netstat wird verwendet, um die Netzwerkverbindung ein- und ausgehende Anzeige

Hilfe Befehl
--------------

Dieser Befehl hilft, die Nutzung von Netzwerktools Modul zu bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl wird dem Endbenutzer zu wissen, wann und wie der Befehl verwendet werden führen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash

		ptconfigure networktools help

Die bildliche Darstellung der obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools help
 ******************************


  This command allows you to install a set of common Network Tools. These include
  traceroute, netstat, lsof, telnet and ps.

  NetworkTools, networktools, network-tools

        - install
        Installs the latest version of Network Tools
        example: ptconfigure networktools install

 ------------------------------
 End Help
 ******************************

Installation
---------------

Wenn der Benutzer benötigt, um jede Netzwerk-Tool in Maschine zu installieren. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash


 	ptconfigure networktool install



.. cssclass:: table-bordered

 +------------------------+-----------------------------------------------+------------+-------------------------------------------+
 | Parameter              | Alternative Parameter                         | Option     | Kommentare                                |
 +========================+===============================================+============+===========================================+
 |Install Network         | Statt NetworkTools, die wir verwenden können  | Y(Yes)     | Wenn der Benutzer wünschen, den           |
 |Tools? (Y/N)            | networktools, network-tools also.             |            | Installationsprozess können sie Eingang   |
 |                        |                                               |            | als Y. gehen                              |
 +------------------------+-----------------------------------------------+------------+-------------------------------------------+
 |Install Network         | Statt NetworkTools, die wir verwenden können  | N(No)      | Wenn der Benutzer wünschen, den           |
 |Tools? (Y/N)            | networktools, network-tools also.             |            | Installationsprozess können sie Eingang   |
 |                        |                                               |            | als N beenden|                            |
 +------------------------+-----------------------------------------------+------------+-------------------------------------------+

Wenn der Benutzer Erlös Installation während des Prozesses der Installation die folgenden Schritte beteiligt sind,

* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools install
 Install Network Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Network Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  traceroute
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 45.0 kB of archives.
 After this operation, 176 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe traceroute amd64 1:2.0.20-0ubuntu0.1 [45.0 kB]
 Fetched 45.0 kB in 4s (10.0 kB/s)
 Selecting previously unselected package traceroute.
 (Reading database ... 182980 files and directories currently installed.)
 Preparing to unpack .../traceroute_1%3a2.0.20-0ubuntu0.1_amd64.deb ...
 Unpacking traceroute (1:2.0.20-0ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up traceroute (1:2.0.20-0ubuntu0.1) ...
 update-alternatives: using /usr/bin/traceroute.db to provide /usr/bin/traceroute (traceroute) in auto mode
 update-alternatives: using /usr/bin/lft.db to provide /usr/bin/lft (lft) in auto mode
 update-alternatives: using /usr/bin/traceproto.db to provide /usr/bin/traceproto (traceproto) in auto mode
 update-alternatives: using /usr/sbin/tcptraceroute.db to provide /usr/sbin/tcptraceroute (tcptraceroute) in auto mode
 [Pharaoh Logging] Adding Package traceroute from the Packager Apt executed correctly
 [Pharaoh Logging] Package netstat from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package lsof from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package telnet from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package ps from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetworkTools: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-----------

Dieses Modul hilft bei der Installation der Reihe gemeinsamer Netzwerk-Tools. Dies kommt der Benutzer verschiedene Werkzeuge, die nützlich sein können bei der Vernetzung mit anderen Computern innerhalb des Netzwerks und über das Internet zu installieren. Dies hilft den Benutzern, die mit Remote-Rechnern arbeiten.

