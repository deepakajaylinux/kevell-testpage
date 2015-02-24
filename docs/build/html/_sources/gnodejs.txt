=========
NodeJS
=========

Zusammenfassung
-------------------------

Dieses Modul hilft den Benutzern, die ein Knoten JS Server Side JS Sprache zu installieren. Node.js ist ein Open Source, plattformübergreifende Laufzeitumgebung für serverseitige und Netzwerkanwendungen. Node.js Anwendungen in JavaScript geschrieben und kann innerhalb der Laufzeit Node.js auf OS X, Microsoft Windows, Linux und FreeBSD laufen. Hier wollen wir sehen, wie funktioniert das Modul ermöglicht in Installation und Verwendung des Node-JS.

Hilfe Befehl
---------------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der Node-JS-Modul enthalten sind. Der Befehl help Listen aus der alternativen Parameter Node-JS-Modul. Es beschreibt auch die Syntax für die Installation von Node-JS-Modul. Der Befehl help für Node-JS-Modul ist wie unten dargestellt.

.. code-block:: bash

		ptconfigure NodeJS help
Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Node JS.

.. code-block:: bash
		


 kevell@corp:/# ptconfigure NodeJS help
 ******************************


  This command allows you to install Node JS, The Server Side JS Language

  NodeJS, node-js, nodejs

        - install
        Installs NodeJS through apt-get.
        example: ptconfigure node-js install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Installation des Node-JS zu Ihrer Maschine, können einfach mit Hilfe des folgenden Befehls, wie gezeigt durchgeführt werden:

.. code-block:: bash

		ptconfigure node-js install

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered


 +-------------------------+------------------------------------------+---------------+------------------------------------------+
 | Parameter               | Alternative Parameter                    | Option        | Kommentare                               |
 +=========================+==========================================+===============+==========================================+
 |Install Node JS? (Y/N)   | Trotz Node JS, NodeJS, node-js, nodejs   | Y(Yes)        | Wenn der Benutzer wünschen, den          |
 |                         | können ebenfalls verwendet werden.       |               | Installationsprozess können sie Eingang  |
 |                         |                                          |               | als Y. gehen                             |
 +-------------------------+------------------------------------------+---------------+------------------------------------------+
 |Install Node JS? (Y/N)   | Trotz Node JS, NodeJS, node-js, nodejs   | N(No)         | Wenn der Benutzer wünschen, den          |
 |                         | können ebenfalls verwendet werden.       |               | Installationsprozess können sie Eingang  |
 |                         |                                          |               | als N. gehen|                            |
 +-------------------------+------------------------------------------+---------------+------------------------------------------+



Wenn der Benutzer den Installationsprozess fort, während der Ausführung der Installation wird der folgende Prozess durchgeführt:

* Liest Paketlisten.
* Baut Abhängigkeitsbaum.
* Liest Statusinformationen.
* Liste der Pakete, die automatisch installiert werden.
* Liste der neuen Pakete installiert.
* Listet die Anzahl der Dateien, die aktualisiert werden, neu installiert, entfernt wird, nicht aktualisiert.

Schließlich werden die Berichte und Status klar ausgewiesen. Und auch das Hinzufügen Paket nodejs vom Packager Apt korrekt ausgeführt. Der folgende Screenshot zeigt den gesamten Prozess der Installation, wie beschrieben.

Wenn der Knoten-js-Modul wird bereits in der Maschine vorhandenen Benutzer, wird eine Meldung wie die Knoten Paket-js vom Verpacker Apt bereits installiert ist zu zeigen. Der Screenshot wie folgt ist ein gutes Beispiel für jene Art von Nachrichten.

.. code-block:: bash

 kevell@corp:/# ptconfigure node-js install
 Install Node JS? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Node JS!        *
 *******************************
	Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  ax25-node libax25 openbsd-inetd
 The following NEW packages will be installed:
  ax25-node libax25 node openbsd-inetd
 0 upgraded, 4 newly installed, 0 to remove and 17 not upgraded.
 Need to get 110 kB of archives.
 After this operation, 465 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libax25 amd64 0.0.12-rc2+cvs20120204-2ubuntu2 [22.7 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main openbsd-inetd amd64 0.20091229-2ubuntu3 [30.8 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/universe ax25-node amd64 0.3.2-7.4 [54.8 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/universe node all 0.3.2-7.4 [1,284 B]
 Fetched 110 kB in 2s (39.1 kB/s)
 Selecting previously unselected package libax25.
 (Reading database ... 237551 files and directories currently installed.)
 Preparing to unpack .../libax25_0.0.12-rc2+cvs20120204-2ubuntu2_amd64.deb ...
 Unpacking libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Selecting previously unselected package openbsd-inetd.
 Preparing to unpack .../openbsd-inetd_0.20091229-2ubuntu3_amd64.deb ...
 Unpacking openbsd-inetd (0.20091229-2ubuntu3) ...
 Selecting previously unselected package ax25-node.
 Preparing to unpack .../ax25-node_0.3.2-7.4_amd64.deb ...
 Unpacking ax25-node (0.3.2-7.4) ...
 Selecting previously unselected package node.
 Preparing to unpack .../node_0.3.2-7.4_all.deb ...
 Unpacking node (0.3.2-7.4) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Setting up openbsd-inetd (0.20091229-2ubuntu3) ...
 * Stopping internet superserver inetd
   ...done.
 * Not starting internet superserver: no services enabled
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up ax25-node (0.3.2-7.4) ...
 Setting up node (0.3.2-7.4) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package node from the Packager Apt executed correctly
            
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libv8-3.14.5
 The following NEW packages will be installed:
  libv8-3.14.5 nodejs
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 1,873 kB of archives.
 After this operation, 7,429 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libv8-3.14.5 amd64 3.14.5.8-5ubuntu2 [1,189 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe nodejs amd64 0.10.25~dfsg2-2ubuntu1 [684 kB]
 Fetched 1,873 kB in 14s (126 kB/s)
 Selecting previously unselected package libv8-3.14.5.
 (Reading database ... 237621 files and directories currently installed.)
 Preparing to unpack .../libv8-3.14.5_3.14.5.8-5ubuntu2_amd64.deb ...
 Unpacking libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Selecting previously unselected package nodejs.
 Preparing to unpack .../nodejs_0.10.25~dfsg2-2ubuntu1_amd64.deb ...
 Unpacking nodejs (0.10.25~dfsg2-2ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Setting up nodejs (0.10.25~dfsg2-2ubuntu1) ...
 update-alternatives: using /usr/bin/nodejs to provide /usr/bin/js (js) in auto mode
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package nodejs from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NodeJS: Success
 ------------------------------
 Installer Finished

Vorteile
------------

* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Wenn der Knoten-js Paket bereits in der Benutzermaschine vorhandenen, wird es nicht überschreibt, statt dass er eine Nachricht zu zeigen, wie   bereits existieren.
* Node.js nutzt die Google V8 JavaScript-Engine, um Code auszuführen, und ein großer Prozentsatz der Grundmodule sind in JavaScript geschrieben.
   Node.js enthält eine integrierte Bibliothek, damit Anwendungen als Web-Server, ohne Software zu handeln, wie Apache HTTP Server oder IIS.

