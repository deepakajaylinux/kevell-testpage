==========
Composer
==========

Zusammenfassung
-----------------

Komponist ist ein auf Anwendungsebene Abhängigkeit-Manager für die PHP Programmiersprache, die ein Standardformat zum Verwalten von Abhängigkeiten von PHP-Software und benötigten Bibliotheken bereitstellt.

Es ermöglicht Ihnen die abhängigen Bibliotheken zu deklarieren, die Ihr Projekt braucht und es wird ihnen in Ihrem Projekt für Sie zu installieren. Komponist ist Multi-Plattform und wir bemühen uns zu machen, ebenso gut auf Windows, Linux und OSX ausgeführt.


Hilfe Befehl
-------------

Dieser Befehl hilft, die Verwendung von Komponist Modul bestimmen. Der Benutzer wird kommen, über die verschiedenen Möglichkeiten/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer über die alternative Parameter und den Befehl für die Installation. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

             ptconfigure Composer Help

.. code-block:: bash

 kevell@corp:/# ptconfigure composer help
 ******************************


  This command allows you to update Composer.

  Composer, composer

        - install
        Installs the latest version of composer
        example: ptconfigure composer install

 ------------------------------
 End Help
 ******************************

Installation
------------------

Wenn der Benutzer Komponist-Modul installiert, in der Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.

.. code-block:: bash

	ptconfigure composer install

Während der Installation, das System Fragen für den Verzeichnisnamen, wenn Sie Ihren Pfad einrichten will, können Sie Ihre Pfad definieren. Definieren Sie Ihren Weg zu sein, gefolgt von ' /' symbol hat. Drücken Sie die EINGABETASTE, um die Standard-Pfad zu verwenden.

"Was ist das Programmverzeichnis Daten?"/ opt/Komponist"- verwenden Sie diese?

Während der Installation, das System Fragen zum Ausführen von Verzeichnisnamen an, wenn Sie Ihren Pfad einrichten will, können Sie Ihre Pfad definieren. Definieren Sie Ihren Weg zu sein, gefolgt von ' /' symbol hat. Drücken Sie die EINGABETASTE, um die Standard-Pfad zu verwenden.

"Was ist das Programmverzeichnis Executer? -"/ Usr/bin" gefunden verwenden Sie diese? “


.. cssclass:: table-bordered


 +-------------------------------+---------------------------------+------------------+------------------------------------------------+
 | Parameter 			 | Alternative Parameter	   | Option	      | Kommentare				       |
 +===============================+=================================+==================+================================================+
 |ptconfigure composer Install   | Composer , composer             | Y                | System startet Installation                    |
 +-------------------------------+---------------------------------+------------------+------------------------------------------------+
 |ptconfigure composer Install   | Composer , composer             | N                | System stoppt Installation process|            |
 +-------------------------------+---------------------------------+------------------+------------------------------------------------+

Der Screenshot zur Installation Befehl aufgeführt unten ,

.. code-block:: bash

 kevell@corp:/$ ptconfigure composer install
 Install Composer - Update to latest version ? (Y/N) 
 Y
 ******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...

 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 6
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data Folder /opt/composer Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Composer: Success
 ------------------------------
 Installer Finished
 ******************************

          
Vorteile
------------

* Abhängigkeiten (z.B. Bibliotheken) für eine Anwendung wird installiert.
* Es erlaubt auch Benutzern, PHP-Anwendungen installieren, die stehen auf "Packagist", die seine Main ist Repository mit verfügbaren Pakete.
* Darüber hinaus automatisch laden Funktionen für Bibliotheken, die Auto laden Angaben verwenden, um die Verwendung von Drittanbieter-Code zu 
  vereinfachen.
 

