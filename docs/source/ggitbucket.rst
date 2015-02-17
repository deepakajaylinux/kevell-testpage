=============
Gitbucket
=============

Zusammenfassung
------------------------

Git ist ein verteiltes Versionskontrollsystem mit einem Schwerpunkt auf Geschwindigkeit, Datensicherheit und Unterstützung für verteilte, nicht-linearen Workflows. Git ist die weit verbreitete Versionskontrollsystem für die Softwareentwicklung.

Git-Arbeitsverzeichnis ist ein vollwertiges Repository mit kompletten Geschichte und der Vollversion-Tracking-Funktionen, unabhängig von Netzwerkzugang oder einen zentralen Server.

GitBucket ist das einfach zu installierende Github-Klon mit Scala geschrieben. Es bietet eine grundlegende Funktionen im Handumdrehen:

* Öffentliche / Private Git-Repository ( http Zugriff)
* Repository-Viewer (einige erweiterte Funktionen wie Online-Dateibearbeitung sind nicht implementiert)
* Repository suchen (Kodex und Ausgaben)
* Wiki
* Fragen
* Gabel / Pull-Request
* E-Mail-Benachrichtigung
* Activity Timeline
* Benutzerverwaltung (für Administratoren)
* Gruppe (wie Organisation in Github)
* LDAP-Integration
* Gravatar Unterstützung
* Ausführbare WAR-Dat

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von gitbucket Modul bestimmen. Der Benutzer kommt, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Befehls- und die Bildschirm

.. code-block:: bash
     
                cleopatra gitbucket help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/$ cleopatra gitbucket help
 ******************************
  This command allows you to install a full Git Bucket installation on to a server
  The dependencies for GitBucket are also installed.

  GitBucket, gitbucket, git-bucket

        - install
        Installs the latest version of GitBucket on a system
        example: cleopatra gitbucket install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Wenn der Benutzer muss gitbucket Modul in Maschine zu installieren. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.
Während der Installation wird das System fordern Repository-Stammverzeichnis. Der Benutzer muss den Pfad zu definieren. Es gibt keine Standard-Verzeichnis.

.. code-block:: bash
       
                cleopatra gitbucket install


The screenshot for the above command is listed below,

.. code-block:: bash

 kevell@corp:/$ cleopatra gitbucket install
 Install Git Bucket? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !GitBucket!        *
 *******************************
 PHP Notice:  Undefined index: version in /opt/cleopatra/cleopatra/src/Modules/GitBucket/Model/GitBucketUbuntu.php on line 67
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Command 'git' found
 [Pharaoh Logging] No command 'gitk' found
 [Pharaoh Logging] No command 'git-cola' found
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  git-core
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 1,458 B of archives.
 After this operation, 21.5 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main git-core all 1:1.9.1-1ubuntu0.1 [1,458 B]
 Fetched 1,458 B in 1s (783 B/s)
 Selecting previously unselected package git-core.
 (Reading database ... 182763 files and directories currently installed.)
 Preparing to unpack .../git-core_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking git-core (1:1.9.1-1ubuntu0.1) ...
 Setting up git-core (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package git-core from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 2s (43.1 kB/s)
 Selecting previously unselected package gitk.
 (Reading database ... 182764 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 301 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 13s (27.8 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 182782 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package libjs-underscore.
 Preparing to unpack .../libjs-underscore_1.4.4-2ubuntu1_all.deb ...
 Unpacking libjs-underscore (1.4.4-2ubuntu1) ...
 Selecting previously unselected package git-cola.
 Preparing to unpack .../git-cola_1.9.3-1_all.deb ...
 Unpacking git-cola (1.9.3-1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up libjs-underscore (1.4.4-2ubuntu1) ...
 Setting up git-cola (1.9.3-1) ...
 [Pharaoh Logging] Adding Package git-cola from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/cleopatra-temp-script-15361773074.sh
 chmod 755 /tmp/cleopatra-temp-script-15361773074.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-15361773074.sh Permissions
 Executing /tmp/cleopatra-temp-script-15361773074.sh
 Cloning into 'gitbucket-war'...
 remote: Counting objects: 8, done.
 remote: Total 8 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (8/8), done.
 Checking connectivity... done.
 mkdir: cannot create directory ‘/opt/gitbucket/’: Permission denied
 mv: target ‘/opt/gitbucket/’ is not a directory
 Temp File /tmp/cleopatra-temp-script-15361773074.sh Removed
 Enter Repository Root Directory:
 /
 Program Executor Deleted if existed
 PHP Warning:  file_put_contents(/usr/bin/gitbucket): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/BaseLinuxApp.php on line 312
 chmod: cannot access ‘/usr/bin/gitbucket’: No such file or directory
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 GitBucket: Success
 ------------------------------
 Installer Finished
 ******************************

Optionen
----------

.. cssclass:: table-bordered

        +-----------------------------+------------------------+-----------------------+-----------------------------------------------+
        |       Parameter             | Alternative Parameter  |        Option         |                Kommentare                     |
        +=============================+========================+=======================+===============================================+
        |cleopatra  gitbucket Install |GitBucket, gitbucket ,  |Y                      |System startet Installation                    |
        |                             |git-bucket              |                       |                                               |
        +-----------------------------+------------------------+-----------------------+-----------------------------------------------+
        |cleopatra  gitbucket Install |GitBucket, gitbucket ,  |N                      |                                               |
        |                             |git-bucket              |                       |Das System stoppt den Installations|           |
        +-----------------------------+------------------------+-----------------------+-----------------------------------------------+

Vorteile
--------------

* Git unterstützt die schnelle Verzweigen und Zusammenführen und enthält spezielle Werkzeuge zur Visualisierung und Navigation einer 
  nicht-linearen Entwicklung der Geschichte.
* Repositories können über HTTP, FTP, rsync oder einem Git-Protokoll entweder über eine einfache Steckdose oder ssh veröffentlicht.
* Git beschrieben als sehr schnelle, skalierbare und zeigte es sich um eine Größenordnung schneller als einige Versionskontrollsysteme und das 
  Abrufen Versionsgeschichte von einer lokal gespeicherten Repository kann hundert Mal schneller als das Abrufen aus dem Remote-Server sein.
* Die Schlüsselwörter in Changelogs sind mit den entsprechenden Ausgabe Seiten verlinkt, Pull Requests Seiten und Wiki-Seiten.
* Die Änderungsliste und diff in Änderungsprotokolle werden GitBucket Repository Viewer verlinkt.
* Lösen Sie einen Build, wenn eine Änderung an GitBucket mit einem WebHooks geschoben.
