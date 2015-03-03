===========
Varnish
===========

Zusammenfassung
-------------------------

Dieses Modul hilft bei der Installation der Lack auf die Benutzer-Maschine. Lack ist ein Programm, das stark beschleunigen kann eine Website bei gleichzeitiger Reduzierung der Last auf dem Webserver. Nach den Lack der offiziellen Website, ist Lack eine "Web-Application-Beschleuniger auch als Caching HTTP Reverse Proxy bekannt". Lassen Sie uns sehen Sie hier, wie funktioniert das Modul führt die Installation von Lack von apt-get.

Hilfe Befehl
------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Lackmodul enthalten sind. Der Befehl help listet einige der alternativen Parameter der Lack. Es beschreibt auch die Syntax für die Installation von Lack. Der Befehl help unter dem Lack-Modul ist wie folgt:

.. code-block:: bash

	ptconfigure varnish help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot zeigt Ihnen über die Hilfe-Befehl unter Lackmodul.

.. code-block:: bash

	kevell@corp:/# ptconfigure Varnish help
	******************************


        This command allows you to install Varnish, the popular HTTP Cache

        Varnish, varnish

        - install
        Installs Varnish through apt-get
        example: ptconfigure varnish install

	------------------------------
	End Help

Installation
---------------

Der Befehl zum Installieren der Lack auf die Benutzer-Maschine verwendet wird, unten gezeigt.

.. code-block:: bash

	ptconfigure varnish install

Nach der Eingabe des Befehls vor, tritt die folgenden Vorgänge wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------+------------+-----------------------------------------------+
 | Parameters               | Alternative Parameters                  | Options    | Kommentar                                     |
 +==========================+=========================================+============+===============================================+
 |Install Varnish? (Y/N)    | anstelle vonVarnish, varnish können     | Y(Yes)     | Wenn der Benutzer wünschen, den               |
 |                          | ebenfalls verwendet werden.             |            | Installationsprozess können sie Eingang       |
 |                          |                                         |            | als Y. gehen                                  |
 +--------------------------+-----------------------------------------+------------+-----------------------------------------------+
 |Install Varnish? (Y/N)    | anstelle vonVarnish, varnish können     | N(No)      | Wenn der Benutzer wünschen, den               |
 |                          | ebenfalls verwendet werden.             |            | Installationsprozess können sie Eingang       |
 |                          |                                         |            | als N. Beenden|                               |
 +--------------------------+-----------------------------------------+------------+-----------------------------------------------+


Wenn der Benutzer den Installationsprozess fort, während der Ausführung der Installation wird der folgende Prozess durchgeführt:

* Liest Paketlisten.
* Baut Abhängigkeitsbaum.
* Liest Statusinformationen.
* Liste der installierten Pakete.
* Liste der zusätzlichen Pakete installiert.
* Liste der neuen Pakete installiert.
* Anzahl der Dateien aktualisiert, neu installiert, entfernt wird, nicht aktualisiert.
* Schließlich beginnen HTTP-Accelerator lackiert.
* Der folgende Screenshot zeigt die oben genannten Verfahren:

.. code-block:: bash
   
	Kevell@corp:/# ptconfigure varnish install
	Install Varnish? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Varnish !        *
	*******************************
	Creating /tmp/ptconfigure-temp-script-95745650915.sh
	chmod 755 /tmp/ptconfigure-temp-script-95745650915.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-95745650915.sh Permissions
	Executing /tmp/ptconfigure-temp-script-95745650915.sh
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        libjemalloc1 libvarnishapi1
	Suggested packages:
	varnish-doc
	The following NEW packages will be installed:
	libjemalloc1 libvarnishapi1 varnish
	0 upgraded, 3 newly installed, 0 to remove and 6 not upgraded.
	Need to get 518 kB of archives.
	After this operation, 1,653 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libvarnishapi1 amd64 3.0.5-2 [29.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjemalloc1 amd64 3.5.1-2 [76.8 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe varnish amd64 3.0.5-2 [411 kB]
	Fetched 518 kB in 3s (152 kB/s)
	Selecting previously unselected package libvarnishapi1.
	(Reading database ... 201582 files and directories currently installed.)
	Preparing to unpack .../libvarnishapi1_3.0.5-2_amd64.deb ...
	Unpacking libvarnishapi1 (3.0.5-2) ...
	Selecting previously unselected package libjemalloc1.
	Preparing to unpack .../libjemalloc1_3.5.1-2_amd64.deb ...
	Unpacking libjemalloc1 (3.5.1-2) ...
	Selecting previously unselected package varnish.
	Preparing to unpack .../varnish_3.0.5-2_amd64.deb ...
	Unpacking varnish (3.0.5-2) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libvarnishapi1 (3.0.5-2) ...
	Setting up libjemalloc1 (3.5.1-2) ...
	Setting up varnish (3.0.5-2) ...
	 * Starting HTTP accelerator varnishd
	   ...done.
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Temp File /tmp/ptconfigure-temp-script-95745650915.sh Removed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	Varnish: Success
	------------------------------
	Installer Finished
	******************************


Vorteile
------------

* Lack ist eine moderne, leistungsfähige Open-Source-Caching Reverse HTTP-Proxy-Implementierung.
* Die Hilfe Befehl deklarieren verwendeten Parameter werden Installation nicht beachtet, welche ein zusätzlicher Vorteil ist, während im 
  Vergleich zu anderen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.

