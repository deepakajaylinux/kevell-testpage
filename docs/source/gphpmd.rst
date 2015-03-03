=========
PHPMD
=========

Zusammenfassung
-----------------------

PHP MessDeductor ist ein Spin-off der PHP ab, und zielt darauf ab, ein PHP, das von dem bekannten Java-Tool PMD sein. PHPMD kann als benutzerfreundliche Frontend-Anwendung für den rohen Messdaten Strom gemessen mit PHP Depend sehen. Allgemeine Sicherheiten oder GC ist das Spektrum der Vermögenswerte, die in den Repo-Markt von der Mehrheit der Vermittler am Markt und zu einem sehr ähnlichen Reposatz akzeptiert werden, zu einem bestimmten Zeitpunkt, als Sicherheiten. Dies eignet sich mit Ubuntu und Cent OS.

Hilfe Befehl
----------------------

  Es dauert eine bestimmte PHPMD Quellcodes und nach mehrere potentielle Probleme innerhalb dieser Quelle. PHPMD ist ein junges Projekt und bietet somit nur eine begrenzte Anzahl von vordefinierten Regeln, gegenüber PMD, die Code Gerüche und mögliche Fehler in der analysierten Quellcode zu erkennen. Kasse der Abschnitt Regeln, um mehr über allimplemented Regeln zu lernen. Der folgende Befehl help führt den Benutzer zu phpmd Module installiert.

.. code-block:: bash

		ptconfigure PHPMD help

Der folgende Screenshot vizualize seine Funktionen.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPMD help
 ******************************


  This command allows you to install PHPMD from a GC Repo.

  PHPMD

        - install
        Installs the latest GC Repo version of PHPMD
        example: ptconfigure phpmd install

 ------------------------------
 End Help
 ******************************

Installation
-------------------------

Im Moment kommt PHPMD mit den folgenden drei Renderer:

* Xml, die den Bericht als XML formatiert.
* Text, einfache Textformat.
* Html, einzelne HTML-Datei mit möglichen Problemen.

Der Befehl zum Installieren der PHPMD zum Benutzer Maschine verwendet wird unten gezeigt.

.. code-block:: bash

		ptconfigure PHPMD install

Nach der Eingabe des Befehls oben, passiert folgendes Verfahren wie im Screenshot-Format angezeigt.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpmd install
 Install PHP Mess Detector ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mess Dt.        *
 *******************************
 What is the program data directory? Found "/opt/phpmd" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpmd.git'  /tmp/phpmd/phpmdCloning into '/tmp/phpmd/phpmd'...
 remote: Counting objects: 356, done.
 remote: Total 356 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (356/356), 306.45 KiB | 9.00 KiB/s, done.
 Resolving deltas: 100% (239/239), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 PHPMD: Success
 ------------------------------
 Installer Finished
 ******************************

Optionen 
------------


.. cssclass:: tabe-bordered


 +-----------------------------+-------------------------+----------------------+----------------------------------------------------------+
 | Parameters                  | Verzeichnis (Standard)  | Optionen             | Kommentare                                               |
 +=============================+=========================+======================+==========================================================+
 |Data directory (Default)     | Yes                     | “/opt/PHPMD”         | It will install PHPMD module unter ptconfigure           |
 +-----------------------------+-------------------------+----------------------+----------------------------------------------------------+
 |Data directory               | No                      | End Schrägstrich     | Der Benutzer muss den Pfad ein.                          |
 +-----------------------------+-------------------------+----------------------+----------------------------------------------------------+
 |Executor directory (Default) | Yes                     | “/usr/bin”           | Es wird Testamentsvollstrecker Verzeichnis installieren  |
 +-----------------------------+-------------------------+----------------------+----------------------------------------------------------+
 |Executor directory           | No                      | No Schrägstrich      | Der Nutzer ist damit Eingang als Verzeichnisname|        |
 +-----------------------------+-------------------------+----------------------+----------------------------------------------------------+




Vorteile
------------------

ExcessivePublicCount:
 
Eine große Anzahl von öffentlichen Methoden und Attribute in einer Klasse deklariert die Klasse angeben müssen als größere Anstrengungen, um 
gebrochen zu werden, wird verpflichtet werden, bereits ausgiebig testen.


ExcessiveParameterList:

Lange Parameterlisten können angeben, dass ein neues Objekt erstellt werden soll, um die Vielzahl von Parametern zu wickeln. Grundsätzlich versuchen, die Parameter-Gruppe zusammen.


CyclomaticComplexity:

Die Komplexität wird durch die Anzahl von Entscheidungspunkten in einem Verfahren sowie eine für den Verfahrenseintrag bestimmt.


Superglobale:

Direkten Zugriff auf eine super-globalen Variablen gilt als eine schlechte Praxis. Diese Variablen sollten in Objekten gekapselt, die vorgesehensind durch einen Rahmen, zum Beispiel.


ShortVariable:

Erkennt, wenn ein Feld, verfügt über lokale oder Parameter eine sehr kurze Namen.


LongVariable:

Erkennt, wenn ein Feld, wird formell oder lokale Variable mit einem langen Namen erklärt.

