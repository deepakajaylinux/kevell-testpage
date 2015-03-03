===========
PHPModules
===========

Zusammenfassung
-----------------------

Diese Module zielt auf die Installation und Kuvertierung einige der häufigsten und hilfsbereit, die Unterstützung von PHP-Modulen. Einige Beispiele sind: php5-gd das Bild libs, php5-imagick das Bild libs, php5-curl dem entfernten Datei-Handling-Bibliotheken, php5-mysql die Bibliotheken für den Umgang mit MySQL-Verbindungen. Wir wollen sehen, wie dieses Modul, den Prozess der Installation im kommenden Themen verwenden.

Hilfe Befehl
----------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der PHP-Modul enthalten sind. Es listet einige der alternativen Parameter der PHP-Modul. Es beschreibt auch die Syntax für die Installation des PHP-Moduls. Der Befehl help for Php-Modul wird wie unten dargestellt.

.. code-block:: bash
	
		ptconfigure PHPModules help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP-Modul.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************

Installation
--------------

Der Befehl für die Installation der PHP-Module in der Benutzer-Maschine verwendet wird, wie folgt dar:

.. code-block:: bash

		ptconfigure phpmods install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 | Parameters                  | Alternative Parameter                             | Optionen  | Kommentare                              |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 |Install PHP Modules? (Y/N)   | anstelle von phpmods,Die wir verwenden können     | Y(Yes)    | Wenn der Benutzer wünschen, den         |
 |                             | PHPModules, php-mods, php-modules, phpmodules     |           | Installationsprozess können sie Eingang |
 |                             | also.                                             |           | als Y. gehen                            |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+
 |Install PHP Modules? (Y/N)   | anstelle von phpmods,Die wir verwenden können     | N(No)     | Wenn der Benutzer wünschen, den         |
 |                             | PHPModules, php-mods, php-modules, phpmodules     |           | Installationsprozess können sie Eingang |
 |                             | also.                                             |           | als N. beenden|                         |
 +-----------------------------+---------------------------------------------------+-----------+-----------------------------------------+

Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:


* Baut die Abhängigkeitsstruktur.
* Liest den Status Informationen.
* Liste outs die Pakete, die automatisch installiert werden.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.



Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install
 
 Install PHP Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mysql from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Alle die häufig verwendete PHP-Module der Installation wird in einer einzigen Prozess gehüllt.
