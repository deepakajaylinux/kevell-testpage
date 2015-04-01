============
Pear
============


Zusammenfassung
----------------------

PEAR ist die Abkürzung für "PHP-Erweiterung und Application Repository" und ist genau wie die Frucht ausgeprägt. Der Zweck ist die Bereitstellung von PEAR:

* Eine strukturierte Sammlung von Open-Source-Code für PHP-Benutzer
* Ein System zur Code-Distribution und Paketverwaltungs
* Ein Standard-Stil für Code in PHP geschrieben, hier angegebenen
* Die PHP-Erweiterung Community Library (PECL)


PEAR-Mission ist es, wiederverwendbare Komponenten, führen Innovationen in PHP zur Verfügung stellen Best Practices für die PHP-Entwicklung und zu erziehen Entwickler.

Der Code in PEAR in "Pakete" aufgeteilt. Jedes Paket ist ein eigenes Projekt mit einem eigenen Entwicklungsteam, Versionsnummer, Release-Zyklus, Dokumentation und einem definierten Verhältnis zu anderen Paketen (einschließlich Abhängigkeiten). Pakete werden gzipped tar-Dateien mit einer Beschreibungsdatei im Inneren verteilt und auf dem lokalen System mit dem PEAR Installer installiert.

Hilfe Befehl
----------------------

Dieser Befehl hilft, die Verwendung von PEAR-Modul zu bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
	        ptconfigure pear help

The pictorial representation of the above command is listed below,

.. code-block:: bash


 kevell@corp:/# ptconfigure pear help
 ******************************


  This command allows you to modify create or modify pears

  Pear, pear

        - install
        Install
        example: ptconfigure pear pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure pear pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure pear pkg-ensure --package-name="somename"
        
 ------------------------------
 End Help


Install
---------------

Wenn der Benutzer müssen eine Birne zu installieren , wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure pear pkg-install --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-install --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************


Remove
------------

Wenn der Benutzer braucht, um ein System Birne zu entfernen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash

	ptconfigure pear pkg-remove --package-name="somename"

.. code-block:: bash


Ensure
---------

Wenn der Benutzer braucht, um eine Birne zu gewährleisten , wird der unten angegebenen Befehl den Prozess und führen .

.. code-block:: bash

	ptconfigure pear pkg-ensure --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-ensure --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************



Alternative Parameter
--------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

Pear, pear


Vorteile
--------------
 
Pear.php.net bietet sowohl eine menschenfreundliche (HTML) und maschinenfreundlich (derzeit REST) Schnittstelle zu den von pear.php.net Pakete. Die gesamte Kommunikation findet über das HTTP-Protokoll. Weitere Funktionen der pear.php.net Website bietet, sind:


* Benutzerkontenverwaltung (unabhängig von der SVN-Server)
* Paketverwaltung
* Release-Management
* Well-to-do in Ubuntu und Cent OS
* Nicht Groß- und Kleinschreibung

