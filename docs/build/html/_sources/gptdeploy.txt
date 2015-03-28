==================
PTDeploy
==================

Zusammenfassung
----------------

Die ptdeploy umhüllt die Anwendungen der Nutzer mit automatisierte Bereitstellung , Aufbau und Release -Funktionen , Web- App Versionierung und Infrastruktur -Code in PHP.

Um gut Einsatz zu bauen, werden viele Dateien benötigt, um von FTP- oder anderen Ad-hoc -Lösungen kopiert werden. Und auch viele Unternehmen Automation Werkzeuge fehlten. Um diese Engpässe ptdeploy unter dem Pharao Werkzeug überwunden waren aufzubauen . PHP hat ptdeploy wie Rubin fiils die Lücke in ptdeploy .

Dieses Tool ist für die Bereitstellung Anwendungen und baut auf Ihre Boxen. Der Benutzer kann mit einem oder zwei PHP-Dateien Oder schnell Setup Cloud freundliche Bereitstellungsmustern einzurichten sogar einfache oder komplexe Anwendungsbereitstellungsmusterfür ihr System .

ptdeploy ist modular, objektorientiert und erweiterbar . Also, wenn der Benutzer keine zusätzlichen Module erfordert sie erstellen und die neuen Module auf der Basis ihrer Anforderungen .

Diese ptdeploy fungiert als Wrapper , wo alle Schritte Benutzerbereitstellungin einer einzigen Datei abgedeckt zu werden. Auf diese Weise können mit einem einzigen Befehl zu feuern eine Instanz Ihrer Anwendungen.

Hilfe Befehl
----------------------

Diese Funktion dient , um die Verwendung von ptdeploy Modul bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender , um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
         ptconfigure ptdeploy help

Der Screenshot für den obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy help
 ******************************


  This command allows you to update ptdeploy.

  ptdeploy, dapper, ptdeploy

        - install
        Installs the latest version of ptdeploy
        example: ptconfigure ptdeploy install

        - ensure
        Installs the latest version of ptdeploy, only if a version is not installed
        example: ptconfigure ptdeploy ensure

 ------------------------------
 End Help
 ******************************

Installation
----------------

Dieser Befehl hilft, die neueste Version von ptdeploy installieren. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
        
        ptconfigure ptdeploy install

Der Screenshot für den obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy install


 Install ptdeploy? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ptdeploy         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-30110448761.sh
 chmod 755 /tmp/ptconfigure-temp-script-30110448761.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-30110448761.sh Permissions
 Executing /tmp/ptconfigure-temp-script-30110448761.sh
 Cloning into 'ptdeploy'...
 remote: Counting objects: 7006, done.
 remote: Total 7006 (delta 0), reused 0 (delta 0), pack-reused 7006
 Receiving objects: 100% (7006/7006), 2.62 MiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (4349/4349), done.
 Checking connectivity... done.
 Temp File /tmp/ptconfigure-temp-script-30110448761.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************


Dafür Sorgen
----------------

Dieser Befehl hilft, die neueste Version von ptdeploy zu installieren, nur dann, wenn eine Version nicht installiert. Die unten angegebenen Befehl wird den Prozess der Installation auszuführen.

.. code-block:: bash
        
        ptconfigure ptdeploy ensure

Der Screenshot für den obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************




Options
-----------                               

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------------+------------+---------------------------------------+
 | Parameter               | Alternative Parameter                        | Optionen   | Kommentare                            |
 +=========================+==============================================+============+=======================================+
 |ptconfigure ptdeploy     | Es gibt zwei alternative Parameter,          | Y          | System startet Installation           |
 |install? (Y/N)           | können in der Befehlszeile verwendet werden. |            |                                       |
 |                         | ptdeploy, dapper, ptdeploy                   |            |                                       |
 |                         | Beispiel: ptconfigure ptdeploy install /     |            |                                       |
 |                         | ptconfigure dapper install                   |            |                                       |
 +-------------------------+----------------------------------------------+------------+---------------------------------------+
 |ptconfigure ptdeploy     | Es gibt zwei alternative Parameter,          | N          | Das System stoppt den                 |
 |install? (Y/N)           | können in der Befehlszeile verwendet werden. |            | Installationsprozess                  |
 |                         | ptdeploy, dapper, ptdeploy                   |            |                                       |
 |                         | Beispiel: ptconfigure ptdeploy install /     |            |                                       |
 |                         | ptconfigure dapper install|                  |            |                                       |
 +-------------------------+----------------------------------------------+------------+---------------------------------------+


Vorteile
--------------

* Bearbeiten der Host-Dateien , virtuellen Host -Dateien , Konfigurationsdateien , Datenbankupdates und alle mit dieser automatisiert werden.
* Durch die Verwendung der Fähigkeit der Remote-Server -Management, können die Benutzer -Bereitstellungen in Infrastruktur jeder Größe zu 
  automatisieren.
