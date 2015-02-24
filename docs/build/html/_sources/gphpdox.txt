=========
PHPDox
=========

Zusammenfassung
-----------------------

Mit diesem Modul können die Benutzer bei der Installation der PHP-Dox mit der neuesten Version. phpdox ist ein Dokumentationsgenerator zur Erzeugung von API-Dokumentation im HTML-Format, zum Beispiel von PHP-Quellcode. Wir wollen sehen, wie dieses Modul hilft bei der Installation der PHP-Dox.

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Phpdox Modul enthalten sind. Es listet einige der alternativen Parameter Phpdox Modul. Es beschreibt auch die Syntax für die Installation des Phpdox Moduls. Der Befehl help für Phpdox Modul wird wie unten dargestellt.

.. code-block:: bash
	
		ptconfigure Phpdox help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Phpdox.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPDox help

 ******************************

  This command allows you to update PHPDox.

   PHPDox, phpdox

         - install
         Installs the latest version of Docker
         example: ptconfigure phpdox install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl zum Installieren der phpdox im Benutzer Maschine verwendet wird unten dargestellt:

.. code-block:: bash

		ptconfigure phpdox install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-------------------------+------------------------------------------+-------------+-------------------------------------------+
 | Parameters              | Alternative Parameter                    | Optionen    |  Kommentare                               |
 +=========================+==========================================+=============+===========================================+
 |Install PHPDox? (Y/N)    | anstelle von phpdox, wir verwenden       | Y(Yes)      | Wenn der Benutzer wünschen, den           |
 |                         | können, PHPDox also.                     |             | Installationsprozess können sie Eingang   |
 |                         |                                          |             | als Y. gehen                              |
 +-------------------------+------------------------------------------+-------------+-------------------------------------------+
 |Install PHPDox? (Y/N)    | anstelle von phpdox, wir verwenden       | N(No)       | Wenn der Benutzer wünschen, den           |
 |                         | können, PHPDox also.                     |             | Installationsprozess können sie Eingang   |
 |                         |                                          |             | als N. beenden|                           |
 +-------------------------+------------------------------------------+-------------+-------------------------------------------+


Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpdox install

 Install PHPDox? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPDox!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-27804177792.sh
 chmod 755 /tmp/ptconfigure-temp-script-27804177792.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-27804177792.sh Permissions
 Executing /tmp/ptconfigure-temp-script-27804177792.sh
 --2015-01-28 15:42:36--  http://phpdox.de/releases/phpdox.phar
 Resolving phpdox.de (phpdox.de)... 188.94.27.6
 Connecting to phpdox.de (phpdox.de)|188.94.27.6|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 801185 (782K) [application/phar]
 Saving to: â€˜phpdox.pharâ€™

 100%[=======================================================================================================>] 8,01,185    11.7KB/s   in 2m 9s  

 2015-01-28 15:44:47 (6.08 KB/s) - â€˜phpdox.pharâ€™ saved [801185/801185]
 
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open 
 shared object file: No such file or directory in Unknown on line 0
 Sorry, but your PHP environment is currently not able to run phpDox due to
 the following issue(s):

 ext/xsl not installed/enabled

 Please adjust your PHP configuration and try again.



 Oups... phpDox encountered a problem and has terminated!

 It most likely means you've found a bug, so please file a report for this
 and paste the following details and the stacktrace (if given) along:

 PHP Version: 5.5.9-1ubuntu4.5 (Linux)
 PHPDox Version: 0.7.0
 ErrorException: E_CORE_WARNING 
 Location: Unknown (Line 0)
 
 PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open shared object 
 file: No such file or directory

 No stacktrace available
 

 phpDox 0.7.0 - Copyright (C) 2010 - 2015 by Arne Blankerts

 Temp File /tmp/ptconfigure-temp-script-27804177792.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 Single App Installer:
 --------------------------------------------
 PHPDox: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-----------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die phpdox in aktualisierte Version.
* Wenn das Modul bereits in der Benutzermaschine vorhandene es wird eine Meldung angezeigt werden, da sie bereits vorhanden sind.

