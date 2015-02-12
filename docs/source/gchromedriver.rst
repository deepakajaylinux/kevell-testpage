=================
ChromeDriver
=================

Übersicht
------------

Dieses Modul erlaubt den Benutzern, paar GC empfohlenen Standard-Tools zu installieren, die locken, Vim, Drush und Postleitzahl enthält. Um den Chrom zu erhalten installiert die Benutzer muss Java installiert bekommen. Lassen Sie uns sehen Sie, über wie Sie diese nutzen und wie installiere ich die in anstehenden Themen.

Help-Befehl
-------------


Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in dem Chrom-Treibermodul enthalten sind. Der Hilfebefehl listet alternative Ausgabeparameter des Chrom-Treibermodul. Es beschreibt auch die Syntax für die Installation von Chrome-Treibermodul. Der Help-Befehl für Chrome-Treibermodul wird gezeigt wie unten beschrieben.

.. code-block:: bash

	cleopatra ChromeDriver help


Die Syntax zum Deklarieren des Help-Befehls ist nicht Groß-/Kleinschreibung einen zusätzlichen Vorteil. Der folgende Screenshot visualisieren Sie über den Befehl Help unter Chrom-Treiber.


.. code-block:: bash

 kevell@corp:/# cleopatra ChromeDriver help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  ChromeDriver, chromedriver-server, chromedriver, chromedriver-srv, chromedriverserver

        - install
        Installs ChromeDriver. Note, you'll also need Java installed
        as it is a prerequisite for ChromeDriver
        example: cleopatra chromedriver install

 ------------------------------
 End Help
 ******************************



Installation
------------------


Chrom-Treiber auf Ihrem Rechner installieren, kann getan werden, indem mithilfe des folgenden Befehls, wie gezeigt:

.. code-block:: bash

 	cleopatra-Chromedriver install


Nach den oben genannten Befehl eingeben, tritt die folgenden Vorgänge wie in tabellarischer Form dargestellt.

.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------+-----------+------------------------------------------------+
 | Parameter		    | Alternative Parameter			| Optionen  | Kommentare				     |
 +==========================+===========================================+===========+================================================+
 |Install ChromeDriver      | anstelle von Chrome Chrome Driver Driver  | Y(Yes)    | Wenn der Benutzer den Installationsvorgang     |
 |Server? (Y/N)	            | wir können server, Chrome Driver,         |           | fortsetzen möchten, können sie als Y eingeben. |
 |			    | Driver Chrome server, Chrome Driver Srv   |	    |						     |
 |			    | auch noch					| 	    | 						     |
 +--------------------------+-------------------------------------------+-----------+------------------------------------------------+
 |Install ChromeDriver      | anstelle von Chrome Chrome Driver Driver  | N(No)     | Wenn der Benutzer den Installationsvorgang     |
 |Server? (Y/N)             | wir können server, Chrome Driver,         |           | zu beenden möchten können sie eingeben, als N. |
 |                          | Driver Chrome server, Chrome Driver Srv   |           |                                                |
 |                          | auch noch|                                |           |                                                |
 +--------------------------+-------------------------------------------+-----------+------------------------------------------------+

 
Wenn der Benutzer den Vorgang der Installation während der Ausführung der Installation verläuft, fordert der Prozess den Benutzer auf

.. code-block:: bash

	Enter Chrome driver version

Chrom-Treiber-Versionen, die verfügbar sind, sind unten aufgeführt:

.. code-block:: bash

 0. 2.0
 1. 2.10
 2. 2.1
 3. 2.11
 4. 2.2
 5. 2.3
 6. 2.4
 7. 2.5
 8. 2.6
 9. 2.7
 10. 2.8
 11. 2.9


Der Benutzer hat die Zahlen von 0 bis 11 abhängig von den Anforderungen der Version angeben.

Nachdem der Benutzer die Version angibt der Prozess der Installation beginnt und ruft abgeschlossen so bildhaft aus der folgenden Bildschirmabbildung dargestellt.

.. code-block:: bash

 kevell@corp:/# cleopatra chromedriver install

 Install ChromeDriver Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         ChromeDriver        *
 *******************************
 Enter Chrome Driver Version
 (0) 2.0 
 (1) 2.10 
 (2) 2.1 
 (3) 2.11 
 (4) 2.2 
 (5) 2.3 
 (6) 2.4 
 (7) 2.5 
 (8) 2.6 
 (9) 2.7 
 (10) 2.8 
 (11) 2.9 
 11
 PHP Notice:  Undefined index: version in /opt/cleopatra/cleopatra/src/Modules/ChromeDriver/Model/ChromeDriverAllLinux.php on line 42
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/cleopatra-temp-script-26804823734.sh
 chmod 755 /tmp/cleopatra-temp-script-26804823734.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-26804823734.sh Permissions
 Executing /tmp/cleopatra-temp-script-26804823734.sh
 --2015-02-02 21:35:49--  http://chromedriver.storage.googleapis.com//chromedriver_linux64.zip
 Resolving chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)... 74.125.236.44, 74.125.236.43, 74.125.236.42, ...
 Connecting to chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)|74.125.236.44|:80... connected.
 HTTP request sent, awaiting response... 404 Not Found
 2015-02-02 21:35:52 ERROR 404: Not Found.
 
 mv: cannot stat '/tmp/chromedriver/*': No such file or directory
 unzip:  cannot find or open chromedriver_linux64.zip, chromedriver_linux64.zip.zip or chromedriver_linux64.zip.ZIP.
 Temp File /tmp/cleopatra-temp-script-26804823734.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 ChromeDriver: Success
 ------------------------------
 Installer Finished
 ******************************



Vorteile
------------


* Die verwendeten Parameter für das Deklarieren von Help-Befehl, Installation sind nicht Groß-/Kleinschreibung ist ein zusätzlicher Vorteil, 
  während im Vergleich zu anderen.
* Es ist gut situierten in beiden Cent OS und auch wie Ubuntu.
* Der Benutzer kann die Version angeben, dass, die Sie während der Installation 

