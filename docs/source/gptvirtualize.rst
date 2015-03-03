=============
PTVirtualize
=============

Zusammenfassung
-----------------------

  ptvirtualize zu erreichen, um die Virtualbox verwalten. Dieses Modul hilft, unter ptconfigure installieren. Data-Verzeichnis und Vollstrecker Verzeichnis angeben können während der Installation in diesem Modul. Dieses Modul ist am bequemsten mit Ubuntu und Cent-OS.

Hilfe Befehl
---------------

Dieser Befehl help führen den Benutzer zu ptvirtualize Modul. Dies eignet sich für alle Arten von Geschäftsleuten. Der Befehl help zeigt eine kurze Liste der Befehle in das ptvirtualize Modul gebaut.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize help
	******************************


	This command allows you to install or update ptvirtualize.

	ptvirtualize, ptvirtualize

        - install
        Installs the latest version of ptvirtualize
        example: ptconfigure ptvirtualize install

	------------------------------
	End Help
	******************************
Installation
------------

Installation eines ptvirtualize Modul ist einschließlich Gerätetreiber und Plugins, Akt der das Programm zur Ausführung bereit. Während der Installation dieses Moduls wird folgendes Kommando übergeben werden.

.. code-block:: bash

	ptconfigure ptvirtualize install
Nach Den Befehl das System an ist

Install ptvirtualize?(Y/N)

Wenn der Benutzer gibt Y dann ptvirtualize installiert werden. Der folgende Screenshot zeigen es.
.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ptvirtualize         *
	*******************************
	What is the program data directory? Found "/opt/ptvirtualize" - use this? (Enter nothing for yes, no end slash)

	What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

	git clone 'https://github.com/PharaohTools/ptvirtualize.git'  /tmp/ptvirtualize/ptvirtualizeCloning into '/tmp/ptvirtualize/ptvirtualize'...
	remote: Counting objects: 4063, done.
	remote: Total 4063 (delta 0), reused 0 (delta 0)
	Receiving objects: 100% (4063/4063), 2.13 MiB | 393.00 KiB/s, done.
	Resolving deltas: 100% (2530/2530), done.
	Checking connectivity... done.
	Program Data folder populated
	Program Executor Deleted if existed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	ptvirtualize: Success
	------------------------------
	Installer Finished
	******************************

Wenn der Benutzer gibt N, dann wird es den Bildschirm zu verlassen. Der folgende Screenshot zeigen es.

.. code-block:: bash

	kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
        N	
	******************************


	Single App Installer:
	--------------------------------------------
	ptvirtualize: Failure
	------------------------------
	Installer Finished
	******************************

Option
-----------

.. cssclass:: table-bordered


 +--------------------------+----------------+-----------------------------+----------------------------------------------------+
 | Parameters               | Verzeichnis    | Option                      | Bemerkung                                          |
 +==========================+================+=============================+====================================================+
 |Data directory(DEFAULT)   | YES            | “/opt/ptvirtualize”         | Es wird installiert ptvirtualize uter ptconfigure  |
 +--------------------------+----------------+-----------------------------+----------------------------------------------------+
 |Data directory            | No             | End Schrägstrich            | Der Benutzer muss den Pfad ein.                    |
 +--------------------------+----------------+-----------------------------+----------------------------------------------------+
 |Executor directory        | Yes            | “/usr/bin”                  | Es wird Testamentsvollstrecker Verzeichnis         | 
 |(Default)                 |                |                             | installieren                                       |
 +--------------------------+----------------+-----------------------------+----------------------------------------------------+
 |Executor directory        | No             | No Schrägstrich             | Der Nutzer ist damit Eingang als Verzeichnisname|  |
 +--------------------------+----------------+-----------------------------+----------------------------------------------------+



Vorteile
---------

* Ubuntu-Anwender können einfach installieren ptvirtualize aus dem Repository.
* Der eigentliche Vorteil von ptvirtualize liegt in seiner Leistung.
* Integration mit Host-Betriebssystem.
* Geschwindigkeit Zugänglichkeit.
* Verwalten von virtuellen Box.

