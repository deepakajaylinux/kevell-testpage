================
Ubuntu Compiler
================

Zusammenfassung
-------------------------

Dieses Modul beleben c-Programm. Ubuntu und anderen Linux-Distributionen haben umfangreiche Paket-Depots, um den Benutzer von der Mühe der Erstellung zu speichern. Mit nur einem einzigen Befehl können Sie aus den Quellen wie ein Profi zu bauen. Es ist bequem mit Ubuntu und CentOS.

Hilfe Befehl
--------------

Dieser Befehl help führen den Benutzer zu Ubuntu-Compiler. Es ist weniger zeitaufwendig, da es automatisch installiert werden können. Geeignet für C-Programm

.. code-block:: bash

		ptconfigure Ubuntucompiler help

Der folgende Befehl help wird der Benutzer für die Installation zu unterstützen.

.. code-block:: bash

	kevell@corp:/# ptconfigure UbuntuCompiler help
	******************************


         This allows you to Complie programs written in C Source

          UbuntuCompiler, ubuntu-compiler, ubuntucompiler

        - install
        Installs Ubuntu Compiling tools through apt-get.
        example: ptconfigure ubuntu-compiler install

	------------------------------
	End Help
	******************************


Installation
--------------

Dies ist eine deutliche Prozess Ubuntu-Compiler-Modul unter ptconfigure installieren, indem einfach mit dem Befehl unten angegeben,

.. code-block:: bash

  		ptconfigure Ubuntu-compiler install

Nachdem er den Befehl, wird die Ubuntu-Compiler mit neuen Updates installiert werden.

Wenn die Benutzereingabe als N wird der folgende Bildschirm kommen.

.. code-block:: bash

	Kevell@corp:/# ptconfigure UbuntuCompiler install
	Install Ubuntu Compiler? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	UbuntuCompiler: Failure
	------------------------------
	Installer Finished
	******************************



option
-----------

.. cssclass:: table-bordered

 +-----------------------------+------------------------------+-------------+-----------------------------------------------+
 | Parameters                  | Alternative parameter        | option      | Kommentar                                     |
 +=============================+==============================+=============+===============================================+
 |Install Ubuntu compiler? Y/N | UbuntuCompiler,              | Yes         | erfolgreich installiert                       |
 |                             | ubuntu-compiler,             |             |                                               |
 |                             | ubuntucompiler               |             |                                               |
 +-----------------------------+------------------------------+-------------+-----------------------------------------------+
 |Install Ubuntu compiler? Y/N | UbuntuCompiler,              | No          | Verlassen Sie das Bild                        |
 |                             | ubuntu-compiler,             |             |                                               |
 |                             | ubuntucompiler|              |             |                                               |
 +-----------------------------+------------------------------+-------------+-----------------------------------------------+


Vorteile
-----------

* Schnellere Boot
* Mehr Sicherheit
* Ändern des Kernelzuvorzukommen, während Kompilierung
* Geeignet für C-Programm
