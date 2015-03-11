=========
Behat
=========

Zusammenfassung
--------------------------

Dieses Modul erlaubt es dem Benutzer, Behat Testsuite zu initialisieren. Die Behat hilft bei Prüfung eines PHP-Skript. Es kann die aktiviert und deaktiviert Vorlagen markieren. Lassen Sie uns sehen, wie man init und führen Sie den teskingkamen Behat.

Hilfe Befehl
------------------

Der Befehl help führt den Anwender in Bezug auf den Zweck und die Möglichkeiten im Rahmen eines Moduls. Es listet einige der alternativen Parameter, die in der Erklärung verwendet. Es beschreibt die Syntax für Initialisierung und einen Behat unter der pttest auszuführen. Der Befehl, um Hilfe erklärt verwendet wird nachfolgend dargestellt:

.. code-block:: bash

	pttest behat help

Der folgende Screenshot zeigt bildhaft über die Arbeit der Befehl help.

.. code-block:: bash

 kevell@corp:/# pttest Behat help
 ******************************


  This command allows you to initialize a Behat test suite.

  Behat, behat

        - init, initialize
        Initialises the Behat test suite of this project
        example: pttest behat init
        example: pttest behat initialize

        - execute
        Executes the Behat test suite of this project
        example: pttest behat execute

 ------------------------------
 End Help
 ******************************

Wie Behat initialisieren
-----------------------------

Der Befehl zum Initialisieren des Behat unter pttest verwendet wird angezeigt:

.. code-block:: bash

	pttest behat init

or 

.. code-block:: bash

	pttest behat initialize

Nach der Eingabe des Befehls über das Verfahren der initialize auftritt, wie in der Tabelle unten dargestellt.

.. cssclass:: table-bordered

 +------------------------------+----------------------------------------+-----------+-------------------------------------------------+
 | Parameters                   | Alternative Parameters                 | Options   | Kommentare                                      |
 +==============================+========================================+===========+=================================================+
 |Initialize Behat (Y/N)        | Statt Behat, können wir auch Behat     | Y(Yes)    | Wenn der Benutzer wünschen, den init sie        |
 |                              |                                        |           | eingeben können, wie Y. gehen                   |
 +------------------------------+----------------------------------------+-----------+-------------------------------------------------+
 |Initialize Behat? (Y/N)       | Statt Behat, können wir auch Behat     | N(No)     | Wenn der Benutzer wünschen, den init-Prozess    |
 |                              |                                        |           | können sie Eingang als N. beenden|              |
 +------------------------------+----------------------------------------+-----------+-------------------------------------------------+


Schließlich wird die pttest Behat wird initialisiert, wie im folgenden Screenshot gezeigt.

.. code-block:: bash

 kevell@corp:/# pttest behat init
 Initialize Behat? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Behat         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-72748278108.sh
 chmod 755 /tmp/ptconfigure-temp-script-72748278108.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-72748278108.sh Permissions
 Executing /tmp/ptconfigure-temp-script-72748278108.sh
 /tmp/ptconfigure-temp-script-72748278108.sh: 3: /tmp/ptconfigure-temp-script-72748278108.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-72748278108.sh Removed
 Creating /tmp/ptconfigure-temp-script-35600300430.sh
 chmod 755 /tmp/ptconfigure-temp-script-35600300430.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-35600300430.sh Permissions
 Executing /tmp/ptconfigure-temp-script-35600300430.sh
 Temp File /tmp/ptconfigure-temp-script-35600300430.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************

Wie Sie das Behat ausführen
---------------------------

Der Befehl für die Ausführung der Behat unter pttest verwendet wird angezeigt:

.. code-block:: bash

	pttest behat execute

Wie Sie das Behat ausführen
---------------------------

Der Befehl für die Ausführung der Behat unter pttest verwendet wird angezeigt:

.. cssclass:: table-bordered 

 +------------------------+----------------------------------+----------+-------------------------------------------------------+ 
 | Parameters             | Alternative Parameters           | Options  | Kommentare                                            |
 +========================+==================================+==========+=======================================================+
 |Execute Behat (Y/N)     | Statt Behat, können wir auch     | Y(Yes)   | Wenn der Benutzer wünschen, die Ausführung            |
 |                        | Behat                            |          | können sie Eingang als Y. gehen                       |
 +------------------------+----------------------------------+----------+-------------------------------------------------------+
 |Execute Behat? (Y/N)    | Statt Behat, können wir auch     | N(No)    | Wenn der Benutzer wünschen, den                       |
 |                        | Behat                            |          | Ausführungsprozess können sie Eingang als N. beenden| |
 +------------------------+----------------------------------+----------+-------------------------------------------------------+

Wenn der Benutzer die Ausführung gehen, wird der Prozess der Ausführung auftreten, wie im folgenden Screenshot dargestellt.

.. code-block:: bash

 kevell@corp:/# pttest behat execute
 Execute Behat? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *            Behat!           *
 *******************************
 Creating /tmp/ptconfigure-temp-script-93439425208.sh
 chmod 755 /tmp/ptconfigure-temp-script-93439425208.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-93439425208.sh Permissions
 Executing /tmp/ptconfigure-temp-script-93439425208.sh
 /tmp/ptconfigure-temp-script-93439425208.sh: 2: /tmp/ptconfigure-temp-script-93439425208.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-93439425208.sh Removed
 Creating /tmp/ptconfigure-temp-script-97268122064.sh
 chmod 755 /tmp/ptconfigure-temp-script-97268122064.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-97268122064.sh Permissions
 Executing /tmp/ptconfigure-temp-script-97268122064.sh
 Temp File /tmp/ptconfigure-temp-script-97268122064.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************

Vorteile
-----------

* Es führt den Anwender, um die Fehler in PHP-Skript zu identifizieren.
* Bei Verwendung der Funktionen von Behat die Benutzer Rahmen und geben das Verhalten Driven Development können.
* Der Prozess der Initialisierung und Ausführung können im Rahmen dieser Behat von pttestt erfolgen.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Die in der Erklärung verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen Parametern.

