=================
Selenium Server
=================

Zusammenfassung
-------------------------

Selen ist ein portable Software-Test-Framework für Web-Anwendungen. Selen eine Aufnahme / Wiedergabe-Tool für die Erstellung von Tests ohne das Erlernen einer Testskriptsprache (Selenium IDE). Es bietet auch eine Testdomänenspezifische Sprache (Selenese) [1], um Tests in einer Reihe von gängigen Programmiersprachen wie Java, C #, Groovy, Perl, PHP, Python und Ruby zu schreiben. Die Tests können dann mit modernsten Web-Browser ausgeführt werden. Selen setzt auf Windows, Linux und Macintosh-Plattformen

Lassen Sie uns darüber, wie dieses Modul ermöglicht den Benutzern bei der Installation von Selen-Server zu sehen.

Hilfe Befehl
--------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Selen-Server-Modul enthalten sind. Es listet einige der alternativen Parameter von Selen-Server-Modul. Es beschreibt auch die Syntax für die Installation. Der Befehl help zur Selen-Server-Modul wird wie unten dargestellt.

.. code-block:: bash

	ptconfigure seleniumserver help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Selen-Server-Modul.

.. code-block:: bash

 kevell@corp:/# ptconfigure SeleniumServer help
 ******************************


  This command allows you to install Selenium Server.

  SeleniumServer, selenium-server, selenium, selenium-srv, seleniumserver

        - install
        Installs Selenium Server. Note, you'll also need Java installed
        as it is a prerequisite for Selenium
        example: ptconfigure selenium install
        example: ptconfigure selenium install --with-chrome-driver # will set the executor command to use default chrome driver


 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl für die Installation des Selenium-Server verwendet wird, ist einfach, wie Sie den Befehl, die unten gezeigt wird.

.. code-block:: bash

		ptconfigure seleniumserver install

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# ptconfigure selenium install 

 Install Selenium Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Selenium Srv        * 
 ******************************* 
 Enter Selenium Version 
 (0) 2.39 
 (1) 2.40 
 (2) 2.41 
 (3) 2.42 
 (4) 2.43 
 (5) 2.44 
 0 

 [Pharaoh Logging] Ensure module install is not checking versions 
 [Pharaoh Logging] Command 'git' found 
 [Pharaoh Logging] Command 'gitk' found 
 [Pharaoh Logging] Command 'git-cola' found 
 [Pharaoh Logging] Not installing as already installed 
 [Pharaoh Logging] Ensure module install is not checking versions 
 [Pharaoh Logging] Module Java reports itself as Installed 
 [Pharaoh Logging] Not installing as already installed 
 Creating /tmp/ptconfigure-temp-script-5204575277.sh 
 chmod 755 /tmp/ptconfigure-temp-script-5204575277.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-5204575277.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-5204575277.sh 
 --2015-03-26 15:54:02--  http://selenium-release.storage.googleapis.com/2.39/selenium-server-standalone-2.39.0.jar 
 Resolving selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)... 216.58.220.33, 2404:6800:4007:805::2001 
 Connecting to selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)|216.58.220.33|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 34603971 (33M) [application/x-java-archive] 
 Saving to: ‘selenium-server-standalone-2.39.0.jar’ 

 100%[========================================================================================================>] 3,46,03,971 48.6KB/s   in 19m
 15s 

 2015-03-26 16:13:18 (29.3 KB/s) - ‘selenium-server-standalone-2.39.0.jar’ saved [34603971/34603971] 

 Temp File /tmp/ptconfigure-temp-script-5204575277.sh Removed 
 Program Executor Deleted if existed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 SeleniumServer: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 




Option
------------

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-------------------------+---------------------------------------------+-------------+---------------------------------------------+
 | Parameters              | Alternative Parameters                      | Optionen    | Kommentare                                  |
 +=========================+=============================================+=============+=============================================+
 |Install Selenium         | anstelle von seleniumserver, wir verwenden  | Y(Yes)      | Wenn der Benutzer wünschen, den             |
 |Server? (Y/N)            | können, SeleniumServer, Selenium,           |             | Installationsprozess können sie Eingang     |
 |                         | selenium-srv , selenium-server also.        |             | als Y. gehen                                |
 +-------------------------+---------------------------------------------+-------------+---------------------------------------------+
 |Install Selenium         | anstelle von seleniumserver, wir verwenden  | N(No)       | Wenn der Benutzer wünschen, den             |
 |Server? (Y/N)            | können, SeleniumServer, Selenium,           |             | Installationsprozess können sie Eingang     |
 |                         | selenium-srv , selenium-server also.        |             | als N. beenden|                             |
 +-------------------------+---------------------------------------------+-------------+---------------------------------------------+




Vorteile
-----------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Sie können automatisierte Tests in der Programmiersprache Ihrer Wahl, wie C #, Java, Python, PHP, Perl und Rubin sowie laufende Entwicklung
  diese Tests auf andere Kombination von Browsern wie Chrome, Firefox oder IE.
