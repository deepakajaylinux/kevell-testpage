==========
Xcache
==========

Zusammenfassung
------------------

XCache ist eine freie, quelloffene Operationscode Cacher, es soll die Leistung von PHP-Skripten-Ausführung auf Servern zu erhöhen. Es optimiert die Leistung durch den Wegfall der Kompilierung von PHP Code durch caching die kompilierte Version des Codes in den Speicher und auf diese Weise die kompilierte Version lädt das PHP-Skript direkt aus dem Speicher.

Hilfe Befehl
---------------

Dieser Befehl hilft, um die Verwendung von Xcache zu bestimmen. Es listet die alternative Ausgabeparameter von Xcache. Es beschreibt auch die Syntax für Xcache Modul funktionieren. Der Help-Befehl für Xcache wird gezeigt wie unten beschrieben.


.. code-block:: bash

	ptconfigure xcache help

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache help
 ******************************


  This command allows you to update Xcache.

  Xcache, xcache

        - install
        Installs the latest version of xcache
        example: ptconfigure xcache install

 ------------------------------
 End Help
 ******************************


Installation
-------------


Der Befehl für die Installation von Xcache-Modul auf dem Terminal ist im folgenden aufgeführt,


.. code-block:: bash

        ptconfigure xcache install

Der obige Befehl soll die neueste Version von Xcache und seine Abhängigkeiten zu installieren...   

Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache install
 Install Xcache? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Xcache!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-56147605410.sh
 chmod 755 /tmp/ptconfigure-temp-script-56147605410.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-56147605410.sh Permissions
 Executing /tmp/ptconfigure-temp-script-56147605410.sh
 --2015-03-20 17:05:11--  http://kr.archive.ubuntu.com/ubuntu/pool/universe/x/xcache/php5-xcache_3.1.0-2_amd64.deb
 Resolving kr.archive.ubuntu.com (kr.archive.ubuntu.com)... 103.22.220.133
 Connecting to kr.archive.ubuntu.com (kr.archive.ubuntu.com)|103.22.220.133|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 108582 (106K) [application/x-debian-package]
 Saving to: ‘php5-xcache_3.1.0-2_amd64.deb.1’

 100%[=======================================================================================================>] 1,08,582    36.1KB/s   in 2.9s   

 2015-03-20 17:05:15 (36.1 KB/s) - ‘php5-xcache_3.1.0-2_amd64.deb.1’ saved [108582/108582]

 php5_invoke xcache: already enabled for apache2 SAPI
 php5_invoke xcache: already enabled for cli SAPI
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 (Reading database ... 195553 files and directories currently installed.)
 Preparing to unpack php5-xcache_3.1.0-2_amd64.deb ...
 Unpacking php5-xcache (3.1.0-2) over (3.1.0-2) ...
 Setting up php5-xcache (3.1.0-2) ...
 * Restarting web server apache2
   ...done.
 Temp File /tmp/ptconfigure-temp-script-56147605410.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xcache: Success
 ------------------------------
 Installer Finished
 ******************************



Alternative Parameter
-----------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden können.

Xcache, xcache


Vorteile
-----------

* Stabiler Betrieb 
* schnelle Anpassung an neueren PHP-Versionen 
* einfache Installation








