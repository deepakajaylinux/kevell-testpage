=================
PHPStorm
=================

Zusammenfassung
-----------------------

PhpStorm hält mit neuesten PHP & ptconfigure Trends, integriert eine Vielzahl von modernen Tools und bringt noch mehr Erweiterbarkeit mit Unterstützung für große PHP-Frameworks. Entwicklungsumgebung Auto-Konfiguration (Codierungsstandard, Dateizuordnungen, etc.) möglich. Es ist bequem mit Ubuntu und Cent-OS.

Hilfe Befehl
------------------------

Dieser Befehl kann über die Ziele und Befehle unter ptconfigure Php Sturm-Modul funktionieren. Es erklärt auch den Befehl zum Sturm PHP Modul zu installieren. Vor der Installation kann der Benutzer lesen diese Hilfe Befehl erklärt seine Funktion.

.. code-block:: bash
   
	       ptconfigure PHPStorm help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter PHP Storm.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPStorm help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  PHPStorm, phpstorm

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

Installation
------------------

Wenn der Benutzer git Werkzeuge, um ihre Maschine installieren wollen, können sie den Befehl wie unten angegeben verwenden können,

.. code-block:: bash

	ptconfigure gittools install

Nach der Eingabe des Befehls oben, sind die folgenden Schritte im Prozess der Installation beteiligt, wie in der Tabelle beschrieben,

.. cssclass:: table-bordered

 +---------------------+-------------------------------------+--------------+---------------------------------------------------------+
 | Parameters          | Alternative Parameters              | Optionen     | Kommentare                                              |
 +=====================+=====================================+==============+=========================================================+
 |Install Git Tools?   | Anstelle der Verwendung PHPStorm    | Y(Yes)       | Wenn der Benutzer wünschen, den                         |
 |(Y/N)                | Wir verwenden phpstorm              |              | Installationsprozess können sie Eingang als Y. gehen    |
 +---------------------+-------------------------------------+--------------+---------------------------------------------------------+
 |Install Git Tools?   | Anstelle der Verwendung PHPStorm    | N(No)        | Wenn der Benutzer wünschen, den                         |
 |(Y/N)                | Wir verwenden phpstorm              |              | Installationsprozess können sie Eingang als N beenden|  |
 +---------------------+-------------------------------------+--------------+---------------------------------------------------------+

Der folgende Screenshot zeigt bildhaft die oben beschriebene Prozess der Installation.

.. code-block:: bash

 
 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package gitk from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-cola from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************

Vorteile
-------------------

* Weitere Einstellungen, um Ihren Code so sauber wie möglich zu halten
* Bessere Schnittstelle mit Entwicklungsumgebung Auto-Konfiguration.
* Bessere Codehinweise & Debugging
* Zen Coding ist mit DevOps.
* Mehrere Cursor und einfache Tastenkombinationen für die Erstellung, Bearbeitung und Navigation zwischen Themen.
* Mehr Benutzerdefinierte Attribute, anpassbare Workflows und leistungsstarke Customization.
* Wird verwendet, um neueste Version von Entwickler-Tools installieren.

