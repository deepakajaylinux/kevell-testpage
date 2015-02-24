=======
PHPAPC
=======

Zusammenfassung
-------------------------

Dieses Modul soll die Installation der PHP APC an die Benutzer-Maschine auf alle möglichen Arten.

APC ist eine der beliebtesten Caching-Mechanismus für die PHP-Op-Code-Caching. Einmal aktiviert, startet automatisch das Caching PHP-Codes. Es funktioniert auch gut mit W3 Total Cache Plugin zur Speicherung von Objekt & MySQL-Caches.

Die anstehenden Themen werden vollständig in jeder Hinsicht in der Installation des PHP APC beteiligt führt Ihre.



Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der PHP-APC-Modul enthalten sind. Es listet einige der alternativen Parameter der PHP APC-Modul. Es beschreibt auch die Syntax für die Installation des PHP APC-Modul. Der Befehl help for Php APC-Modul wird wie unten dargestellt.

.. code-block:: bash
	
		ptconfigure PHPAPC help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPAPC help

 ******************************


  This command allows you to install some common and helpful PHP APC.

  PHPAPC, php-apc, phpapc, phpapc

        - install
        Install PHP APC.
        example: ptconfigure phpapc install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Der Befehl für die Installation der PHP-APC in der Benutzer-Maschine verwendet wird, wie folgt dar:

.. code-block:: bash
	

		ptconfigure phpapc install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +----------------------------+--------------------------------------------------------+------------+------------------------------------+
 | Parameters                 | Alternative Parameter                                  | Optionen   |  Kommentare                        |
 +============================+========================================================+============+====================================+
 |Install PHP APC? (Y/N)      | anstelle von phpapc, wir verwenden können, PHPAPC,     | Y(Yes)     | Wenn der Benutzer wünschen, den    |
 |                            | php-apc.                                               |            | Installationsprozess können sie    |
 |                            |                                                        |            | Eingang als Y. gehen               |
 +----------------------------+--------------------------------------------------------+------------+------------------------------------+
 |Install PHP APC? (Y/N)      | anstelle von phpapc, wir verwenden können, PHPAPC,     | N(No)      | Wenn der Benutzer wünschen, den    |
 |                            | php-apc.                                               |            | Installationsprozess können sie    |
 |                            |                                                        |            | Eingang als N. beenden|            |
 +----------------------------+--------------------------------------------------------+------------+------------------------------------+

Wenn der Benutzer geht der Installation, während des Prozesses der Anlage wird in den folgenden Listen beschrieben:


* Liest Paketlisten.
* Erstellt die Abhängigkeitsstruktur.
* Liest Statusinformationen.
* Liste outs die Pakete, die automatisch installiert werden.
* Liste outs das zusätzliche Paket installieren.
* Liste outs die vorgeschlagenen Pakete.
* Liste outs die neuen Pakete installieren.
* Details über die Anzahl der Dateien aktualisiert, neu installiert, entfernt und nicht aktualisiert.


Schließlich ist der Prozess der Installation abgeschlossen wird. Der folgende Screenshot visuell darstellen, den Prozess der Installation des PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpapc install

 Install PHP APC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP APC!        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  php5-apcu
 The following packages will be REMOVED:
  php5-xcache
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 1 to remove and 78 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPAPC: Success
 ------------------------------
 Installer Finished
 ******************************

APC-Funktionen
------------------


Diese Unterthemen befasst sich mit den am häufigsten verwendeten Funktionen unter APC. Während der Arbeit mit PHP APC kann der Benutzer mit diesen Funktionen des APC beziehen.

* Apc_add - Cache eine neue Variable im Datenspeicher
* Apc_bin_dump - Holen Sie sich eine binäre Dump der angegebenen Dateien und Benutzervariablen
* Apc_bin_dumpfile - Ausgabe eine binäre Dump der Cache-Dateien und Benutzervariablen in eine Datei
* Apc_bin_load - Legen Sie eine binäre Sicherung in die APC-Datei / Benutzer-Cache
* Apc_bin_loadfile - Legen Sie eine binäre Dump aus einer Datei in die APC-Datei / Benutzer-Cache
* Apc_cache_info - Ruft zwischengespeicherte Informationen aus APC-Datenspeicher
* Apc_cas - Aktualisiert einen alten Wert durch einen neuen Wert
* Apc_clear_cache - Löscht die APC-Cache
* Apc_compile_file - Speichert eine Date im Bytecode Cache unter Umgehung aller Filter.
* Apc_dec - Verringern Sie eine gespeicherte Nummer
* Apc_define_constants - Definiert eine Gruppe von Konstanten für den Abruf und die Masse-Definition-
* Apc_delete_file - Löscht Dateien aus dem Opcode-Cache
* Apc_delete - Entfernt eine gespeicherte Variable aus dem Cache
* Apc_exists - Prüft, ob APC Schlüssel vorhanden
* Apc_fetch - Holt eine gespeicherte Variable aus dem Cache
* Apc_inc - Erhöhen Sie eine gespeicherte Nummer
* Apc_load_constants - Lädt eine Reihe von Konstanten aus dem Cache
* Apc_sma_info - Ruft APC Shared Memory Allocation Informationen
* Apc_store - Cache eine Variable im Datenspeicher

Vorteile
-----------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die php apc in aktualisierte Version.
* Wenn das Modul bereits in der Benutzermaschine vorhandene es wird eine Meldung angezeigt werden, da sie bereits vorhanden sind.
* APC kommt mit Datei apc.php benannt, die über eine einfache Web-basierte Schnittstelle zur Verfügung stellt.

