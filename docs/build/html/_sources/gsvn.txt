=======
SVN
=======

Zusammenfassung
-----------------------

Dieses Modul hilft den Benutzern, die neueste Version von SVN in Ubuntu zu installieren. Apache Subversion (oft abgekürzt SVN, hinter den Befehlen svn) ist ein Software-Versionierung und Versionskontrollsystem verteilt als freie Software unter der Apache-Lizenz. [1] Entwickler benutzen Subversion auf aktuelle und frühere Versionen von Dateien wie Quellcode zu erhalten, Web-Seiten und Dokumentation. Ziel ist es, ein weitgehend kompatibel Nachfolger des weit verbreiteten Concurrent Versions System (CVS) sein. Wir wollen sehen, wie dieses Modul ermöglicht in Installieren, Deinstallieren, die Gewährleistung der Subversion in Ubuntu.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der SVN enthalten sind. Es listet einige der alternativen Parameter SVN. Es beschreibt auch die Syntax für die Installation, Deinstallation, die Gewährleistung der SVN. Der Befehl help zur SVN-Modul wird wie unten dargestellt.

.. code-block:: bash
	
		ptconfigure svn help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter SVN.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn help
 ******************************


  This command allows you to install the latest available SVN in the Ubuntu
  repositories.

  SVN, svn

        - install
        Installs the latest available (In your package manager) version of SVN
        example: ptconfigure svn install

        - ensure
        Ensures SVN is installed
        example: ptconfigure svn ensure

        - uninstall
        Installs the latest version of SVN
        example: ptconfigure svn uninstall

 ------------------------------
 End Help
 ******************************

Installation
---------------

Der Befehl für die Installation des SVN auf die Ubuntu verwendet, wird unten gezeigt.

.. code-block:: bash
		
		ptconfigure svn install

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge als in Tabellenform dargestellt.

.. cssclass:: table-bordered

 +------------------------+----------------------------------------+--------------+---------------------------------------+
 | Parameters             | Alternative Parameter                  | Option       | Kommentare                            |
 +========================+========================================+==============+=======================================+
 |Install SVN? (Y/N)      | anstelle von SVN, wir verwenden        | Y(Yes)       | Wenn der Benutzer wünschen, den       |
 |                        | können, svn also                       |              | Installationsprozess können sie       |
 |                        |                                        |              | Eingang als Y. gehen                  |
 +------------------------+----------------------------------------+--------------+---------------------------------------+
 |Install SVN? (Y/N)      | anstelle von SVN, wir verwenden        | N(No)        | Wenn der Benutzer wünschen, den       |
 |                        | können, svn also                       |              | Installationsprozess können sie       |
 |                        |                                        |              | Eingang als N. beenden|               |
 +------------------------+----------------------------------------+--------------+---------------------------------------+

Wenn der Benutzer den Installationsprozess fort, während der Ausführung der Installation wird der folgende Prozess durchgeführt:

* Liest Paketlisten.
* Baut Abhängigkeitsbaum.
* Liest Statusinformationen.
* Führt Sie zusätzliche Pakete installiert.
* Listet neue Pakete installiert.
* Anzahl der Dateien aktualisiert, neu installiert, entfernt wird, nicht aktualisiert.
* Schließlich ist die Installation von SVN abgeschlossen wird. Der folgende Screenshot zeigt Sie den Prozess der Installation SVN in Ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn install
 Install SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libserf-1-1 libsvn1
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  libserf-1-1 libsvn1 subversion
 0 upgraded, 3 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,240 kB of archives.
 After this operation, 4,701 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libserf-1-1 amd64 1.3.3-1ubuntu0.1 [42.2 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libsvn1 amd64 1.8.8-1ubuntu3.1 [917 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main subversion amd64 1.8.8-1ubuntu3.1 [280 kB]
 Fetched 1,240 kB in 43s (28.3 kB/s)
 Selecting previously unselected package libserf-1-1:amd64.
 (Reading database ... 211229 files and directories currently installed.)
 Preparing to unpack .../libserf-1-1_1.3.3-1ubuntu0.1_amd64.deb ...
 Unpacking libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Selecting previously unselected package libsvn1:amd64.
 Preparing to unpack .../libsvn1_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Selecting previously unselected package subversion.
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Setting up libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

Un installieren
---------------------

Der Befehl für un Installation des SVN auf die Ubuntu verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure svn uninstall

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +---------------------+-----------------------------------------+--------------+---------------------------------------------------+
 | Parameters          | Alternative Parameter                   | Option       | Kommentare                                        |
 +=====================+=========================================+==============+===================================================+
 |Uninstall SVN? (Y/N) | anstelle von SVN, wir verwenden können, | Y(Yes)       | Wenn der Benutzer den Wunsch, un-Installation     |
 |                     | svn also                                |              | durchgeführt werden können sie Eingang als Y.     |
 +---------------------+-----------------------------------------+--------------+---------------------------------------------------+
 |Uninstall SVN? (Y/N) | anstelle von SVN, wir verwenden können, | N(No)        | Wenn der Benutzer wünschen, die un-Installation   |
 |                     | svn also                                |              | können sie Eingang als N beenden|                 |
 +---------------------+-----------------------------------------+--------------+---------------------------------------------------+

Wenn der Benutzer die un Installationsprozess, geht während der Ausführung des un-Installation geschieht Folgendes:

* Liest Paketlisten.
* Baut Abhängigkeitsbaum.
* Liest Statusinformationen.
* Führt aus Paketen, die automatisch installiert werden.
* Führt Sie Pakete, die entfernt werden.
* Anzahl der Dateien aktualisiert, neu installiert, entfernt wird, nicht aktualisiert.

Schließlich ist die un-Installation des SVN abgeschlossen wird. Der folgende Screenshot zeigt Ihnen über den Prozess der Installation un SVN in Ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn uninstall
 Uninstall SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 [Pharaoh Logging] Removing Package subversion
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  libserf-1-1 libsvn1
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  subversion
 0 upgraded, 0 newly installed, 1 to remove and 8 not upgraded.
 After this operation, 1,425 kB disk space will be freed.
 (Reading database ... 211322 files and directories currently installed.)
 Removing subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package subversion from the Packager Apt
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

Dafür Sorgen
-----------------

Der Befehl zur Sicherstellung SVN verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure svn ensure

Das Verfahren gewährleistet die folgenden Funktionen:

* Es wird sichergestellt, ob das Modul installiert ist oder nicht, und nicht überprüft die Version.
* Wenn das Modul bereits installiert ist, wird darstellen, wie es bereits vorhanden ist.
* Wenn das Modul nicht in der Benutzermaschine, dann wird es Installation fortzufahren.

Die folgenden Screenshots zeigt den Prozess der Sicherstellung.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: svn: not found
 [Pharaoh Logging] Module SVN reports itself as Not Installed 
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  subversion
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 0 B/280 kB of archives.
 After this operation, 1,425 kB of additional disk space will be used.
 Selecting previously unselected package subversion.
 (Reading database ... 211282 files and directories currently installed.)
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

Vorteile
-----------

* Die in Deklaration der Hilfe und Installationen, deinstallieren verwendeten Parameter, sicherzustellen, muss nicht beachtet werden, welche 
  zusätzlichen Vorteil, während es im Vergleich zu anderen.
* Der Benutzer kann über die Verfügbarkeit, bevor Sie mit der Installation zu gewährleisten.
* Es wird nicht überschreiben, die Pakete, daher ist es weniger zeitaufwendig.

