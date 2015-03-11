========
PhpUnit
========

Zusammenfassung
-------------------------

PHPUnit ist ein Unit Testing Framework für die Programmiersprache PHP in tesingkamen. Es ist eine Instanz der Architektur zur Einheit Test-Frameworks, die mit initialisiert php Testsuite entstanden und wurde populär mit pttest.

Es funktioniert auf zwei Arten. Sie sind init und auszuführen. Es ist wertvoll, um mit Ubuntu und CentOS arbeiten.

Hilfe Befehl
---------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der PHPUnit-Module enthalten sind. Der Befehl help Listen aus der alternativen Parameter PHPUnit unter pttest Modul. Es beschreibt auch die Syntax für die Initialisierung der Maschine des Benutzers. Der Befehl help für phpunit ist nachfolgend dargestellt.

.. code-block:: bash
	
	pttest phpunit help

Die Syntax für den Befehl help non-und Kleinschreibung, die einen Vorteil für das Modul erstellt. Der folgende Screenshot den Benutzer über den Befehl help unter Systemerkennung zu visualisieren.

.. code-block:: bash

 kevell@corp:/# pttest PHPUnit help
 ******************************


  This command allows you to initialize a PHPUnit test suite.

  PHPUnit, phpunit

        - init, initialize
        Initialises the PHPUnit test suite of this project
        example: pttest phpunit init
        example: pttest phpunit initialize

        - execute
        Executes the PHPUnit test suite of this project
        example: pttest phpunit execute

 ------------------------------
 End Help
 ******************************

Alternative Parameter
---------------------------

Anstelle der Verwendung von phpunit den Benutzer können die folgenden Parameter altenative zu nutzen.

PHPUnit,  phpunit

Nach der Eingabe des System kann als initialisieren PHPUnit in Frage stellen? J / N. Dies kann durch das folgende Screenshot erklären.

.. code-block:: bash

 kevell@corp:/# pttest phpunit init
 Initialize PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79746566500.sh
 chmod 755 /tmp/ptconfigure-temp-script-79746566500.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79746566500.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79746566500.sh
 Temp File /tmp/ptconfigure-temp-script-79746566500.sh Removed
 Creating /tmp/ptconfigure-temp-script-57284647129.sh
 chmod 755 /tmp/ptconfigure-temp-script-57284647129.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-57284647129.sh Permissions
 Executing /tmp/ptconfigure-temp-script-57284647129.sh
 Temp File /tmp/ptconfigure-temp-script-57284647129.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitInit: Success

 ------------------------------
 Installer Finished
 ******************************

ausführen
-------------

Diese führen Sie hilft dem Anwender, PHPUnit Testsuite von pttest ausführt. Programme für ein System kann in einem Batch-Verfahren ohne menschliche Interaktion auszuführen, oder ein Benutzer kann Befehle in einer interaktiven Sitzung eines Dolmetschers geben. Mit dem folgenden Befehl wird verwendet, um phpunit auszuführen.

.. code-block:: bash

	pttest phpunit execute

Nach der Eingabe des Befehls ist eine Frage stellen. Es kann durch das folgende Bild visualisiert werden.

.. code-block:: bash

 kevell@corp:/# pttest phpunit execute
 Execute PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-23757829034.sh
 chmod 755 /tmp/ptconfigure-temp-script-23757829034.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23757829034.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23757829034.sh
 /tmp/ptconfigure-temp-script-23757829034.sh: 3: /tmp/ptconfigure-temp-script-23757829034.sh: phpunit: not found
 Temp File /tmp/ptconfigure-temp-script-23757829034.sh Removed
 Creating /tmp/ptconfigure-temp-script-85280710426.sh
 chmod 755 /tmp/ptconfigure-temp-script-85280710426.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85280710426.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85280710426.sh
 Temp File /tmp/ptconfigure-temp-script-85280710426.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitExec: Success

 ------------------------------
 Installer Finished
 ******************************


Option
--------------


.. cssclass:: table-bordered

 +-----------------------------------+-----------+-----------------------------------------------+
 | Parameters                        | Option    | Kommentare                                    |
 +===================================+===========+===============================================+
 |Initialize Phpunit? (Y/N)          | Yes       | phpunit unter pttest initialisiert werden.    | 
 +-----------------------------------+-----------+-----------------------------------------------+
 |Execute Phpunit? (Y/N)             | Yes       | PHPUnit kann unter pttest ausgeführt werden.  |
 +-----------------------------------+-----------+-----------------------------------------------+
 |Initialize Phpunit/                | No        | Es kann den Bildschirm zu verlassen           |
 |Execute Phpunit? (Y/N)|            |           |                                               |
 +-----------------------------------+-----------+-----------------------------------------------+


Vorteile
----------

* PHPUnit mit der Ansicht, dass die früher Sie Ihren Code Fehler erkennen, desto schneller können Sie sie zu beheben erstellt.
* Wie alle Unit-Tests Frameworks PHPUnit Aussagen verwendet, um dieses Verhalten der Einheit von Code unter Test überprüfen verhält wie erwartet.
* PHPUnit ausgeben kann Testergebnisse in einer Reihe von verschiedenen Formaten wie XML.
* PHPUnit kann ein nicht-Groß- und Kleinschreibung ist.
* PHPUnit Komfort mit Ubuntu und CentOS.
