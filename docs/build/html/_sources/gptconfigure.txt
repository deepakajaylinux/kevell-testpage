============
PTConfigure
============

Synopsis
----------

Dieses Modul Aufzugsanlage in aktualisierte Version. Automation möglich. Standort für Datenverzeichnis und Vollstrecker Verzeichnis kann bei der Installation dieses Moduls angegeben werden. Es gibt die Konfiguration Ihrer Umgebung. Es ist benutzerfreundlich mit Ubuntu und Cent-OS.
Hilfe command

Dieser Befehl help führen den Benutzer zu ptconfigure. Geeignet für alle Arten von Benutzer. Es stellt die alternative Parameter und Befehle für die Installation. Der folgende Befehl help, und der Screenshot wird der Benutzer über die Nutzung zu unterstützen.

.. code-block:: bash

	ptconfigure ptconfigure help

.. code-block:: bash



 kevell@corp:/# ptconfigure ptconfigure help
 ******************************


 This command allows you to update ptconfigure.

 ptconfigure, cleo, ptconfigure

 - install
 Installs the latest version of ptconfigure
 example: ptconfigure ptconfigure install

 ------------------------------
 End Help
 ******************************



Installation
------------------

Es ist eine einfachere Verfahren zu ptconfigure Modul nur mit dem Befehl unten angegeben zu installieren,

.. code-block:: bash

	ptconfigure ptconfigure install

Nachdem er den Befehl der ptconfigure mit neuen Updates installiert werden.

Nachdem die Benutzereingabe verstrichen ist es zu überprüfen, ob eine Datei fehlt, und in der Hand wird es automatisch zu installieren.

Der folgende Screenshot aufzuzählen es.


.. code-block:: bash

 kevell@corp:/# ptconfigure ptconfigure install

 Install ptconfigure - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          PTConfigure!         *
 *******************************
 What is the program data directory? Found "/opt/ptconfigure" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptconfigure.git'  /tmp/ptconfigure/ptconfigureCloning into '/tmp/ptconfigure/ptconfigure'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/ptconfigure Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptconfigure: Success
 ------------------------------
 Installer Finished
 ******************************



Option
--------

.. cssclass:: table-bordered


 +-------------------------------------------+------------------------------------+---------+-----------------------------------------+
 | Parameter 				     | Alternative Parameter              | Option  | Kommentare		              |
 +===========================================+====================================+=========+=========================================+
 |Install ptconfigure ptconfigure Update to  | Anstelle von ptconfigure wir       | Y(YES)  | Es wird ptconfigure installieren unter  |
 |latest version? (Y/N)			     | verwenden können, ptconfigure,     |         | ptconfigure			      |
 |                                           | cleo du auch                       |         |                                         |
 +-------------------------------------------+------------------------------------+---------+-----------------------------------------+
 |Install ptconfigure ptconfigure Update to  | Anstelle von ptconfigure wir       | N(NO)   | Es wird die Installation zu beenden     |
 |latest version? (Y/N) 	             | verwenden können, ptconfigure,     |         | ptconfigure	                      |
 |                                           | cleo du auch|                      |         |                                         |
 +-------------------------------------------+------------------------------------+---------+-----------------------------------------+



Vorteile
-----------


* ptconfigure wird verwendet, um Konfigurationsdatei zu installieren. Bei der Installation, ob es eine Datei überschreiben den Inhalt
  bestehende.
* Neue Version automatisch aktualisiert.
* Updation können in diesem Modul ohne Web-Suche durchgeführt werden.
