============
Cleopatra
============

Synopsis
----------

Dieses Modul Aufzugsanlage in aktualisierte Version. Automation möglich. Standort für Datenverzeichnis und Vollstrecker Verzeichnis kann bei der Installation dieses Moduls angegeben werden. Es gibt die Konfiguration Ihrer Umgebung. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.
Hilfe command

Dieser Befehl help führen den Benutzer zu Cleopatra. Geeignet für alle Arten von Benutzer. Es stellt die alternative Parameter und Befehle für die Installation. Der folgende Befehl help, und der Screenshot wird der Benutzer über die Nutzung zu unterstützen.

.. code-block:: bash

	cleopatra Cleopatra help

.. code-block:: bash



 kevell@corp:/# cleopatra Cleopatra help
 ******************************


 This command allows you to update Cleopatra.

 Cleopatra, cleo, cleopatra

 - install
 Installs the latest version of cleopatra
 example: cleopatra cleopatra install

 ------------------------------
 End Help
 ******************************



Installation
------------------

Es ist eine einfachere Verfahren zu Cleopatra Modul nur mit dem Befehl unten angegeben zu installieren,

.. code-block:: bash

	cleopatra Cleopatra install

Nachdem er den Befehl der Kleopatra mit neuen Updates installiert werden.

Nachdem die Benutzereingabe verstrichen ist es zu überprüfen, ob eine Datei fehlt, und in der Hand wird es automatisch zu installieren.

Der folgende Screenshot aufzuzählen es.


.. code-block:: bash

 kevell@corp:/# cleopatra cleopatra install

 Install Cleopatra - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          Cleopatra!         *
 *******************************
 What is the program data directory? Found "/opt/cleopatra" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/cleopatra.git'  /tmp/cleopatra/cleopatraCloning into '/tmp/cleopatra/cleopatra'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/cleopatra Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Cleopatra: Success
 ------------------------------
 Installer Finished
 ******************************



Option
--------

.. cssclass:: table-bordered


 +---------------------------------------------+---------------+----------------------------------------------+
 | Parameter 				       | Option	       | Kommentare				      |
 +=============================================+===============+==============================================+
 |Install cleopatra cleopatra Update to        | Y(YES)        | Es wird Cleopatra installieren unter         |
 |latest version? (Y/N)			       |               | Cleopatra				      |
 +---------------------------------------------+---------------+----------------------------------------------+
 |Install cleopatra cleopatra Update to        | N(NO)	       | Es wird die Installation zu beenden	      |
 |latest version? (Y/N)|		       |               | 				              |
 +---------------------------------------------+---------------+----------------------------------------------+



Vorteile
-----------


* Cleopatra wird verwendet, um Konfigurationsdatei zu installieren. Bei der Installation, ob es eine Datei überschreiben den Inhalt bestehende.
* Neue Version automatisch aktualisiert.
* Updation können in diesem Modul ohne Web-Suche durchgeführt werden.
